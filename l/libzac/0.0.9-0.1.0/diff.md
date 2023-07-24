# Comparing `tmp/libzac-0.0.9-py3-none-any.whl.zip` & `tmp/libzac-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14632 bytes, number of entries: 13
+Zip file size: 15887 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      134 b- defN 23-Jun-19 08:09 libzac/__init__.py
--rw-rw-rw-  2.0 fat     6198 b- defN 23-Jul-12 03:11 libzac/bitfield.py
--rw-rw-rw-  2.0 fat     1960 b- defN 23-May-17 07:50 libzac/dsp.py
--rw-rw-rw-  2.0 fat     4978 b- defN 23-Jun-19 08:10 libzac/e.py
--rw-rw-rw-  2.0 fat     3007 b- defN 23-May-17 07:56 libzac/io.py
--rw-rw-rw-  2.0 fat     1510 b- defN 23-May-23 02:36 libzac/math.py
+-rw-rw-rw-  2.0 fat     7782 b- defN 23-Jul-24 09:30 libzac/bitfield.py
+-rw-rw-rw-  2.0 fat     2997 b- defN 23-Jul-19 08:26 libzac/dsp.py
+-rw-rw-rw-  2.0 fat     5139 b- defN 23-Jul-20 06:16 libzac/e.py
+-rw-rw-rw-  2.0 fat     4073 b- defN 23-Jul-21 03:43 libzac/io.py
+-rw-rw-rw-  2.0 fat     4126 b- defN 23-Jul-20 07:43 libzac/math.py
 -rw-rw-rw-  2.0 fat     3074 b- defN 23-May-17 08:19 libzac/plt.py
--rw-rw-rw-  2.0 fat     8751 b- defN 23-Jul-12 03:13 libzac/reg.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1734 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      947 b- defN 23-Jul-12 03:15 libzac-0.0.9.dist-info/RECORD
-13 files, 33479 bytes uncompressed, 13090 bytes compressed:  60.9%
+-rw-rw-rw-  2.0 fat     7770 b- defN 23-Jul-13 09:53 libzac/reg.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-24 09:33 libzac-0.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1734 b- defN 23-Jul-24 09:33 libzac-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 09:33 libzac-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-24 09:33 libzac-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      947 b- defN 23-Jul-24 09:33 libzac-0.1.0.dist-info/RECORD
+13 files, 38962 bytes uncompressed, 14345 bytes compressed:  63.2%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: libzac/plt.py
 Comment: 
 
 Filename: libzac/reg.py
 Comment: 
 
-Filename: libzac-0.0.9.dist-info/LICENSE
+Filename: libzac-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: libzac-0.0.9.dist-info/METADATA
+Filename: libzac-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: libzac-0.0.9.dist-info/WHEEL
+Filename: libzac-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: libzac-0.0.9.dist-info/top_level.txt
+Filename: libzac-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: libzac-0.0.9.dist-info/RECORD
+Filename: libzac-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libzac/bitfield.py

```diff
@@ -1,162 +1,227 @@
 from __future__ import annotations
 from typing import Any
 import numpy as np
-from .e import eread, ewrite
+from .e import eread, ewrite,einput
+import classutilities
 
-########## used for debug without actually read/wrtie memory #############
-# eread = lambda addr,length: np.random.randint(0,255,length,dtype="u1")
-# ewrite = lambda addr,value: None
-##########################################################################
-
-class bitfield():
-    _fields_ = {}
-    addr = ""
+_MEMMAP = None
+
+class bitfield(object):
+    r"""
+    base class for bitfield, all bitfield should inherit from this class
+    subclass should explicitly define `_fields_` and `_addr_` to specify the bitfield layout and address, for example:
+
+    Examples
+    --------
+    >>> class BF(bitfield):
+    ...     _addr_ = 0x4ff0
+    ...     _fields_ = [
+    ...         ("A", 8),
+    ...         ("B", 12),
+    ...         ("", 2),
+    ...         ("C", 2),
+    ...     ]
+    >>> bf = BF(0x123456)
+    >>> bf.A == (0x123456 >> 0) & ((1<<8)-1)
+    True
+    >>> bf.B == (0x123456 >> 8) & ((1<<12)-1)
+    True
+    >>> bf.C == (0x123456 >> 22) & ((1<<2)-1)
+    True
+    >>> hex(bf.data)
+    '0x123456'
+    >>> np.binary_repr(bf.data,24) # doctest: +NORMALIZE_WHITESPACE
+        '000100100011010001010110'
+    >>> #CC__BBBBBBBBBBBBAAAAAAAA
+    >>> bf.A = 0
+    >>> bf.C = 2
+    >>> hex(bf.data)
+    '0x923400'
+    >>> np.binary_repr(bf.data,24) # doctest: +NORMALIZE_WHITESPACE
+        '100100100011010000000000'
+    >>> #CC__BBBBBBBBBBBBAAAAAAAA
+    >>> bf.addr
+    '4ff0'
+    >>> bf.addr_
+    20464
+    >>> bf.size
+    3
+    >>> bf.name
+    'BF'
+    >>> bf.bytes
+    b'\x004\x92'
+    >>> print(bf)
+    BF @ 4ff0 = 0x923400
+      A[7:0] = 0x0
+      B[19:8] = 0x234
+      C[23:22] = 0x2
+    <BLANKLINE>
+    >>> mem_map = {}
+    >>> load_memmap(mem_map)
+    >>> bf.write()
+    >>> mem_map
+    {20464: 0, 20465: 52, 20466: 146}
+    >>> bf2 = BF().load()
+    >>> bf2.data == bf.data
+    True
+    >>> BF.get("A")
+    0
+    >>> BF.set("B",0)
+    >>> mem_map
+    {20464: 0, 20465: 0, 20466: 144}
+    >>> BF.set(value=0x123456) # 0x12==18, 0x34==52, 0x56==86 
+    >>> mem_map
+    {20464: 86, 20465: 52, 20466: 18}
+    >>> BF.get() # 0x123456 == 1193046
+    1193046
+    >>> bf.diff(bf2) # return None if two bitfields are the same
+    >>> bf2.B = 0
+    >>> print(bf.diff(bf2))
+    BF @ 4ff0 = 0x923400 => 0x900000
+      B[19:8] = 0x234 => 0x0
+    <BLANKLINE>
+    >>> bf.jam()
+    jam 0x00,0x4ff0
+    jam 0x34,0x4ff1
+    jam 0x92,0x4ff2
+    """
+    _fields_ = []
+    _addr_ = 0
     __ENDIANESS = 'little'
     def __init__(self, data:int=0):
-        self._data = data
+        """initialize bitfield with data, data will be masked by the size of bitfield"""
+        self._data = data & ((1<<(self.size*8))-1)
         shift = 0
-        for field,bit in self._fields_.items():
+        for field,bit in self._fields_:
             mask = ((1<<bit)-1) << shift
             def getter(self, mask=mask, shift=shift): # `mask=mask` will remember current value of mask
                 return (self.data & mask) >> shift
             def setter(self, value, mask=mask, shift=shift):
                 self._data = ((value << shift) & mask) | (self.data & ~mask)
-            setattr(type(self),field,property(getter, setter))
+            if field:
+                setattr(type(self),field,property(getter, setter)) # dynamically add property to class
             shift += bit
 
-    def __str__(self): # print(bitfield) will print all info about it
-        s = f"{self.__class__.__name__} @ {self.addr} = 0x{self.data:0{self.size*2}x}\n"
+    def __str__(self):
+        """print all info about the bitfield"""
+        s = f"{self.__class__.__name__} @ {self.addr} = {self.hex}\n"
         start = 0
-        for field,bit in self._fields_.items():
-            width = f"[{start+bit-1:d}:{start:d}]" if bit > 1 else f"[{start}]"
-            s += f"  {field}{width} = {hex(getattr(self,field))}\n"
+        for field,bit in self._fields_:
+            if field:
+                width = f"[{start+bit-1:d}:{start:d}]" if bit > 1 else f"[{start}]"
+                s += f"  {field}{width} = {hex(getattr(self,field))}\n"
             start += bit
         return s
     
-    def __setattr__(self, __name: str, __value: Any) -> None: # prevent add new attribute other than _fields_
-        if __name in list(self._fields_.keys())+["_data"]:
+    def __setattr__(self, __name: str, __value: Any) -> None:
+        """prevent add new attribute other than _fields_ and _data"""
+        if __name in [field for field,bit in self._fields_]+["_data"]:
             super().__setattr__(__name, __value)
         else:
-            raise AttributeError(f"Bitfield '{self.__class__.__name__}' has no field '{__name}'")
+            raise AttributeError(f"Bitfield '{self.name}' has no field '{__name}'")
+        
+    @classutilities.classproperty
+    def addr(cls):
+        """return the address(string, '8b1c') of the bitfield"""
+        return einput(cls._addr_, output_int=False)
+    @classutilities.classproperty
+    def addr_(cls):
+        """return the address(int, 0x8b1c/35612) of the bitfield"""
+        return einput(cls._addr_, output_int=True)
+    @classutilities.classproperty
+    def size(cls):
+        """return the number of bytes of the bitfield"""
+        return (sum([bit for field,bit in cls._fields_])-1)//8 + 1
+    @classutilities.classproperty
+    def name(cls):
+        return cls.__name__
     
+    @classmethod
+    def load(cls):
+        """read a bitfield from memory and return an instance of it"""
+        return cls().read()
+    @classmethod
+    def get(cls, field=None): 
+        """get a signle bit field, if field is None, get all data"""
+        bf = cls.load()
+        if field:
+            return getattr(bf, field)
+        else:
+            return bf.data
+    @classmethod
+    def set(cls, field=None, value=0):
+        """set a single bit field while keep others untouched, if field is None, set value as binary"""
+        if field:
+            bf = cls.load()
+            setattr(bf, field, value)
+        else:
+            bf = cls(value)
+        bf.write()
+    @classmethod
+    def show(cls):
+        """show current info of the bitfield in memory"""
+        print(cls.load())
+
     @property
     def data(self):
         return self._data
     @property
     def hex(self):
-        return hex(self.data)[2:]
+        return f"0x{self.data:0{self.size*2}x}"
     @property
     def bytes(self):
-        return self.data.to_bytes(self.size, self.__ENDIANESS)   
-    @classmethod
-    @property
-    def size(cls):
-        return (sum(cls._fields_.values())-1)//8 + 1
-    @classmethod
-    def get(cls, field): 
-        """get a signle bit field"""
-        bf = cls()
-        bf.read()
-        attr = getattr(bf, field, None)
-        if attr is None:
-            raise AttributeError(f"Bitfield '{cls.__name__}' has no field '{field}'")
-        return attr
-    @classmethod
-    def set(cls, field, value):
-        """set a single bit field while keep others untouched"""
-        bf = cls()
-        bf.read()
-        setattr(bf, field, value)
-        bf.write()
-    @classmethod
-    def from_bytes(cls, byte:bytes):
-        return cls(int.from_bytes(byte, cls.__ENDIANESS))
-    @classmethod
-    def from_np(cls, np_array:np.ndarray):
-        return cls.from_bytes(np_array.tobytes())
-    @classmethod
-    def show(cls, verbose=True):
-        bf = cls()
-        bf.read()
-        if verbose:
-            print(bf)
-        return bf.data
-
-    def to_np(self, dtype:np.dtype="u1"):
-        return np.frombuffer(self.bytes, dtype=dtype)
+        """convert self.data to bytes"""
+        return self.data.to_bytes(self.size, self.__ENDIANESS) 
 
     def read(self, verbose=False):
-        r = eread(self.addr, self.size) # read `self.size` bytes from memory at address `self.addr`
+        """read `self.size` bytes from memory to self.data at address `self.addr`"""
+        if _MEMMAP is not None:
+            r = np.zeros(self.size,dtype="u1")
+            for i in range(self.size):
+                r[i] = _MEMMAP.get(self.addr_+i,0)
+        else:
+            r = eread(self.addr, self.size) # read `self.size` bytes from memory at address `self.addr`
         if verbose:
             print(f"read {r} @ {self.addr}")
         self._data = int.from_bytes(r.tobytes(), self.__ENDIANESS)
+        return self
 
     def write(self, verbose=False):
+        """write `self.size` bytes of self.data to memory at address `self.addr`"""
         if verbose:
             print(f"write {self.hex} @ {self.addr}")
-        ewrite(self.addr, self.hex) # write `self.size` bytes to memory at address `self.addr`
+        if _MEMMAP is not None:
+            byte = np.frombuffer(self.data.to_bytes(self.size, self.__ENDIANESS),"u1")
+            for i in range(self.size):
+                _MEMMAP[self.addr_+i] = byte[i]
+        else:
+            ewrite(self.addr, self.hex) # write `self.size` bytes to memory at address `self.addr`
 
-    def diff(self, another:bitfield):
+    def diff(self, another:bitfield, verbose=False):
+        """diff two bitfields, return None if they are the same, otherwise return the diff string"""
         if isinstance(another, type(self)):
+            if self.data == another.data:
+                return None
             s = ""
             for this,that in zip(str(self).splitlines(), str(another).splitlines()):
                 this_value = this.split("=")[1]
                 that_value = that.split("=")[1]
                 if this_value == that_value:
-                    s += this+"\n"
+                    if verbose:
+                        s += this+"\n"
                 else:
                     s += this + " =>" + that_value + "\n"
             return s
         else:
-            raise TypeError(f'Try to diff "{another.__class__.__name__}" to "{self.__class__.__name__}"')
+            raise TypeError(f'Try to diff "{another.name}" to "{self.name}"')
+        
+    def jam(self):
+        """print 'jam val,addr' for each byte"""
+        data = np.frombuffer(self.bytes,"u1")
+        for i in range(self.size):
+            print(f"jam 0x{data[i]:02x},0x{self.addr_+i:x}")
+
 
-if __name__ == "__main__":
-    # following C bitfield struct `Example` has total 24 bits, which is 3 bytes
-    # GCC's `__attribute__((packed))` minimize memory usage, no padding between members
-    # ```c
-    # typedef struct
-    # {
-    # 	volatile unsigned short A	    :8;
-    # 	volatile unsigned short B	    :14;
-    # 	volatile unsigned short C	    :2;
-    # }__attribute__((packed)) Example;
-    # sizeof(Example) == 3
-    # ```
-
-    # but ctypes.Structure with `_pack_=1` works like `#pragma pack(1)` in MSVC, 
-    # align member at 1 byte boundary. not same as GCC's `__attribute__((packed))`
-    from ctypes import Structure, sizeof, c_ubyte, c_uint16
-    class Example_ctypes(Structure):
-        addr = '8000'
-        _pack_ = 1
-        _fields_ = [
-            ("A", c_uint16, 8),
-            ("B", c_uint16, 14),
-            ("C", c_uint16, 2),
-        ]
-    e = Example_ctypes()
-    e.A = 0x00
-    e.B = 0x3fff # set all 14 bit to 1
-    e.C = 0x3
-    print(bin(int.from_bytes(bytes(e),'little'))) 
-    # >>> 0b11001111111111111100000000 
-    #       CCPPBBBBBBBBBBBBBBAAAAAAAA  note 2 zero bit padded between B and C
-    print(sizeof(Example_ctypes)) # >>> 4, because of padding/alignment
-
-    # class `bitfield` mimic GCC's `__attribute__((packed))` behavior, no padding between members
-    # it use bit-wise mask/shift to manipulate bitfield, does not rely on any memory layout 
-    class Example_bitfield(bitfield):
-        addr = '8000' # address of reading/writing via memory
-        _fields_ = {
-            "A" : 8,
-            "B" : 14,
-            "C" : 2,
-        }
-    x = Example_bitfield()
-    x.A = 0x00
-    x.B = 0x3fff # set all 14 bit to 1
-    x.C = 0x3
-    print(bin(int.from_bytes(x.bytes,'little'))) 
-    # >>> 0b111111111111111100000000 
-    #       CCBBBBBBBBBBBBBBAAAAAAAA  note B is NOT padded, still 14 bit
-    print(x.size) # >>> 3, bitfield.size is calculated by sum all bitfield in cls._fields_
+def load_memmap(mem_map:dict={}):
+    global _MEMMAP
+    _MEMMAP = mem_map
```

## libzac/dsp.py

```diff
@@ -1,39 +1,79 @@
 import numpy as np
 from packaging import version
 
 def rolling_window(array:np.ndarray, window:int, step:int=1):
-    """ return rolling window matrix of input `array` with `step`, 
-        drop tails that not enough for one window. NOTE: THIS FUNCTION
-        RETURN A "VIEW" OF `array`, THEY POINT TO SAME OBJECT IN MEMORY!
-            Example:
-            >> rolling_window([0,1,2,3,4,5,6,7,8,9], 5, 2) =  
-            [[0, 1, 2, 3, 4],
-             [2, 3, 4, 5, 6],
-             [4, 5, 6, 7, 8]]
+    """
+    return rolling window matrix of input 1d `array` with `step`,
+    drop tails that not enough for one window. 
+        
+    NOTE: THIS FUNCTION RETURN A READ-ONLY "VIEW" OF `array`, THEY SHARE THE SAME MEMORY!
+    
+    Examples
+    --------
+    >>> x = np.arange(20)
+    >>> rolling_window(x,9,3)
+    array([[ 0,  1,  2,  3,  4,  5,  6,  7,  8],
+           [ 3,  4,  5,  6,  7,  8,  9, 10, 11],
+           [ 6,  7,  8,  9, 10, 11, 12, 13, 14],
+           [ 9, 10, 11, 12, 13, 14, 15, 16, 17]])
+    >>> # 18/19 is dropped
+    
+    >>> rolling_window(x,9,-3) 
+    array([[11, 12, 13, 14, 15, 16, 17, 18, 19],
+           [ 8,  9, 10, 11, 12, 13, 14, 15, 16],
+           [ 5,  6,  7,  8,  9, 10, 11, 12, 13],
+           [ 2,  3,  4,  5,  6,  7,  8,  9, 10]])
+    >>> # 0/1 is dropped
+
+    >>> rolling_window(x,9,-3).flags
+      C_CONTIGUOUS : False
+      F_CONTIGUOUS : False
+      OWNDATA : False
+      WRITEABLE : False
+      ALIGNED : True
+      WRITEBACKIFCOPY : False
+    <BLANKLINE>
     """
     if version.parse(np.version.version) < version.parse('1.20.0'):
         # before numpy 1.20.0
         shape = array.shape[:-1] + (array.shape[-1] - window + 1, window)
         strides = array.strides + (array.strides[-1],)
         return np.lib.stride_tricks.as_strided(array, shape=shape, strides=strides)[::step]
     else:
         # sliding_window_view() added after numpy 1.20.0
         return np.lib.stride_tricks.sliding_window_view(array, window)[::step]
 
-def sig2frames(array:np.ndarray, window:int, overlap:int=0, padding:bool=True):
-    """ similiar to `rolling_window()`, where `overlap = window - step`, 
-        and if `padding` is True, pad zeros to tails to fill up a window.
-        NOTE: THIS FUNCTION RETURN A "COPY" of `array`, THEY POINT TO DIFFERENT OBJECT"""
-    assert 0 <= overlap < window
-    step = window - overlap
-    slice_window = rolling_window(array, window, step).copy()
+def sig2frames(array:np.ndarray, window:int, step:int=0, **pad_kwarg):
+    """
+    same as `rolling_window()`, but padding zeros to tails to fill up a window.
+    Thus return a copy of `array` instead of a view. `**pad_kwarg` is passed to `np.pad()`.
+    
+    Examples
+    --------
+    >>> x = np.arange(20)
+    >>> sig2frames(x, 9, 3)
+    array([[ 0,  1,  2,  3,  4,  5,  6,  7,  8],
+           [ 3,  4,  5,  6,  7,  8,  9, 10, 11],
+           [ 6,  7,  8,  9, 10, 11, 12, 13, 14],
+           [ 9, 10, 11, 12, 13, 14, 15, 16, 17],
+           [12, 13, 14, 15, 16, 17, 18, 19,  0]])
+    >>> # note the last frame is padded with 0
+
+    >>> sig2frames(x, 9, -3) 
+    array([[11, 12, 13, 14, 15, 16, 17, 18, 19],
+           [ 8,  9, 10, 11, 12, 13, 14, 15, 16],
+           [ 5,  6,  7,  8,  9, 10, 11, 12, 13],
+           [ 2,  3,  4,  5,  6,  7,  8,  9, 10],
+           [ 0,  0,  1,  2,  3,  4,  5,  6,  7]])
+    >>> # when step is negative, pad to head
+    """
+    n_step = abs(step)
+    n_window = (array.size - window)//n_step + 1
+    if window+(n_window-1)*n_step < array.size:
+        pad_size = window + n_window*n_step - array.size
+        array = np.pad(array, (0, pad_size) if step>0 else (pad_size,0), **pad_kwarg)
+    return rolling_window(array, window, step)
 
-    # NOTE: if you do statistic on each window, result is inaccurate 
-    # for last window if there is padding because of the padding zeros.
-    #   if the array already ends with zeros, it may be difficult to 
-    # distinguish the newly appended zeros from the existing ones.
-    if padding: 
-        remain_data = array[slice_window.shape[0]*step:]
-        last_frame = np.pad(remain_data, (0, window-remain_data.size))
-        slice_window = np.vstack([slice_window, last_frame])
-    return slice_window
+if __name__ == '__main__':
+    import doctest
+    doctest.testmod()
```

## libzac/e.py

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 import os
 import re
 import numpy as np
 import matplotlib.pyplot as plt
-from .math import byte2int,i3u1_to_i4
+from .math import byte2int
 from subprocess import STDOUT, check_output, CalledProcessError
 
 from typing import TYPE_CHECKING
-if TYPE_CHECKING:  # Only imports the below statements during type checking
+if TYPE_CHECKING:  # Only imports the below statements during type checking, avoid circular import
     from .bitfield import bitfield
 
 def einput(num, output_int=False):
     """convert all kind of input to hex string(default) or integer"""
     if isinstance(num, str):
         return int(num,16) if output_int else num 
     elif isinstance(num, (int, np.integer)):
@@ -94,18 +94,22 @@
         ax.get_yaxis().set_major_formatter(lambda x, pos: int(x))
     fig.show()
 
 def e2write(input, skip_row=1):
     u1_data, addr = e2int(input, "u1", skip_row=skip_row)
     ewrite_block(addr[0], u1_data)
 
+###############################################
+#  wrapper of HREAD/HWRITE macro in yc11xx.h  #
+###############################################
+
 HREAD = HREAD2 = HREAD3 = HREAD_INLINE =        lambda reg: eread(reg)[0]
 HREADW =                                        lambda reg: eread(reg, length=2, dtype="u2")[0]
-HREAD24BIT = HREADADDR3 =                       lambda reg: i3u1_to_i4(eread(reg, length=3))[0]
-HREAD4 = HREADL = HREADRV =                     lambda reg: eread(reg, length=4, dtype="i4")[0]
+HREAD24BIT = HREADADDR3 =                       lambda reg: eread(reg, length=3, dtype="u3")[0]
+HREAD4 = HREADL = HREADRV =                     lambda reg: eread(reg, length=4, dtype="u4")[0]
 
 HWRITE = HWRITE2 = HWRITE3 = HWRITE_INLINE =    lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xff)
 HWRITEW = HWRITEW_INLINE =                      lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xffff)
 HWRITE24BIT =                                   lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xffffff) 
 HWRITEL = HWRITERV = HWRITE4 =                  lambda reg, value: ewrite(reg, einput(value,output_int=True) & 0xffffffff)
 
 def HREAD_STRUCT(reg, stc:bitfield):
```

## libzac/io.py

```diff
@@ -1,76 +1,91 @@
 import os
 import re
 import numpy as np
 np.set_printoptions(threshold=999999)
 
 def c2np(filename):
+    """
+    parse c array from file to numpy array
+    
+    WARNING: this function use `eval()` so not secure, do not use it on untrusted file
+    """
     with open(filename,'r') as f:
         raw = f.read()
     dtype_dict = {
-        'float':        np.float32,
-        'double':       np.float64,
-        'unsigned char':np.uint8,
-        'char':         np.int8,
-        'uint8_t':      np.uint8,
-        'int8_t':       np.int8,
-        'short':        np.int16,
-        'uint16_t':     np.uint16,
-        'int16_t':      np.int16,
-        'unsigned int': np.uint32,
-        'uint32_t':     np.uint32,
-        'int':          np.int32,
-        'int32_t':      np.int32,
+        'float':            np.float32,
+        'double':           np.float64,
+
+        'unsigned char':    np.uint8,
+        'uint8_t':          np.uint8,
+        'char':             np.int8,
+        'int8_t':           np.int8,
+
+        'unsigned short':   np.uint16,
+        'uint16_t':         np.uint16,
+        'short':            np.int16,
+        'int16_t':          np.int16,
+        
+        'unsigned int':     np.uint32,
+        'uint32_t':         np.uint32,
+        'int':              np.int32,
+        'int32_t':          np.int32,
     }
     regex = "((?:"+")|(?:".join(list(dtype_dict.keys()))+"))" + r"\s*(\w*)(\[.*\])\s*=\s*(\{[\s\S]*?\});"
     match = re.findall(regex, raw)
     array_dict = {}
     for group in match:
         dtype = dtype_dict[group[0]]
         array_name = group[1]
         data_str = group[3].replace("{","[").replace("}",']')   # change c array {} to python list []
         clean_str = re.sub("\/\/[\S\s]*?\\n", '', data_str)    # remove comment //
         clean_str = re.sub("\/\*[\S\s]*?\*\/",'', clean_str)   # remove comment /* */
         try:
             data = eval(clean_str) # this is not secure but i dont care
         except Exception as error:
-            print(f"parse {group[1]} error: ",error)
+            print(f"parse {array_name} error: ",error)
         array = np.array(data).astype(dtype)
         array_dict[array_name] = array
     return array_dict
 
-def np2c(np_dict_array, filename, addition=[], const=True, **kwarg_for_array2string):
-    with open(filename, "w") as f:
-        root, file = os.path.split(filename)
-        filename_no_ext, ext = os.path.splitext(file)
+def np2c(np_dict_array, filename, addition="", const=True, formatter={"float_kind":lambda f:f"{f:f}f"}, **kwargs):
+    """write numpy array to `<filename>.h` as c array format"""
+    filename = os.path.splitext(filename)[0]
+    filename_no_ext = os.path.split(filename)[1]
+    with open(filename+".h", "w") as f:
         const = "const " if const else "" 
-        f.write(f"#ifndef __{filename_no_ext}__\n#define __{filename_no_ext}__\n#include <stdint.h>\n\n")
-        
-        for line in addition:
-            f.write(line)
-            f.write("\n")
-        
+        f.write(f"#ifndef __{filename_no_ext}__\n#define __{filename_no_ext}__\n#include <stdint.h>\n\n")        
+        f.write(addition)        
         for array_name,array in np_dict_array.items():
             dtype = array.dtype
             if np.issubdtype(dtype, np.floating):
                 dtype_name = "float" if dtype.itemsize == 4 else "double"
             elif np.issubdtype(dtype, np.integer):
                 dtype_name = f"{np.dtype(dtype).base.name}_t"
+            else:
+                raise TypeError(f"unsupported dtype {dtype} for {array_name}")
             f.write(f"{const}{dtype_name} {array_name}[{array.size}] = {{\n ")
-            array_str = np.array2string(array, separator=",", **kwarg_for_array2string)[1:-1]
+            array_str = np.array2string(array, separator=",", formatter = formatter, **kwargs)[1:-1] # remove []
             f.write(array_str)
             f.write("\n};\n\n")
+        f.write(f"\n#endif /* __{filename_no_ext}__ */")           
 
-        f.write("\n#endif")           
-
-
-def file2c(filename_in, filename_out, array_name, dtype=np.uint8):
+def file2c(filename_in, filename_out, array_name, dtype=np.uint8, pad_tail=False, **kwargs):
+    """read file to byte array then to numpy array with dtype, kwargs pass to np2c"""
     with open(filename_in, "rb") as f:
         raw_byte = f.read()
-    byte2c(raw_byte, filename_out, array_name, dtype)
+    byte2c(raw_byte, filename_out, array_name, dtype, pad_tail, **kwargs)
 
-def byte2c(byte, filename, array_name="byte_buf", dtype=np.int8):
+def byte2c(byte, filename, array_name="byte_buf", dtype=np.uint8, pad_tail=False, **kwargs):
+    """convert byte array to numpy array with dtype then write to `<filename>.h` as c array format, kwargs pass to np2c"""
     dtype = np.dtype(dtype)
     size = dtype.itemsize
-    byte = byte[:len(byte)//size*size]
+    if len(byte)%size != 0:
+        print(f"WARNING: byte size {len(byte)} is not multiple of {size}, ", end="")
+        if pad_tail:
+            print(f"pad last {size-len(byte)%size} byte")
+            byte = byte + b'\x00'*(size-len(byte)%size)
+        else:
+            print(f"remove last {len(byte)%size} byte")
+            byte = byte[:len(byte)//size*size]
     array = np.frombuffer(byte, dtype=dtype)
-    np2c({array_name:array}, filename)
+    np2c({array_name:array}, filename, **kwargs)
```

## libzac/math.py

```diff
@@ -1,40 +1,106 @@
 import numpy as np
 
 def i4_to_i3u1(i4):
-    """unpack a int32 array, turn lower 3 bytes into a uint8 array (endianness matters)"""
+    """Unpack [u]int32 numpy array, turn lower 3 bytes into a uint8 array (endianness matters).
+
+    NOTE: By default it works on 24 bit data stored in 32 bit integers, simply drop the highest byte and no sign extend.
+    
+    Examples
+    --------
+    >>> i4 = np.array([0x01020304, 0x05060708], dtype=">u4") # big-endian
+    >>> i4_to_i3u1(i4)
+    array([2, 3, 4, 6, 7, 8], dtype=uint8)
+    >>> i4 = np.array([0x01020304, 0x05060708], dtype="<u4") # little-endian
+    >>> i4_to_i3u1(i4)
+    array([4, 3, 2, 8, 7, 6], dtype=uint8)
+    >>> i4 = np.array([0xf1020304, 0xf5060708], dtype="<u4") # negative value < -2**23 may give wrong result
+    >>> i4_to_i3u1(i4)
+    array([4, 3, 2, 8, 7, 6], dtype=uint8)
+    >>> i4 = np.random.randint(0, 2**24, 100, dtype="<u4")
+    >>> i3u1 = i4_to_i3u1(i4)
+    >>> np.allclose(i4,i3u1_to_i4(i3u1, "<", sign=False))
+    True
+    """
     offset = 1 if i4.dtype.byteorder == ">" else 0    
     return i4.view("u1").reshape(-1,4)[:, 0+offset:3+offset].ravel()
 
-def i3u1_to_i4(i3u1, endian="<"):
-    """pack every 3 items of a uint8 array as lower 3 bytes of int32 array (endianness matters)"""
-    i4 = np.zeros(i3u1.size//3, dtype="i4")
-    i4.view("u1").reshape(-1,4)[:,:3] = i3u1.reshape(-1,3)[:,::-1 if endian == ">" else 1]
-    return u2i(i4, 24)
+def i3u1_to_i4(u3u1, endian="<", sign=True):
+    """pack every 3 items of a uint8 array as lower 3 bytes of int32 array (endianness matters)
+    
+    Examples
+    --------
+    >>> i3u1 = np.array([2, 3, 4, 6, 7, 8], dtype="u1")
+    >>> i3u1_to_i4(i3u1,">",False) == np.array([0x020304, 0x060708], dtype=">u4")
+    array([ True,  True])
+    >>> i3u1 = np.array([4, 3, 2, 8, 7, 6], dtype="u1")
+    >>> i3u1_to_i4(i3u1,"<",False) == np.array([0x020304, 0x060708], dtype="<u4")
+    array([ True,  True])
+    >>> i3u1 = np.array([4, 3, 255, 8, 7, 255], dtype="u1")
+    >>> i3u1_to_i4(i3u1,"<",True) == np.array([0xffff0304, 0xffff0708], dtype="<u4").astype('i4')
+    array([ True,  True])
+    >>> i3u1 = np.random.randint(0, 2**8, 100*3, dtype="u1")
+    >>> i4 = i3u1_to_i4(i3u1, "<", sign=False)
+    >>> np.allclose(i3u1, i4_to_i3u1(i4))
+    True
+    """
+    i4 = np.zeros(u3u1.size//3, dtype="i4")
+    i4.view("u1").reshape(-1,4)[:,:3] = u3u1.reshape(-1,3)[:,::(-1 if endian == ">" else 1)]
+    return u2i(i4, 24) if sign else i4
 
 def u2i(x, width, overflow_warning=True):
+    """
+    Convert unsigned integer to signed integer (2's complement) with any bit width.
+
+    Examples
+    --------
+    >>> u2i(np.array([0x7f, 0x80, 0xff], dtype="u1"), 8)
+    array([ 127, -128,   -1], dtype=int8)
+    >>> u2i(np.arange(8,dtype="u1"), 3)
+    array([ 0,  1,  2,  3, -4, -3, -2, -1], dtype=int8)
+    >>> u = np.random.randint(0, 2**24, 100, dtype="u4")
+    >>> i = u2i(u, 24)
+    >>> np.allclose(u,i2u(i, 24))
+    True
+    """
     y = np.copy(x)
     overflow = (y >> width).astype(bool)
     if overflow_warning and overflow.any():
         print("Overflow")
     y[x >= (1<<(width-1))] -= (1<<width)
     y[overflow] = -1
     return y.astype(f"i{y.dtype.itemsize}")
 
 def i2u(x, width, overflow_warning=True):
+    """
+    Convert signed integer (2's complement) to unsigned integer with any bit width.
+    
+    Examples
+    --------
+    >>> i2u(np.array([127, -128, -1], dtype="i1"), 8)
+    array([127, 128, 255], dtype=uint8)
+    >>> i2u(np.arange(-4,4,dtype="i1"), 3)
+    array([4, 5, 6, 7, 0, 1, 2, 3], dtype=uint8)
+    >>> u = np.random.randint(0, 2**24, 100, dtype="u4")
+    >>> i = u2i(u, 24)
+    >>> np.allclose(u,i2u(i, 24))
+    True
+    """
     y = np.copy(x)
     upper = y >  (1<<(width-1))-1
     lower = y < -(1<<(width-1))
     if overflow_warning and (upper.any() or lower.any()):
         print("Overflow")
     y[upper] =   (1<<(width-1))-1
     y[lower] =  -(1<<(width-1))
     y[y < 0] +=  (1<<(width))
     return y.astype(f"u{y.dtype.itemsize}")
     
 def byte2int(byte, dtype="<i4"):
+    """Mainly for converting byte string to 24 bit("i3") numpy array, 
+    for common dtypes(8/16/32/64) just call np.frombuffer."""
     if isinstance(dtype, str) and dtype[-1]=='3':
-        i3u1 = np.frombuffer(byte,"u1").copy()
+        u3u1 = np.frombuffer(byte,"u1").copy()
         endianness = ">" if dtype[0]==">" else "<"
-        return i3u1_to_i4(i3u1, endianness)
+        return i3u1_to_i4(u3u1, endianness, dtype[-2]=='i')
     else:
         return np.frombuffer(byte,dtype=dtype).copy()
```

## libzac/reg.py

```diff
@@ -9,75 +9,19 @@
 from .e import e2int,eread,einput
 from typing import Union
 
 if xlrd.__version__ < "2.0.0":
     xlrd.xlsx.ensure_elementtree_imported(False, None)
     xlrd.xlsx.Element_has_iter = True
 
-
 autoREG = """
 e 8000lc29  > bb.txt
 e 8900laa   > modem.txt
 e 8a00la4   > rf.txt
 e 8b00l1c   > codec.txt
-
-e 8336l16   > lpm.txt
-
-e 801c 0
-e 83a1l4    > "LDO Control.txt"
-
-e 801c 1
-e 8380l4    > "CHARGER CTRL.txt"
-
-e 801c 2
-e 8380l4    > "XO32K CONTROL.txt"
-
-e 801c 4
-e 8380l4    > CHARGER_WAKE_CTRL.txt
-
-e 81f2 1
-e 8389l4    > TS_ANA_CTRL.txt
-e 81f2 0
-e 81f2 2
-e 8389l4    > TS_FIR_CTRL.txt
-e 81f2 0
-e 81f2 4
-e 8389l4    > TS_CAL_CTRL1.txt
-e 81f2 0
-e 81f2 8
-e 8389l4    > TS_CAL_CTRL2.txt
-e 81f2 0
-e 81f2 10
-e 8389l4    > TS_CAL_CTRL3.txt
-e 81f2 0
-e 81f2 20
-e 8389l4    > TS_CAL_CTRL4.txt
-e 81f2 0
-e 81f2 40
-e 8389l4    > TS_CMP_CTRL1.txt
-e 81f2 0
-e 81f2 80
-e 8389l4    > TS_CMP_CTRL2.txt
-e 81f2 0
-
-e 81f3 1
-e 8389l4    > TS_CAL_CFG.txt
-e 81f3 0
-e 81f3 2
-e 8389l4    > TS_BL_CTRL1.txt
-e 81f3 0
-e 81f3 4
-e 8389l4    > TS_BL_CTRL2.txt
-e 81f3 0
-e 81f3 8
-e 8389l4    > TS_BL_CTRL3.txt
-e 81f3 0
-e 81f3 10
-e 8389l4    > TS_BL_CTRL4.txt
-e 81f3 0
 """
 addr_name = "addr"
 reg_name = "name"
 width_name = "width"
 domain_name = "domain"
 access_name = "access"
 init_name = "init"
@@ -162,70 +106,72 @@
     wb = openpyxl.load_workbook(filename)
     tables = {sheet_name:read_yc_reg(wb, sheet_name) for sheet_name in wb.sheetnames if sheet_name != 'lpm'}
     return tables
 
 def keep_only_rows(table:pd.DataFrame, keep_list:list, col:str = addr_name) -> pd.DataFrame:
     return table.loc[table[col].isin(keep_list)]
 
-def efile_to_hashmap(filename:str) -> dict:
+def table2tree(table:pd.DataFrame, key:str) -> dict:
+    """convert pandas Dataframe to tree like dict, use either `addr_name` or `reg_name` as `key`"""
+    tree = {}
+    old_key = ""
+    for i in table.to_dict("records"):
+        if tree.get(i[key],False):
+            if i[key] != old_key:
+                raise ValueError(f"multiple '{i[key]}'")
+            tree[i[key]].append(i)
+        else:
+            tree[i[key]] = [i]
+        old_key = i[key]
+    return tree
+
+
+"""manipulate data
+mem_map = {0x8b00 : 0x20, ...}
+reg_map = {CODEC_LDO_EN0RegDef : 0x20, ...}
+addr_map = {0x8b00: CODEC_LDO_EN0RegDef, ...}
+"""
+
+def efile_to_mem_map(filename:str) -> dict:
     """convert an `e [addr]l[size]` output file to dict where key is addr and value is data"""
-    return {f"{a:x}":d for d,a in zip(*e2int(filename,"u1"))}
+    return {addr:data for data,addr in zip(*e2int(filename,"u1"))}
 
 def parse_width(width:Union[str,int]) -> tuple[int,int]:
     """parse_width('[x]/x') = (x,x);  parse_width('[x:y]/x:y') = (x,y)"""
     if isinstance(width, (np.integer, int)):
         return width, width
-    if (not width) or (width == "nan"):
+    if (not width) or (width == "nan") or not isinstance(width, str):
         raise ValueError(f"parse_width() failed: {type(width)}:{width}")
     width = width.replace("[","").replace("]","").replace(" ","").split(":")
     return (int(width[1]), int(width[0])) if len(width)==2 else (int(width[0]), int(width[0]))
 
-def parse_reg(addr:str, reg_map:dict, start:int, stop:int) -> str:
-    """Get bits between `start` and `stop` from start address `addr` in `reg_map`.
-    if total bits > 64, return `too large`, if cannot find `addr` in `reg_map` return `nan`, otherwise return string of data in hex"""
+def parse_reg(addr:int, mem_map:dict, start:int, stop:int) -> str:
+    """Get bits between `start` and `stop` from start address `addr` in `mem_map`.
+    if total bits > 64, return `too large`, if cannot find `addr` in `mem_map` return `nan`, otherwise return string of data in hex"""
     bits = stop-start+1
     if bits > 64:
         return "too large"    
-    if reg_map.get(addr,-1) >= 0:
+    if mem_map.get(addr,-1) >= 0:
         num = 0
         for i in range(stop//8+1):
-            num |= reg_map[f"{int(addr,16)+i:x}"]<<(i*8)
+            num |= mem_map[addr+i]<<(i*8)
         num = (num >> start) & ((1<<bits)-1)
         return f"{num:0{((bits-1)//8+1)*2}x}"
     else:
         return "nan"
     
-def parse_table(table:pd.DataFrame, reg_map:dict, new_column:str) -> None:        
+def parse_table(table:pd.DataFrame, mem_map:dict, new_column:str) -> None:        
     """add new column named `new_column` to `table`, apply `parse_reg` to each row"""
     table.loc[:,new_column] = np.zeros(len(table),str)
     for i in table.index:    
         try:
             start, stop = parse_width(table.loc[i,width_name])
             if start >= 0 and not pd.isna(table.loc[i,addr_name]):            
                 addr = re.search(r"[\da-f]{4,}",table.loc[i,addr_name])
                 if addr is not None:     
-                    table.loc[i,new_column] = parse_reg(addr.group(), reg_map, start, stop)
+                    table.loc[i,new_column] = parse_reg(int(addr.group(),16), mem_map, start, stop)
         except Exception as e:
             print(f"Unable to parse table line {i}: \n{table.loc[i]}\n")
             raise e
 
-def table2tree(table:pd.DataFrame, key:str) -> dict:
-    """convert pandas Dataframe to tree like dict, use either `addr_name` or `reg_name` as `key`"""
-    tree = {}
-    old_key = ""
-    for i in table.to_dict("records"):
-        if tree.get(i[key],False):
-            if i[key] != old_key:
-                raise ValueError(f"multiple '{i[key]}'")
-            tree[i[key]].append(i)
-        else:
-            tree[i[key]] = [i]
-        old_key = i[key]
-    return tree
-
-def load_reg_1121M(MODULE_PATH = "E:\\Work\\Yichip\\1121M\\Soft_Doc\\xlsxtoStructTool\\reg"):    
-    spec = importlib.util.spec_from_file_location(os.path.split(MODULE_PATH)[1], MODULE_PATH+"/__init__.py")
-    module = importlib.util.module_from_spec(spec)
-    sys.modules[spec.name] = module 
-    spec.loader.exec_module(module)
-    setattr(sys.modules[__name__],"reg_1121M",module)
-    return module
+def load_reg_1121M(MODULE_PATH = "E:\\Work\\Yichip\\1121M\\Soft_Doc\\xlsxtoStructTool\\reg_1121M"):    
+    sys.path.append(MODULE_PATH)
```

## Comparing `libzac-0.0.9.dist-info/LICENSE` & `libzac-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libzac-0.0.9.dist-info/METADATA` & `libzac-0.1.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libzac
-Version: 0.0.9
+Version: 0.1.0
 Summary: A private use library
 Author-email: ZinGer_KyoN <zinger.kyon@gmail.com>
 License: MIT License        
         Copyright (c) 2022 YiChip Inc.        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

