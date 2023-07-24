# Comparing `tmp/pyfant-19.12.5.0.tar.gz` & `tmp/pyfant-23.7.24.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyfant-19.12.5.0.tar", last modified: Thu Dec  5 16:30:25 2019, max compression
+gzip compressed data, was "pyfant-23.7.24.0.tar", last modified: Mon Jul 24 12:44:06 2023, max compression
```

## Comparing `pyfant-19.12.5.0.tar` & `pyfant-23.7.24.0.tar`

### file list

```diff
@@ -1,152 +1,164 @@
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/
--rw-r--r--   0 j         (1000) j         (1000)       34 2018-03-02 13:15:17.000000 pyfant-19.12.5.0/MANIFEST.in
--rw-r--r--   0 j         (1000) j         (1000)      445 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)      150 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/README.md
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/
--rw-r--r--   0 j         (1000) j         (1000)     1199 2019-12-02 20:14:14.000000 pyfant-19.12.5.0/pyfant/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     1143 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/_star.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/basic/
--rw-r--r--   0 j         (1000) j         (1000)      396 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/basic/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)      774 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/basic/constants.py
--rw-r--r--   0 j         (1000) j         (1000)    11564 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/basic/conversion.py
--rw-r--r--   0 j         (1000) j         (1000)      215 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/basic/errors.py
--rw-r--r--   0 j         (1000) j         (1000)      738 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/basic/misc.py
--rw-r--r--   0 j         (1000) j         (1000)     2546 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/basic/paths.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/convmol/
--rw-r--r--   0 j         (1000) j         (1000)      218 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     1564 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/calc_qgbd.py
--rw-r--r--   0 j         (1000) j         (1000)     3877 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/conv.py
--rw-r--r--   0 j         (1000) j         (1000)     6387 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/conv_hitran.py
--rw-r--r--   0 j         (1000) j         (1000)     5470 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/conv_kurucz.py
--rw-r--r--   0 j         (1000) j         (1000)     3225 2019-12-03 19:04:00.000000 pyfant-19.12.5.0/pyfant/convmol/conv_plez.py
--rw-r--r--   0 j         (1000) j         (1000)     3327 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/conv_vald3.py
--rw-r--r--   0 j         (1000) j         (1000)      794 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/convmol/convlog.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/data/
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/data/default/
--rw-r--r--   0 j         (1000) j         (1000)     1163 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/abonds.dat
--rw-r--r--   0 j         (1000) j         (1000)     2551 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/absoru2.dat
--rw-r--r--   0 j         (1000) j         (1000)      618 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/abxfwhm.py
--rw-r--r--   0 j         (1000) j         (1000)      362 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/configconvmol.py
--rw-r--r--   0 j         (1000) j         (1000)     1353 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/configmolconsts.py
--rw-r--r--   0 j         (1000) j         (1000)     3628 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/dissoc.dat
--rw-r--r--   0 j         (1000) j         (1000)    14336 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/hitrandb.sqlite
--rw-r--r--   0 j         (1000) j         (1000)      381 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/hmap.dat
--rw-r--r--   0 j         (1000) j         (1000)       89 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/main.dat
--rw-r--r--   0 j         (1000) j         (1000)     2400 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/modeles.mod
--rw-r--r--   0 j         (1000) j         (1000)    77824 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/moldb.sqlite
--rw-r--r--   0 j         (1000) j         (1000)    53356 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/data/default/partit.dat
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/downloaders/
--rw-r--r--   0 j         (1000) j         (1000)      783 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/downloaders/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     5083 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/downloaders/downhitran.py
--rw-r--r--   0 j         (1000) j         (1000)     7550 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/downloaders/downnist.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/filetypes/
--rw-r--r--   0 j         (1000) j         (1000)      585 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/filetypes/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     7533 2018-06-21 13:06:07.000000 pyfant-19.12.5.0/pyfant/filetypes/fileabonds.py
--rw-r--r--   0 j         (1000) j         (1000)      494 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/fileabsoru2.py
--rw-r--r--   0 j         (1000) j         (1000)     5690 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/fileabxfwhm.py
--rw-r--r--   0 j         (1000) j         (1000)     9301 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/fileatoms.py
--rw-r--r--   0 j         (1000) j         (1000)      348 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/fileconfconvmol.py
--rw-r--r--   0 j         (1000) j         (1000)     4346 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filedissoc.py
--rw-r--r--   0 j         (1000) j         (1000)     3964 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filehitrandb.py
--rw-r--r--   0 j         (1000) j         (1000)     2360 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/filetypes/filehmap.py
--rw-r--r--   0 j         (1000) j         (1000)    16251 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filekuruczmol.py
--rw-r--r--   0 j         (1000) j         (1000)     4058 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filemain.py
--rw-r--r--   0 j         (1000) j         (1000)    17453 2018-03-01 14:43:37.000000 pyfant-19.12.5.0/pyfant/filetypes/filemod.py
--rw-r--r--   0 j         (1000) j         (1000)     1101 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/filetypes/filemolconsts.py
--rw-r--r--   0 j         (1000) j         (1000)    14203 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/filetypes/filemoldb.py
--rw-r--r--   0 j         (1000) j         (1000)    18303 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/filetypes/filemolecules.py
--rw-r--r--   0 j         (1000) j         (1000)     4350 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/fileoptions.py
--rw-r--r--   0 j         (1000) j         (1000)      518 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filepartit.py
--rw-r--r--   0 j         (1000) j         (1000)     9594 2019-12-04 14:18:21.000000 pyfant-19.12.5.0/pyfant/filetypes/fileplezlinelist.py
--rw-r--r--   0 j         (1000) j         (1000)    10212 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filepleztio.py
--rw-r--r--   0 j         (1000) j         (1000)     3085 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filetoh.py
--rw-r--r--   0 j         (1000) j         (1000)    17088 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filetraprb.py
--rw-r--r--   0 j         (1000) j         (1000)    10714 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/filevald3.py
--rw-r--r--   0 j         (1000) j         (1000)     9913 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/filetypes/morespectra.py
--rw-r--r--   0 j         (1000) j         (1000)     5793 2019-12-02 20:29:27.000000 pyfant-19.12.5.0/pyfant/from_turbospectrum.py
--rw-r--r--   0 j         (1000) j         (1000)     6563 2019-12-02 20:20:47.000000 pyfant-19.12.5.0/pyfant/from_vald.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/gui/
--rw-r--r--   0 j         (1000) j         (1000)     1728 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)     3086 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/_shared.py
--rw-r--r--   0 j         (1000) j         (1000)    13175 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WContinua.py
--rw-r--r--   0 j         (1000) j         (1000)     5037 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WContinuum.py
--rw-r--r--   0 j         (1000) j         (1000)     7851 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WDBFCF.py
--rw-r--r--   0 j         (1000) j         (1000)     5134 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WDBMolecule.py
--rw-r--r--   0 j         (1000) j         (1000)     4856 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WDBPFANTMol.py
--rw-r--r--   0 j         (1000) j         (1000)     6533 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WDBState.py
--rw-r--r--   0 j         (1000) j         (1000)     4791 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WDBSystem.py
--rw-r--r--   0 j         (1000) j         (1000)     2927 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WDBSystemPfantmolFCF.py
--rw-r--r--   0 j         (1000) j         (1000)     7412 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WFileAbXFwhm.py
--rw-r--r--   0 j         (1000) j         (1000)    11906 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WFileAbonds.py
--rw-r--r--   0 j         (1000) j         (1000)    14369 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WFileMain.py
--rw-r--r--   0 j         (1000) j         (1000)     3832 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/gui/a_WFileMolConsts.py
--rw-r--r--   0 j         (1000) j         (1000)     2312 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_WFileMolDB.py
--rw-r--r--   0 j         (1000) j         (1000)    36569 2019-12-05 10:50:29.000000 pyfant-19.12.5.0/pyfant/gui/a_WMolecularConstants.py
--rw-r--r--   0 j         (1000) j         (1000)    33331 2018-03-02 13:15:17.000000 pyfant-19.12.5.0/pyfant/gui/a_WOptionsEditor.py
--rw-r--r--   0 j         (1000) j         (1000)     3059 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XAtomLinesEditor.py
--rw-r--r--   0 j         (1000) j         (1000)    36371 2019-12-05 10:49:27.000000 pyfant-19.12.5.0/pyfant/gui/a_XConvMol.py
--rw-r--r--   0 j         (1000) j         (1000)     5551 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileAbonds.py
--rw-r--r--   0 j         (1000) j         (1000)    15676 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileAtoms.py
--rw-r--r--   0 j         (1000) j         (1000)     3212 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileAtomsHistogram.py
--rw-r--r--   0 j         (1000) j         (1000)     3826 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileMain.py
--rw-r--r--   0 j         (1000) j         (1000)     1874 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileMolConsts.py
--rw-r--r--   0 j         (1000) j         (1000)     1023 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileMolDB.py
--rw-r--r--   0 j         (1000) j         (1000)    22971 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileMolecules.py
--rw-r--r--   0 j         (1000) j         (1000)      936 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XFileOptions.py
--rw-r--r--   0 j         (1000) j         (1000)    15149 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XMainAbonds.py
--rw-r--r--   0 j         (1000) j         (1000)     3049 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XMolLinesEditor.py
--rw-r--r--   0 j         (1000) j         (1000)     7504 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XMulti.py
--rw-r--r--   0 j         (1000) j         (1000)     4805 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XPFANT.py
--rw-r--r--   0 j         (1000) j         (1000)    14232 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/gui/a_XRunnableManager.py
--rw-r--r--   0 j         (1000) j         (1000)    38170 2019-12-05 12:17:20.000000 pyfant-19.12.5.0/pyfant/kovacs.py
--rw-r--r--   0 j         (1000) j         (1000)    11679 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/molconsts.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/run/
--rw-r--r--   0 j         (1000) j         (1000)      118 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/run/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)    17714 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/run/conf.py
--rw-r--r--   0 j         (1000) j         (1000)     9047 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/run/multirunnable.py
--rw-r--r--   0 j         (1000) j         (1000)    16962 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/run/rm.py
--rw-r--r--   0 j         (1000) j         (1000)    17806 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/run/runnables.py
--rw-r--r--   0 j         (1000) j         (1000)     3725 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/run/traprbclass.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/scripts/
--rwxr-xr-x   0 j         (1000) j         (1000)     2363 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/_copy-from-sessions.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1633 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/_diff-molecules.py
--rwxr-xr-x   0 j         (1000) j         (1000)     4311 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/_plot-innewmarcs-result.py
--rwxr-xr-x   0 j         (1000) j         (1000)      563 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/_recreate-hitrandb.py
--rwxr-xr-x   0 j         (1000) j         (1000)     2216 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/_save-pdf.py
--rwxr-xr-x   0 j         (1000) j         (1000)      625 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/abed.py
--rwxr-xr-x   0 j         (1000) j         (1000)      667 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/ated.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1104 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/convmol.py
--rwxr-xr-x   0 j         (1000) j         (1000)     2791 2018-03-01 13:45:00.000000 pyfant-19.12.5.0/pyfant/scripts/copy-star.py
--rwxr-xr-x   0 j         (1000) j         (1000)     3669 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/create-grid.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1286 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/cut-atoms.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1267 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/cut-molecules.py
--rwxr-xr-x   0 j         (1000) j         (1000)     6811 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/hitran-scraper.py
--rwxr-xr-x   0 j         (1000) j         (1000)     3173 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/link.py
--rwxr-xr-x   0 j         (1000) j         (1000)      636 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/mained.py
--rwxr-xr-x   0 j         (1000) j         (1000)      943 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/mced.py
--rw-r--r--   0 j         (1000) j         (1000)     2197 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/merge-molecules.py
--rwxr-xr-x   0 j         (1000) j         (1000)      703 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/mled.py
--rwxr-xr-x   0 j         (1000) j         (1000)      912 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/moldbed.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1848 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/nist-scraper.py
--rwxr-xr-x   0 j         (1000) j         (1000)     3879 2018-06-19 12:56:24.000000 pyfant-19.12.5.0/pyfant/scripts/nulbad.py
--rwxr-xr-x   0 j         (1000) j         (1000)      849 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/optionsed.py
--rwxr-xr-x   0 j         (1000) j         (1000)     2113 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/run-multi.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1152 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/run4.py
--rwxr-xr-x   0 j         (1000) j         (1000)    10219 2019-12-04 12:43:29.000000 pyfant-19.12.5.0/pyfant/scripts/tune-zinf.py
--rwxr-xr-x   0 j         (1000) j         (1000)     2762 2019-12-02 20:14:14.000000 pyfant-19.12.5.0/pyfant/scripts/turbospectrum-to-atoms.py
--rwxr-xr-x   0 j         (1000) j         (1000)     2770 2019-12-04 13:34:22.000000 pyfant-19.12.5.0/pyfant/scripts/vald3-to-atoms.py
--rwxr-xr-x   0 j         (1000) j         (1000)     1101 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/scripts/x.py
--rw-r--r--   0 j         (1000) j         (1000)    15663 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/util.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant/vis/
--rw-r--r--   0 j         (1000) j         (1000)       67 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/vis/__init__.py
--rw-r--r--   0 j         (1000) j         (1000)      723 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/vis/modgrid.py
--rw-r--r--   0 j         (1000) j         (1000)     3073 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/vis/vismany.py
--rw-r--r--   0 j         (1000) j         (1000)     8273 2018-01-04 23:34:13.000000 pyfant-19.12.5.0/pyfant/vis/vismod.py
-drwxr-xr-x   0 j         (1000) j         (1000)        0 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/pyfant.egg-info/
--rw-r--r--   0 j         (1000) j         (1000)      445 2019-12-05 16:30:23.000000 pyfant-19.12.5.0/pyfant.egg-info/PKG-INFO
--rw-r--r--   0 j         (1000) j         (1000)     3834 2019-12-05 16:30:24.000000 pyfant-19.12.5.0/pyfant.egg-info/SOURCES.txt
--rw-r--r--   0 j         (1000) j         (1000)        1 2019-12-05 16:30:23.000000 pyfant-19.12.5.0/pyfant.egg-info/dependency_links.txt
--rw-r--r--   0 j         (1000) j         (1000)      134 2019-12-05 16:30:23.000000 pyfant-19.12.5.0/pyfant.egg-info/requires.txt
--rw-r--r--   0 j         (1000) j         (1000)        7 2019-12-05 16:30:23.000000 pyfant-19.12.5.0/pyfant.egg-info/top_level.txt
--rw-r--r--   0 j         (1000) j         (1000)       38 2019-12-05 16:30:25.000000 pyfant-19.12.5.0/setup.cfg
--rw-r--r--   0 j         (1000) j         (1000)     1584 2019-12-05 16:23:43.000000 pyfant-19.12.5.0/setup.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.955988 pyfant-23.7.24.0/
+-rw-rw-r--   0 j         (1000) j         (1000)       34 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/MANIFEST.in
+-rw-rw-r--   0 j         (1000) j         (1000)      445 2023-07-24 12:44:06.955988 pyfant-23.7.24.0/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)      150 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/README.md
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.927989 pyfant-23.7.24.0/pyfant/
+-rw-rw-r--   0 j         (1000) j         (1000)     1219 2023-04-12 12:29:24.000000 pyfant-23.7.24.0/pyfant/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1143 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/_star.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.931989 pyfant-23.7.24.0/pyfant/basic/
+-rw-rw-r--   0 j         (1000) j         (1000)      396 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/basic/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      774 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/basic/constants.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13639 2023-06-26 13:29:43.000000 pyfant-23.7.24.0/pyfant/basic/conversion.py
+-rw-rw-r--   0 j         (1000) j         (1000)      215 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/basic/errors.py
+-rw-rw-r--   0 j         (1000) j         (1000)      738 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/basic/misc.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2546 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/basic/paths.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.931989 pyfant-23.7.24.0/pyfant/convmol/
+-rw-rw-r--   0 j         (1000) j         (1000)      281 2023-07-06 13:43:21.000000 pyfant-23.7.24.0/pyfant/convmol/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1686 2023-07-16 17:00:47.000000 pyfant-23.7.24.0/pyfant/convmol/calc_qgbd.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9987 2023-07-20 00:08:36.000000 pyfant-23.7.24.0/pyfant/convmol/conv.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14275 2023-07-17 22:57:21.000000 pyfant-23.7.24.0/pyfant/convmol/conv_brooke2014.py
+-rw-rw-r--   0 j         (1000) j         (1000)    16432 2023-07-06 14:14:16.000000 pyfant-23.7.24.0/pyfant/convmol/conv_hitran.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5402 2023-07-20 00:10:14.000000 pyfant-23.7.24.0/pyfant/convmol/conv_hitran160.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3694 2023-07-17 22:26:03.000000 pyfant-23.7.24.0/pyfant/convmol/conv_kurucz.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3602 2023-07-19 15:25:23.000000 pyfant-23.7.24.0/pyfant/convmol/conv_plez.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3328 2023-07-16 17:10:12.000000 pyfant-23.7.24.0/pyfant/convmol/conv_vald3.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1585 2023-05-31 22:53:51.000000 pyfant-23.7.24.0/pyfant/convmol/convlog.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.927989 pyfant-23.7.24.0/pyfant/data/
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.935989 pyfant-23.7.24.0/pyfant/data/default/
+-rw-rw-r--   0 j         (1000) j         (1000)     1163 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/abonds.dat
+-rw-rw-r--   0 j         (1000) j         (1000)     2551 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/absoru2.dat
+-rw-rw-r--   0 j         (1000) j         (1000)      618 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/abxfwhm.py
+-rw-rw-r--   0 j         (1000) j         (1000)      362 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/configconvmol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1353 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/configmolconsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3628 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/dissoc.dat
+-rw-rw-r--   0 j         (1000) j         (1000)    14336 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/hitrandb.sqlite
+-rw-rw-r--   0 j         (1000) j         (1000)      381 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/hmap.dat
+-rw-rw-r--   0 j         (1000) j         (1000)       89 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/main.dat
+-rw-rw-r--   0 j         (1000) j         (1000)     2400 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/modeles.mod
+-rw-rw-r--   0 j         (1000) j         (1000)    77824 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/moldb.sqlite
+-rw-rw-r--   0 j         (1000) j         (1000)    53356 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/data/default/partit.dat
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.935989 pyfant-23.7.24.0/pyfant/downloaders/
+-rw-rw-r--   0 j         (1000) j         (1000)      783 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/downloaders/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5083 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/downloaders/downhitran.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7550 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/downloaders/downnist.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.943988 pyfant-23.7.24.0/pyfant/filetypes/
+-rw-rw-r--   0 j         (1000) j         (1000)      699 2023-07-07 12:46:52.000000 pyfant-23.7.24.0/pyfant/filetypes/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7533 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/fileabonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)      494 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/fileabsoru2.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5690 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/fileabxfwhm.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9301 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/fileatoms.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6927 2023-07-07 17:39:02.000000 pyfant-23.7.24.0/pyfant/filetypes/filebrooke2014.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2220 2023-07-07 13:05:52.000000 pyfant-23.7.24.0/pyfant/filetypes/filecojm1998.py
+-rw-rw-r--   0 j         (1000) j         (1000)      348 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/fileconfconvmol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4346 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filedissoc.py
+-rw-rw-r--   0 j         (1000) j         (1000)    11105 2023-07-06 18:09:36.000000 pyfant-23.7.24.0/pyfant/filetypes/filehitran160.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3964 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filehitrandb.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2360 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filehmap.py
+-rw-rw-r--   0 j         (1000) j         (1000)    17698 2023-07-20 22:56:54.000000 pyfant-23.7.24.0/pyfant/filetypes/filekuruczmol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4058 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filemain.py
+-rw-rw-r--   0 j         (1000) j         (1000)    17453 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filemod.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1101 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filemolconsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14451 2023-05-28 11:43:17.000000 pyfant-23.7.24.0/pyfant/filetypes/filemoldb.py
+-rw-rw-r--   0 j         (1000) j         (1000)    18441 2023-07-05 21:06:29.000000 pyfant-23.7.24.0/pyfant/filetypes/filemolecules.py
+-rw-rw-r--   0 j         (1000) j         (1000)      980 2023-07-05 21:06:29.000000 pyfant-23.7.24.0/pyfant/filetypes/filemollist.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4381 2023-04-14 20:41:53.000000 pyfant-23.7.24.0/pyfant/filetypes/fileoptions.py
+-rw-rw-r--   0 j         (1000) j         (1000)      518 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filepartit.py
+-rw-rw-r--   0 j         (1000) j         (1000)    16754 2023-06-30 20:15:22.000000 pyfant-23.7.24.0/pyfant/filetypes/fileplezlinelist.py
+-rw-rw-r--   0 j         (1000) j         (1000)    10212 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filepleztio.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3085 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filetoh.py
+-rw-rw-r--   0 j         (1000) j         (1000)    17088 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filetraprb.py
+-rw-rw-r--   0 j         (1000) j         (1000)    10714 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/filevald3.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9913 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/filetypes/morespectra.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5793 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/from_turbospectrum.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6563 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/from_vald.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.947988 pyfant-23.7.24.0/pyfant/gui/
+-rw-rw-r--   0 j         (1000) j         (1000)     1768 2023-04-12 13:57:59.000000 pyfant-23.7.24.0/pyfant/gui/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3086 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/_shared.py
+-rw-rw-r--   0 j         (1000) j         (1000)    13175 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WContinua.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5037 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WContinuum.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7851 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WDBFCF.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5134 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WDBMolecule.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4856 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WDBPFANTMol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     6533 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WDBState.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4791 2023-05-27 11:10:12.000000 pyfant-23.7.24.0/pyfant/gui/a_WDBSystem.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3789 2023-05-28 11:36:39.000000 pyfant-23.7.24.0/pyfant/gui/a_WDBSystemPfantmolFCF.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7412 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WFileAbXFwhm.py
+-rw-rw-r--   0 j         (1000) j         (1000)    11906 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WFileAbonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14369 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WFileMain.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3832 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WFileMolConsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2312 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WFileMolDB.py
+-rw-rw-r--   0 j         (1000) j         (1000)    36626 2023-07-16 17:46:29.000000 pyfant-23.7.24.0/pyfant/gui/a_WMolecularConstants.py
+-rw-rw-r--   0 j         (1000) j         (1000)    33331 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_WOptionsEditor.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3059 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XAtomLinesEditor.py
+-rw-rw-r--   0 j         (1000) j         (1000)    36371 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XConvMol.py
+-rw-rw-r--   0 j         (1000) j         (1000)     5551 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileAbonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15676 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileAtoms.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3212 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileAtomsHistogram.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3826 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileMain.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1874 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileMolConsts.py
+-rw-rw-r--   0 j         (1000) j         (1000)     1023 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileMolDB.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3544 2023-04-12 14:29:20.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileMoleculeHistogram.py
+-rw-rw-r--   0 j         (1000) j         (1000)    25430 2023-05-05 17:13:54.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileMolecules.py
+-rw-rw-r--   0 j         (1000) j         (1000)      936 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XFileOptions.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15149 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XMainAbonds.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3049 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XMolLinesEditor.py
+-rw-rw-r--   0 j         (1000) j         (1000)     7504 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XMulti.py
+-rw-rw-r--   0 j         (1000) j         (1000)     4805 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XPFANT.py
+-rw-rw-r--   0 j         (1000) j         (1000)    14232 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/gui/a_XRunnableManager.py
+-rw-rw-r--   0 j         (1000) j         (1000)    38318 2023-04-15 22:19:35.000000 pyfant-23.7.24.0/pyfant/kovacs.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.947988 pyfant-23.7.24.0/pyfant/misc/
+-rw-rw-r--   0 j         (1000) j         (1000)       27 2023-04-12 12:38:10.000000 pyfant-23.7.24.0/pyfant/misc/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      752 2023-04-12 18:08:57.000000 pyfant-23.7.24.0/pyfant/misc/molhistogram.py
+-rw-rw-r--   0 j         (1000) j         (1000)    11950 2023-06-12 13:25:51.000000 pyfant-23.7.24.0/pyfant/molconsts.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.951988 pyfant-23.7.24.0/pyfant/run/
+-rw-rw-r--   0 j         (1000) j         (1000)      118 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/run/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)    18394 2023-07-05 21:06:29.000000 pyfant-23.7.24.0/pyfant/run/conf.py
+-rw-rw-r--   0 j         (1000) j         (1000)     9047 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/run/multirunnable.py
+-rw-rw-r--   0 j         (1000) j         (1000)    16962 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/run/rm.py
+-rw-rw-r--   0 j         (1000) j         (1000)    18010 2023-07-07 12:07:16.000000 pyfant-23.7.24.0/pyfant/run/runnables.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3725 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/run/traprbclass.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.955988 pyfant-23.7.24.0/pyfant/scripts/
+-rwxrwxr-x   0 j         (1000) j         (1000)     2363 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/_copy-from-sessions.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1633 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/_diff-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     4311 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/_plot-innewmarcs-result.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      563 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/_recreate-hitrandb.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2216 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/_save-pdf.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      625 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/abed.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      667 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/ated.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1104 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/convmol.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2791 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/copy-star.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3669 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/create-grid.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1286 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/cut-atoms.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1226 2023-07-05 21:06:29.000000 pyfant-23.7.24.0/pyfant/scripts/cut-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     6811 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/hitran-scraper.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3173 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/link.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      636 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/mained.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      943 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/mced.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2197 2023-07-03 22:19:58.000000 pyfant-23.7.24.0/pyfant/scripts/merge-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      703 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/mled.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      912 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/moldbed.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1848 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/nist-scraper.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     3879 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/nulbad.py
+-rwxrwxr-x   0 j         (1000) j         (1000)      849 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/optionsed.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2113 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/run-multi.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1152 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/run4.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2388 2023-07-15 01:09:27.000000 pyfant-23.7.24.0/pyfant/scripts/search-mollines.py
+-rw-rw-r--   0 j         (1000) j         (1000)     2298 2023-07-05 21:06:29.000000 pyfant-23.7.24.0/pyfant/scripts/split-molecules.py
+-rwxrwxr-x   0 j         (1000) j         (1000)    10219 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/tune-zinf.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2762 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/turbospectrum-to-atoms.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     2770 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/vald3-to-atoms.py
+-rwxrwxr-x   0 j         (1000) j         (1000)     1101 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/scripts/x.py
+-rw-rw-r--   0 j         (1000) j         (1000)    15663 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/util.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.955988 pyfant-23.7.24.0/pyfant/vis/
+-rw-rw-r--   0 j         (1000) j         (1000)       67 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/vis/__init__.py
+-rw-rw-r--   0 j         (1000) j         (1000)      723 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/vis/modgrid.py
+-rw-rw-r--   0 j         (1000) j         (1000)     3073 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/vis/vismany.py
+-rw-rw-r--   0 j         (1000) j         (1000)     8273 2020-10-12 00:16:49.000000 pyfant-23.7.24.0/pyfant/vis/vismod.py
+drwxrwxr-x   0 j         (1000) j         (1000)        0 2023-07-24 12:44:06.927989 pyfant-23.7.24.0/pyfant.egg-info/
+-rw-rw-r--   0 j         (1000) j         (1000)      445 2023-07-24 12:44:06.000000 pyfant-23.7.24.0/pyfant.egg-info/PKG-INFO
+-rw-rw-r--   0 j         (1000) j         (1000)     4194 2023-07-24 12:44:06.000000 pyfant-23.7.24.0/pyfant.egg-info/SOURCES.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        1 2023-07-24 12:44:06.000000 pyfant-23.7.24.0/pyfant.egg-info/dependency_links.txt
+-rw-rw-r--   0 j         (1000) j         (1000)      133 2023-07-24 12:44:06.000000 pyfant-23.7.24.0/pyfant.egg-info/requires.txt
+-rw-rw-r--   0 j         (1000) j         (1000)        7 2023-07-24 12:44:06.000000 pyfant-23.7.24.0/pyfant.egg-info/top_level.txt
+-rw-rw-r--   0 j         (1000) j         (1000)       38 2023-07-24 12:44:06.955988 pyfant-23.7.24.0/setup.cfg
+-rw-rw-r--   0 j         (1000) j         (1000)     1583 2023-07-24 12:43:58.000000 pyfant-23.7.24.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyfant-19.12.5.0/pyfant/__init__.py` & `pyfant-23.7.24.0/pyfant/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from .from_vald import *
 from .from_turbospectrum import *
 from .molconsts import *
 from .kovacs import *
 from .gui import *
 from . import gui
 from .vis import *
+from .misc import *
 
 
 # # Function to access package-specific config file
 #   ===============================================
 def get_config():
     """Returns PyfantConfigObj object that corresponds to file ~/.ftpyfant.conf"""
     return a99.get_config_obj(".pyfant.conf")
```

### Comparing `pyfant-19.12.5.0/pyfant/_star.py` & `pyfant-23.7.24.0/pyfant/_star.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/basic/constants.py` & `pyfant-23.7.24.0/pyfant/basic/constants.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/basic/conversion.py` & `pyfant-23.7.24.0/pyfant/basic/conversion.py`

 * *Files 16% similar despite different names*

```diff
@@ -197,14 +197,49 @@
 
 
     pieces = [f(piece) for f, piece in zip(_PSS_TRANSFORMS, _pieces)]
 
     return pieces
 
 
+def parse_label_mult_spdf(s):
+    """Parses strings such as "A 2 SIGMA", "b3Sigmag-", "a3Piu" ...
+
+    Returns: (label, multiplicity, spdf)
+
+    Examples:
+        'A 2 SIGMA' --> ('A', 2, 0)
+        'b3Sigmag-' --> ('b', 3, 0)
+        'a3Piu' --> ('a', 3, 1)
+
+    Note: This routine is more complete than parse_system_str() (the latter cannot parse Greek letters with subsequent
+    trailing letter (e.g. Piu)
+
+    Note: I wrote this to parse file '12C12C_15000-17500_P-BR.bsyn' and similar, but later realized I just need the
+          "label", so ended up not using this function, although it works.
+    """
+
+    s = s.strip()
+
+    expr = re.compile("([a-zA-Z])\s*(\d+)\s*([a-zA-Z]+)")
+    groups = expr.search(s)
+    label, _mult, _spdf = [groups[i] for i in range(1, 4)]
+    mult = int(_mult)
+    _spdf_ = _spdf.capitalize()
+    spdf = None
+    for i, greek in enumerate(("Sigma", "Pi", "Delta", "Phi")):
+        if _spdf_.startswith(greek):
+            spdf = i
+            break
+    if spdf is None:
+        raise ValueError(f"Invalid greek letter in '{s}'")
+    return label, mult, spdf
+
+
+
 def split_molecules_description(descr):
     """Breaks PFANT molecule description into "(name) (system) (optional notes)" --> (name, system, notes)
 
     System is identified by enclosing square brackets ("[", "]")
     """
 
     match = re.match("(.+?)\s*(\[.+\])\s*(.*)", descr)
@@ -260,14 +295,50 @@
     symbols_ = [rec.search(x).group().capitalize() for x in symbols]
     symbols_ = ["C" if x == "A" else x for x in symbols_]
     if symbols_[0] == symbols_[1]:
         return "{}{}".format(symbols_[0], "2")
     else:
         return "".join(symbols_)
 
+
+def parse_label_mult_spdf(s):
+    """Parses strings such as "A 2 SIGMA", "b3Sigmag-", "a3Piu" ...
+
+    Returns: (label, multiplicity, spdf)
+
+    Note: This routine is more complete than parse_system_str() (the latter cannot parse Greek letters with subsequent
+    trailing letter (e.g. Piu)
+    """
+
+    s = s.strip()
+
+    expr = re.compile("([a-zA-Z])\s*(\d+)\s*([a-zA-Z]+)")
+    groups = expr.search(string)
+    if groups is not None:
+        _pieces = groups[1:4]
+    else:
+        # Initial and final state are the same. Example "12C16O INFRARED [X 1 SIGMA+]"
+        expr = re.compile("\[\s*([a-zA-Z])\s*(\d+)\s*([a-zA-Z0-9]+)[+-]{0,1}\s*\]")
+
+        groups = expr.search(string)
+        if groups is not None:
+            _pieces = [groups[i] for i in range(1, 4)] * 2
+
+        if groups is None:
+            raise ValueError("Could not understand str '{}'".format(string))
+
+
+    pieces = [f(piece) for f, piece in zip(_PSS_TRANSFORMS, _pieces)]
+
+    return pieces
+
+
+
+
+
 # **        ****                ******        ****                ******        ****
 #   **    **    ******    ******      **    **    ******    ******      **    **    ******    ******
 #     ****            ****              ****            ****              ****            ****
 #
 # Conversion and formatting routines: Branch-related
 #
```

### Comparing `pyfant-19.12.5.0/pyfant/basic/misc.py` & `pyfant-23.7.24.0/pyfant/basic/misc.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/basic/paths.py` & `pyfant-23.7.24.0/pyfant/basic/paths.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/convmol/calc_qgbd.py` & `pyfant-23.7.24.0/pyfant/convmol/calc_qgbd.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-"""
-Transition-specific calculations
-
-References:
-  [1] agrup.plez7.f
-"""
-
-from collections import OrderedDict
-
-
-__all__ = ["calc_qgbd_tio_like"]
-
-
-def calc_qgbd_tio_like(molconsts, v_lo):
-    """
-    Calculates qv, gv, bv, dv in TiO-like fashion
-
-    Based on Fortran source 'agrup.plez7.f'
-
-    Args:
-        molconsts: dict-like object with keys:
-            "omega_e"
-            "omega_ex_e"
-            "omega_ey_e"
-            "B_e"
-            "alpha_e"
-            "D_e"
-            "beta_e"
-
-        v_lo: (integer) low transition level
-
-    Returns: qbdg, i.e., a dictionary with keys:
-            "qv", "gv", "bv", "dv", "gzero"
-    """
-
-    omega_e = molconsts["state2l_omega_e"]
-    omega_ex_e = molconsts["state2l_omega_ex_e"]
-    omega_ey_e = molconsts["state2l_omega_ey_e"]
-    B_e = molconsts["state2l_B_e"]
-    D_e = molconsts["state2l_D_e"]
-    alpha_e = molconsts["state2l_alpha_e"]
-    beta_e = molconsts["state2l_beta_e"]
-
-    if int(v_lo) != v_lo:
-        raise ValueError("Argument 'v_lo' must be an integer")
-
-    gzero = omega_e / 2.0 - omega_ex_e / 4.0 + omega_ey_e / 8.0
-    v_lo5 = v_lo + 0.5
-
-    # Franck-Condon factor. Currently always incorporated into "SJ"
-    qv = 1.
-    # rotational constant "B_v"
-    bv = B_e - alpha_e * v_lo5
-    # rotational constant "D_v"
-    dv = (D_e + beta_e * v_lo5) * 1.0e+06
-    # rotational term " G_A"
-    gv = omega_e * v_lo5 - omega_ex_e * v_lo5 ** 2 + omega_ey_e * v_lo5 ** 3 - gzero
-
-    qgbd = OrderedDict((("qv", qv), ("gv", gv), ("bv", bv), ("dv", dv), ("gzero", gzero)))
-
-    return qgbd
+# """
+# Transition-specific calculations
+# 
+# References:
+#   [1] agrup.plez7.f
+# """
+# 
+# from collections import OrderedDict
+# 
+# 
+# __all__ = ["calc_qgbd_tio_like"]
+# 
+# 
+# def calc_qgbd_tio_like(molconsts, v_lo):
+#     """
+#     Calculates qv, gv, bv, dv in TiO-like fashion
+# 
+#     Based on Fortran source 'agrup.plez7.f'
+# 
+#     Args:
+#         molconsts: dict-like object with keys:
+#             "omega_e"
+#             "omega_ex_e"
+#             "omega_ey_e"
+#             "B_e"
+#             "alpha_e"
+#             "D_e"
+#             "beta_e"
+# 
+#         v_lo: (integer) low transition level
+# 
+#     Returns: qbdg, i.e., a dictionary with keys:
+#             "qv", "gv", "bv", "dv", "gzero"
+#     """
+# 
+#     omega_e = molconsts["state2l_omega_e"]
+#     omega_ex_e = molconsts["state2l_omega_ex_e"]
+#     omega_ey_e = molconsts["state2l_omega_ey_e"]
+#     B_e = molconsts["state2l_B_e"]
+#     D_e = molconsts["state2l_D_e"]
+#     alpha_e = molconsts["state2l_alpha_e"]
+#     beta_e = molconsts["state2l_beta_e"]
+# 
+#     if int(v_lo) != v_lo:
+#         raise ValueError("Argument 'v_lo' must be an integer")
+# 
+#     gzero = omega_e / 2.0 - omega_ex_e / 4.0 + omega_ey_e / 8.0
+#     v_lo5 = v_lo + 0.5
+# 
+#     # Franck-Condon factor. Currently always incorporated into "SJ"
+#     qv = 1.
+#     # rotational constant "B_v"
+#     bv = B_e - alpha_e * v_lo5
+#     # rotational constant "D_v"
+#     dv = (D_e + beta_e * v_lo5) * 1.0e+06
+#     # rotational term " G_A"
+#     gv = omega_e * v_lo5 - omega_ex_e * v_lo5 ** 2 + omega_ey_e * v_lo5 ** 3 - gzero
+# 
+#     qgbd = OrderedDict((("qv", qv), ("gv", gv), ("bv", bv), ("dv", dv), ("gzero", gzero)))
+# 
+#     return qgbd
```

### Comparing `pyfant-19.12.5.0/pyfant/convmol/conv_kurucz.py` & `pyfant-23.7.24.0/pyfant/convmol/conv_hitran160.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,137 @@
-from .convlog import *
-from .conv import *
-import pyfant
+"""Molecular lines converter from HITRAN to PFANT format."""
 
-__all__ = ["ConvKurucz"]
+__all__ = ["ConvHITRAN160"]
 
+import a99, airvacuumvald as avv, sys
+from . import Conv
 
-class ConvKurucz(Conv):
-    """Converts Kurucz molecular lines data to PFANT "sets of lines"
+class ConvHITRAN160(Conv):
+    """Converts HITRAN molecular lines data to PFANT "sets of lines" using Einstein's coefficients
 
-        Args:
-            flag_hlf: Whether to calculate the gf's using Honl-London factors or
-                      use Kurucz's loggf instead
+    Args:
+        isowant: (=1) isotopologue ID according to HITRAN or literature e.g. [1]. Li et al. 2015 didn't follow
+                 HITRAN's isotopologues codes for CO
 
-                      ***Note** old format (FileKuruczMoleculeOld) does not have loggf information,
-                                therefore the only way to work with the latter file type is
-                                flag_hlf==True
+        flag_jl_from_branch: whether to determine Jl from (branch, J2l) using rule:
+            branch is P: Jl = J2l-1
+            branch is Q: Jl = J2l
+            branch is R: Jl = J2l+1
 
-            flag_normhlf: Whether to multiply calculated gf's by normalization factor
+    There is a working example conv_hitran_co.py in examples directory
 
-            flag_fcf: Whether to multiply calculated gf's by Franck-Condon Factor
+    References:
+        [1] Li, G., Gordon, I.E., Rothman, L.S., Tan, Y., Hu, S.M., Kassi, S., Campargue, A. and Medvedev, E.S., 2015.
+        Rovibrational line lists for nine isotopologues of the CO molecule in the X1Σ+ ground electronic state.
+        The Astrophysical Journal Supplement Series, 216(1), p.15.
 
-            flag_quiet: Will not log exceptions when a molecular line fails
-
-            flag_spinl: Whether or not to use the spinl of the Kurucz line list
-                        for branch determination (spin2l is always used). Effect:
-
-                - True: possible branches are P1, P12, P21, P2 and repeat for Q, R
-                        (12 possibilities in total)
-
-                - False: possible branches are P1, P2 and repeat for Q, R
-                         (6 possibilities in total)
-
-            iso: (int or None) isotope. If specified as int, only that isotope will be filtered;
-                 otherwise, all isotopes in file will be included. Isotope is
-                 field KuruczMolLine.iso (see KuruczMolLine, FileKuruczMol).
-
-                 **Note** old Kurucz file format does not have the isotope information, therefore,
-                          iso must be None or the thing will not work
+        [2] Plez's conversor translate_molec_linelists_v16.1.f
 
+        [3] Jorge Melendez's work on OH: extraehitran.f
     """
 
-    def __init__(self, flag_hlf=False, flag_fcf=False, flag_quiet=False, flag_special_fcf=False,
-                 flag_spinl=False, fcfs=None, iso=None, *args, **kwargs):
-        Conv.__init__(self, *args, **kwargs)
-        self.flag_hlf = flag_hlf
-        self.flag_fcf = flag_fcf
-        self.flag_quiet = flag_quiet
-        self.flag_spinl = flag_spinl
-        self.flag_special_fcf = flag_special_fcf
-        self.fcfs = fcfs
-        self.iso = iso
-
-    # TODO looks like this routine is kindda generic
-    # TODO could dismember this later
-    def _make_sols(self, lines):
-
-        def append_error(msg):
-            log.errors.append("#{}{} line: {}".format(i + 1, a99.ordinal_suffix(i + 1), str(msg)))
-
-        if not isinstance(lines, pyfant.FileKuruczMoleculeBase):
-            raise TypeError("Invalid type for argument 'fileobj': {}".format(type(lines).__name__))
-        assert self.flag_hlf or isinstance(lines, pyfant.FileKuruczMolecule), \
-               "Old-format file does not contain loggf, must activate Hönl-London factors"
-
-        lines = lines.lines
-        n = len(lines)
-
-        STATEL = self.molconsts["from_label"]
-        STATE2L = self.molconsts["to_label"]
-
-        mtools = self.kovacs_toolbox()
-
-        # Prepares result
-        sols = ConvSols(self.qgbd_calculator, self.molconsts)
-        log = MolConversionLog(n)
-
-        for i, line in enumerate(lines):
-            if self.iso and line.iso != self.iso:
-                log.skip_reasons["Isotope {}".format(line.iso)] += 1
-                continue
-
-            if line.statel != STATEL or line.state2l != STATE2L:
-                log.skip_reasons["Transition {}-{}".format(line.statel, line.state2l)] += 1
-                continue
-
-
-            branch = mtools.quanta_to_branch(line.Jl, line.J2l,
-                spinl=(None if not self.flag_spinl else line.spinl), spin2l=line.spin2l)
-
-
-            # This was only a test, but filters like these may be useful if line.spin2l != line.spinl:
-            #     log.skip_reasons["Different spin"] += 1
-            #     continue
-
+    def __init__(self, *args, isowant=1, flag_jl_from_branch=False, **kwargs):
+        super().__init__(*args, **kwargs)
+        if not (1 <= isowant <= 9):
+            raise ValueError(f"Invalid 'isowant': {isowant} (must be between 1 and 9)")
+        self.isowant = isowant
+        self.flag_jl_from_branch = flag_jl_from_branch
+
+    def _make_sols(self, f):
+        import pyfant
+        assert isinstance(f, pyfant.FileHITRAN160)
+
+        HITRAN = 1
+        LI2015 = 2
+        if isinstance(f, pyfant.FileHITRANHITRAN):
+            flavor = HITRAN
+        elif isinstance(f, pyfant.FileHITRANLi2015):
+            flavor = LI2015
+        else:
+            raise RuntimeError(f"Cannot handle class {f.__class__.__name__}")
+
+        log = self.log
+        sols = self.sols
+
+        n = log.n = len(f)
+        if n == 0:
+            raise RuntimeError("Zero lines found")
+
+        deltak = self.molconsts.get_deltak()
+        S2l = self.molconsts.get_S2l()
+
+        if self.flag_filter_labels and flavor == LI2015:
+            raise RuntimeError(f"Cannot filter labels (flag_filter_labels==True), as labels (e.g. \"A\", \"X\") "
+                               f"are not provided by FileLi2015")
+
+        if not self.flag_jl_from_branch and flavor == HITRAN:
+            raise RuntimeError(f"Cannot determine Jl another way for FileHITRANHITRAN: flag_jl_from_branch must be activated")
+
+        if self.flag_filter_labels:
+            ref_from_label = self.molconsts["from_label"]
+            ref_to_label = self.molconsts["to_label"]
 
+        for i, line in enumerate(f.lines):
             try:
-                sj = 1.
-
-                if self.flag_hlf:
-                    try:
-                        hlf = mtools.get_sj(line.vl, line.v2l, line.J2l, branch)
-                    except pyfant.NoLineStrength:
-                        log.skip_reasons["Cannot calculate HLF"] += 1
+                if line.iso != self.isowant:
+                    log.skip_reasons[f"isotopologue {line.iso}"] += 1
+                    continue
+
+                if self.flag_filter_labels:
+                    if line.from_label != ref_from_label or line.to_label != ref_to_label:
+                        log.skip_reasons[f"Wrong system: {line.from_label}-{line.to_label}"] += 1
                         continue
 
-                    if hlf < 0:
-                        log.skip_reasons["Negative SJ"] += 1
-                        continue
+                if flavor == HITRAN:
+                    J2l = line.J2l
 
-                    sj *= hlf
+                    # The following code was based on Jorge Melendez's extraehitran.f
+                    # HITRAN does not have Jl
+                    # branch examples: two letters, e.g. "PP", "QP", "SR", "PP", "OP"
+                    if line.branch == "PP":
+                        Jl = J2l-1
+                    elif line.branch == "QQ":
+                        Jl = J2l
+                    elif line.branch == "RR":
+                        Jl = J2l+1
+                    else:
+                        log.skip_reasons[f"Unhandled branch: {line.branch}"] += 1
+                        continue
+                    
+                elif flavor == LI2015:
+                    # This conversion of gp, gpp into Jl, J2l was taken from Plez's conversor [2]
+                    # and seems to be correct for the Li 2015 CO file (I checked (vl=3, v2l=0) against the CO from 1998
+                    # and J2l matches)
+                    J2l = (line.gpp-1.)/2.
+
+                    if not self.flag_jl_from_branch:
+                        Jl = (line.gp-1.)/2.
+                    else:
+                        if line.branch == "P":
+                            Jl = J2l-1
+                        elif line.branch == "Q":
+                            Jl = J2l
+                        elif line.branch == "R":
+                            Jl = J2l+1
+                        else:
+                            log.skip_reasons[f"Unhandled branch: {line.branch}"] += 1
+                            continue
 
                 else:
-                    sj *= 10**line.loggf
+                    raise NotImplementedError()
 
-                if self.flag_fcf:
-                    sj *= self._get_fcf(line.vl, line.v2l, self.flag_special_fcf)
+                lambda_ = avv.vacuum_to_air(1e8/line.nu)
+
+                SJ = self.get_sj_einstein(line.A, Jl, J2l, S2l, deltak, line.nu)
+
+                self.append_line2(line.vl, line.v2l, lambda_, SJ, J2l, line.branch)
 
             except Exception as e:
                 reason = a99.str_exc(e)
                 log.skip_reasons[reason] += 1
-                msg = "#{}{} line: {}".format(i + 1, a99.ordinal_suffix(i + 1), reason)
+                msg = "#{}{} line: {}".format(i+1, a99.ordinal_suffix(i+1), reason)
                 log.errors.append(msg)
                 if not self.flag_quiet:
                     a99.get_python_logger().exception(msg)
-                continue
-
-            sols.append_line(line, sj, branch)
 
-            # sol_key = "%3d%3d" % (line.vl, line.v2l)  # (v', v'') transition (v_sup, v_inf)
-            # raise RuntimeError("Como que o calculate_qgbd esta fazendo, sendo que o dicionario molconsts agora tem prefixos to e from?")
-            # if sol_key not in sols:
-            #     qgbd = self._calculate_qgbd(line.v2l)
-            #     sols[sol_key] = pyfant.SetOfLines(line.vl, line.v2l,
-            #                                   qgbd["qv"], qgbd["gv"], qgbd["bv"], qgbd["dv"], 1.)
-            #
-            # sol = sols[sol_key]
-            # sol.append_line(wl, gf_pfant, J2l_pfant, branch)
 
         return sols, log
```

### Comparing `pyfant-19.12.5.0/pyfant/convmol/conv_plez.py` & `pyfant-23.7.24.0/pyfant/convmol/conv_plez.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,96 +2,103 @@
 from .conv import *
 import pyfant
 
 __all__ = ["ConvPlez"]
 
 
 class ConvPlez(Conv):
-    """Converts Plez molecular lines data to PFANT "sets of lines"
+    """
+    Converts Plez molecular lines data to PFANT "sets of lines"
 
         Args:
-            flag_hlf: Whether to calculate the gf's using Honl-London factors or
-                      use Plez's loggf instead
-
-                      ***Note** old format (FilePlezMoleculeOld) does not have loggf information,
-                                therefore the only way to work with the latter file type is
-                                flag_hlf==True
-
-            flag_normhlf: Whether to multiply calculated gf's by normalization factor
+            species: species name within Plez's file. Examples: "NH A-X PGopher", "Sneden web" etc.
 
-            flag_fcf: Whether to multiply calculated gf's by Franck-Condon Factor
-
-            flag_quiet: Will not log exceptions when a molecular line fails
-
-            name: name of molecule+system, e.g., "NH A-X PGopher"
+    ***Note** old format (FilePlezMoleculeOld) does not have loggf information,
+              therefore the only way to work with the latter file type is
+              mode==CONVPLEZMODE_HLF
     """
 
-    def __init__(self, flag_hlf=False, flag_fcf=False, flag_quiet=False, flag_special_fcf=False,
-                 fcfs=None, name="", *args, **kwargs):
+    def __init__(self, *args, species="", **kwargs):
         Conv.__init__(self, *args, **kwargs)
-        self.flag_hlf = flag_hlf
-        self.flag_fcf = flag_fcf
-        self.flag_quiet = flag_quiet
-        self.flag_special_fcf = flag_special_fcf
-        self.fcfs = fcfs
-        self.name = name
+        self.species = species
 
     def _make_sols(self, file):
 
+        log = self.log
+        sols = self.sols
+
         def append_error(msg):
             log.errors.append("#{}{} line: {}".format(i + 1, a99.ordinal_suffix(i + 1), str(msg)))
 
         if not isinstance(file, pyfant.FilePlezLinelistBase):
             raise TypeError("Invalid type for argument 'fileobj': {}".format(type(file).__name__))
 
-        lines = file.molecules[self.name].lines
-        n = len(lines)
+        try:
+            lines = file.molecules[self.species].lines
+        except KeyError:
+            raise KeyError(f"Species '{self.species}' not found in {list(file.molecules.keys())}")
+        n = log.n = len(lines)
 
         if n == 0:
-            raise RuntimeError("Species '{}' has zero lines".format(self.name))
+            raise RuntimeError("Species '{}' has zero lines".format(self.species))
 
-        STATEL = self.molconsts["from_label"]
-        STATE2L = self.molconsts["to_label"]
+        if self.mode == ConvMode.HLF:
+            mtools = self.kovacs_toolbox()
+        else:
+            deltak = self.molconsts.get_deltak()
+            S2l = self.molconsts.get_S2l()
+
+        if self.flag_filter_labels:
+            if self.mode == ConvMode.EINSTEIN_MINIMAL:
+                raise ValueError(f"mode==ConvMode.EINSTEIN_MINIMAL and flag_filter_label==True are incompatible")
 
-        mtools = self.kovacs_toolbox()
-
-        # Prepares result
-        sols = ConvSols(self.qgbd_calculator, self.molconsts)
-        log = MolConversionLog(n)
+            from_label = self.molconsts["from_label"]
+            to_label = self.molconsts["to_label"]
 
         for i, line in enumerate(lines):
             branch = line.branch
+            sj = 1.
 
             try:
-                sj = 1.
+                if self.flag_filter_labels:
+                    if line.from_label != from_label or line.to_label != to_label:
+                        log.skip_reasons[f"Wrong system: {line.from_label}-{line.to_label}"] += 1
+                        continue
 
-                if self.flag_hlf:
+                if self.mode == ConvMode.HLF:
                     try:
                         hlf = mtools.get_sj(line.vl, line.v2l, line.J2l, branch)
                     except pyfant.NoLineStrength:
                         log.skip_reasons["Cannot calculate HLF"] += 1
                         continue
 
                     if hlf < 0:
                         log.skip_reasons["Negative SJ"] += 1
                         continue
 
                     sj *= hlf
 
                 else:
-                    sj *= 10**line.loggf
+                    if self.mode == ConvMode.EINSTEIN_MINIMAL:
+                        J = (line.gu-1.)/2.
+                        if J < 0: J = 0
+                        line.Jl = line.J2l = J
+                        line.vl = line.v2l = 0
+
+                    if not branch:
+                        branch = "-"
 
-                if self.flag_fcf:
-                    sj *= self._get_fcf(line.vl, line.v2l, self.flag_special_fcf)
+                    normalizationfactor = self.get_normalizationfactor(line.J2l, S2l, deltak)
+                    sj *= normalizationfactor*10**line.loggf
+
+                self.append_line(line, sj, branch)
 
             except Exception as e:
                 reason = a99.str_exc(e)
                 log.skip_reasons[reason] += 1
                 msg = "#{}{} line: {}".format(i + 1, a99.ordinal_suffix(i + 1), reason)
                 log.errors.append(msg)
                 if not self.flag_quiet:
                     a99.get_python_logger().exception(msg)
                 continue
 
-            sols.append_line(line, sj, branch)
-
         return sols, log
```

### Comparing `pyfant-19.12.5.0/pyfant/convmol/conv_vald3.py` & `pyfant-23.7.24.0/pyfant/convmol/conv_vald3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 VALD3-specific conversion
 """
 
 
 import a99
-from .calc_qgbd import calc_qgbd_tio_like
+# from .calc_qgbd import calc_qgbd_tio_like
 from .convlog import *
 from collections import OrderedDict
 
 
 __all__ = ["vald3_to_sols"]
 
 
 
 def vald3_to_sols(molconsts, file_vald3, qgbd_calculator):
     """
-    Converts HITRAN molecular lines data to PFANT "sets of lines"
+    Converts VALD3 molecular lines data to PFANT "sets of lines"
 
     Args:
         molconsts: a dict-like object combining field values from tables 'molecule', 'state',
                     and 'pfantmol' from a FileMolDB database
         file_vald3: FileVald3 instance with only one species
         qgbd_calculator: callable that can calculate "qv", "gv", "bv", "dv",
                          e.g., calc_qbdg_tio_like()
```

### Comparing `pyfant-19.12.5.0/pyfant/convmol/convlog.py` & `pyfant-23.7.24.0/pyfant/convmol/convlog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from collections import Counter
-import a99
+import a99, tabulate
 
 @a99.froze_it
 class MolConversionLog(object):
 
     @property
     def num_lines_skipped(self):
         """Sums all counts in self.skip_reasons"""
         return sum(self.skip_reasons.values())
 
+    @property
+    def n(self):
+        return self.num_lines
+
+    @n.setter
+    def n(self, x):
+        self.num_lines = x
 
     def __init__(self, num_lines=0, flag_ok=True):
         # Number of lines in input file
         self.num_lines = num_lines
         # Whether the conversion was considered successful (despite errors)
         self.flag_ok = flag_ok
         # List of error strings
@@ -20,7 +27,21 @@
         # Counter: {"reason": number_of_times, ...}
         # The key should be a descriptive reason, however shortish
         # Access like this:
         #     >>> log.skip_reasons["FCF not found for (vl,v2l)"] += 1
         #
         self.skip_reasons = Counter()
 
+        self.cnt_in = 0
+
+    def __str__(self):
+        INDENT = "    "
+        n = self.num_lines
+        _ret = [f"num_lines: {n}", f"flag_ok: {self.flag_ok}", f"included: {self.cnt_in}/{n}", f"excluded: {n-self.cnt_in}/{n}"]
+
+        if self.skip_reasons:
+            _ret.append("\n*** Skip reasons ***")
+            _ret.append("\n".join([INDENT+line for line in tabulate.tabulate([(k, v) for k, v in self.skip_reasons.items()], ["Reason", "number of occurences"]).split("\n")]))
+        if self.errors:
+            _ret.append("\n*** Errors ***")
+            _ret.append("\n".join([INDENT+line for line in self.errors]))
+        return "\n".join(_ret)
```

### Comparing `pyfant-19.12.5.0/pyfant/data/default/abonds.dat` & `pyfant-23.7.24.0/pyfant/data/default/abonds.dat`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/absoru2.dat` & `pyfant-23.7.24.0/pyfant/data/default/absoru2.dat`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/abxfwhm.py` & `pyfant-23.7.24.0/pyfant/data/default/abxfwhm.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/configmolconsts.py` & `pyfant-23.7.24.0/pyfant/data/default/configmolconsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/dissoc.dat` & `pyfant-23.7.24.0/pyfant/data/default/dissoc.dat`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/hitrandb.sqlite` & `pyfant-23.7.24.0/pyfant/data/default/hitrandb.sqlite`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/modeles.mod` & `pyfant-23.7.24.0/pyfant/data/default/modeles.mod`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/moldb.sqlite` & `pyfant-23.7.24.0/pyfant/data/default/moldb.sqlite`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/data/default/partit.dat` & `pyfant-23.7.24.0/pyfant/data/default/partit.dat`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/downloaders/__init__.py` & `pyfant-23.7.24.0/pyfant/downloaders/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/downloaders/downhitran.py` & `pyfant-23.7.24.0/pyfant/downloaders/downhitran.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/downloaders/downnist.py` & `pyfant-23.7.24.0/pyfant/downloaders/downnist.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/__init__.py` & `pyfant-23.7.24.0/pyfant/filetypes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,8 +15,12 @@
 from .filehitrandb import *
 from .filekuruczmol import *
 from .filepleztio import *
 from .filemolconsts import *
 from .fileconfconvmol import *
 from .filetraprb import *
 from .morespectra import *
-from .fileplezlinelist import *
+from .fileplezlinelist import *
+from .filebrooke2014 import *
+from .filemollist import *
+from .filehitran160 import *
+from .filecojm1998 import *
```

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/fileabonds.py` & `pyfant-23.7.24.0/pyfant/filetypes/fileabonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/fileabxfwhm.py` & `pyfant-23.7.24.0/pyfant/filetypes/fileabxfwhm.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/fileatoms.py` & `pyfant-23.7.24.0/pyfant/filetypes/fileatoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filedissoc.py` & `pyfant-23.7.24.0/pyfant/filetypes/filedissoc.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filehitrandb.py` & `pyfant-23.7.24.0/pyfant/filetypes/filehitrandb.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filehmap.py` & `pyfant-23.7.24.0/pyfant/filetypes/filehmap.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filekuruczmol.py` & `pyfant-23.7.24.0/pyfant/filetypes/filekuruczmol.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,72 @@
-"""VALD3 atomic or molecular lines file"""
-
-
 __all__ = ["KuruczMolLine", "KuruczMolLineOld", "KuruczMolLineOld1", "FileKuruczMolecule", "FileKuruczMoleculeOld",
            "FileKuruczMoleculeBase", "load_kurucz_mol", "FileKuruczMoleculeOld1", "FileKuruczMolecule1"]
 
 import a99
 from f311 import DataFile
 import io
 import os
-from collections import namedtuple
+from dataclasses import dataclass
+from typing import Any
 
 
 # Will update progress status every time the following number of lines is read from file
 _PROGRESS_INDICATOR_PERIOD = 1030 * 5
 
 
-KuruczMolLine = namedtuple("KuruczMolLine",
-    ["lambda_", "loggf", "J2l", "E2l", "Jl", "El", "atomn0", "atomn1", "state2l", "v2l",
-    "lambda_doubling2l", "spin2l", "statel", "vl", "lambda_doublingl", "spinl", "iso", ])
-
-
-KuruczMolLineOld = namedtuple("KuruczMolLineOld",
-                              ["lambda_", "J2l", "Jl", "atomn0", "atomn1", "state2l", "v2l",
-                               "lambda_doubling2l", "spin2l", "statel", "vl", "lambda_doublingl",
-                               "spinl", ])
-
-KuruczMolLineOld1 = namedtuple("KuruczMolLineOld1",
-                              ["lambda_", "J2l", "Jl", "state2l", "v2l", "spin2l", "statel", "vl",
-                               "spinl", ])
+@dataclass
+class KuruczMolLine:
+    lambda_: Any
+    loggf: Any
+    J2l: Any
+    E2l: Any
+    Jl: Any
+    El: Any
+    atomn0: Any
+    atomn1: Any
+    state2l: Any
+    v2l: Any
+    lambda_doubling2l: Any
+    spin2l: Any
+    statel: Any
+    vl: Any
+    lambda_doublingl: Any
+    spinl: Any
+    iso: Any
+    rest: Any
+
+
+@dataclass
+class KuruczMolLineOld:
+    lambda_: Any
+    J2l: Any
+    Jl: Any
+    atomn0: Any
+    atomn1: Any
+    state2l: Any
+    v2l: Any
+    lambda_doubling2l: Any
+    spin2l: Any
+    statel: Any
+    vl: Any
+    lambda_doublingl: Any
+    spinl: Any
+
+
+@dataclass
+class KuruczMolLineOld1:
+    lambda_: Any
+    J2l: Any
+    Jl: Any
+    state2l: Any
+    v2l: Any
+    spin2l: Any
+    statel: Any
+    vl: Any
+    spinl: Any
 
 
 def load_kurucz_mol(filename):
     """
     Attempts to load Kurucz molecular line list (tries old and new format)
 
     Returns:
@@ -91,16 +126,25 @@
         #
         #   204.5126 -7.917  2.5    83.925  2.5  48964.990 108X00f1   A07e1   16
         #   204.7561 -7.745  3.5   202.380  3.5  49025.320 108X00f1   A07e1   16
         #   204.9400 -7.883  5.5   543.596  6.5  49322.740 108X00e1   A07e1   16
         #   205.0076 -7.931  3.5   201.931  2.5  48964.990 108X00e1   A07e1   16
         #   205.0652 -7.621  4.5   355.915  4.5  49105.280 108X00f1   A07e1   16
         #   205.0652 -7.621  4.5   355.915  4.5  49105.280 108X00f1   A07e1   16
+        #
+        # Another sample from file cnax12brookek.asc
+        #  1500.0057 -3.734  7.5-35901.223  6.5 -42566.043 607X20f2   A22f2   12 617 K
+        #  1500.0122 -1.704100.5-34572.316101.5 -41237.107 607X09 2   A10f2   12 617 K
+        #  1500.0307 -2.220 84.5-33050.728 85.5 -39715.437 607X11f2   A12f2   12 617 K
+        #  1500.0701 -5.367 56.5-29897.673 57.5 -36562.207 607X13f2   A14f1   12 617 K
+        #  1500.0896 -3.745 95.5-22615.737 96.5  29280.184 607X03f2   A03f1   12 617 K BR
+        #
         # 1         11     18   23        33   38         49          61      69 1-based
         # 0         10     17   22        32   37         48          60      68 0-based
+        # 01234567890123456789012345678901234567890123456789012345678901234567890123456789
         #
         # FORMAT(F10.4.F7.3,F5.1,F10.3,F5.1,F11.3,I4,A1,I2,A1,I1,3X,A1,I2,A1,I1,3X,I2)
         # "
         # The code for the diatomic molecules is two 2-digit element numbers in
         # ascending order.  The labels consist of the electronic state, the vibrational
         # level, the lambda-doubling component, and the spin state.  Sometimes two
         # characters are required for the electronic state and the format becomes
@@ -120,51 +164,54 @@
         try:
             self.lines = []
             while True:
                 s = h.readline().strip("\n")
                 if len(s) == 0:
                     break
 
-                # Kurucz: "negative energies are predicted or extrapolated"
+                # Kurucz: "negative energies are predicted or extrapolated" ...
                 # (http: // kurucz.harvard.edu / linelists.html)
                 E2l = float(s[22:32])
-                if E2l < 0:
-                    E2l = -E2l
+                # (20230720) ... but it doesn't mean that I need to invert the value: loader should be as impartial as
+                #            possible
+                # if E2l < 0:
+                #     E2l = -E2l
                 El = float(s[37:48])
-                if El < 0:
-                    El = -El
+                # if El < 0:
+                #     El = -El
 
                 try:
                     spin2l = int(s[56:57])
                 except ValueError:
                     spin2l = 0
 
                 try:
                     spinl = int(s[64:65])
                 except ValueError:
                     spinl = 0
 
                 line = KuruczMolLine(
-                    float(s[0:10]) * 10,
-                    float(s[10:17]),
-                    float(s[17:22]),
-                    E2l,
-                    float(s[32:37]),
-                    El,
-                    int(s[48:50]),
-                    int(s[50:52]),
-                    s[52:53],
-                    int(s[53:55]),
-                    s[55:56],
-                    spin2l,
-                    s[60:61],
-                    int(s[61:63]),
-                    s[63:64],
-                    spinl,
-                    int(s[68:70]), )
+                    lambda_=float(s[0:10]) * 10,
+                    loggf=float(s[10:17]),
+                    J2l=float(s[17:22]),
+                    E2l=E2l,
+                    Jl=float(s[32:37]),
+                    El=El,
+                    atomn0=int(s[48:50]),
+                    atomn1=int(s[50:52]),
+                    state2l=s[52:53],
+                    v2l=int(s[53:55]),
+                    lambda_doubling2l=s[55:56],
+                    spin2l=spin2l,
+                    statel=s[60:61],
+                    vl=int(s[61:63]),
+                    lambda_doublingl=s[63:64],
+                    spinl=spinl,
+                    iso=int(s[68:70]),
+                    rest=s[70:])
 
 
                 self.lines.append(line)
                 r += 1
                 ii += 1
                 if ii == _PROGRESS_INDICATOR_PERIOD:
                     a99.get_python_logger().info(
@@ -176,14 +223,28 @@
             # f = type(e)(("Error around %d%s row of file '%s'" %
             #              (r + 1, a99.ordinal_suffix(r + 1), filename)) + ": " + str(
             #     e)).with_traceback(sys.exc_info()[2])
             raise RuntimeError("Error around %d%s row of file '%s': \"%s\"" %
                                (r + 1, a99.ordinal_suffix(r + 1), filename, a99.str_exc(e))) from e
 
 
+    def _do_save_as(self, filename):
+        with open(filename, "w") as h:
+            for l in self.lines:
+                #  1500.0896 -3.745 95.5-22615.737 96.5  29280.184 607X03f2   A03f1   12 617 K BR
+                a99.write_lf(h, f"{l.lambda_/10:10.4f}{l.loggf:7.3f}{l.J2l:5.1f}{l.E2l:10.3f}{l.Jl:5.1f}{l.El:11.3f}"
+                                f"{l.atomn0:2d}{l.atomn1:02d}{l.state2l:1s}{l.v2l:02d}{l.lambda_doubling2l:1s}"
+                                f"{l.spin2l:1d}   {l.statel:1s}{l.vl:02d}{l.lambda_doublingl:1s}{l.spinl:1d}"
+                                f"   {l.iso:2d}{l.rest}")
+
+
+ # 15000.896 -3.745 95.5 22615.737 96.5  29280.184 607X 3f2   A 3f112 617 K BR
+ # 1500.0896 -3.745 95.5-22615.737 96.5  29280.184 607X03f2   A03f1   12 617 K BR
+
+
 @a99.froze_it
 class FileKuruczMolecule1(FileKuruczMoleculeBase):
     """
     Kurucz molecular lines file following format of file "c2dabrookek.asc"
     """
 
     def _do_load(self, filename):
@@ -391,20 +452,14 @@
             self.lines = []
             while True:
                 s = h.readline().strip("\n")
                 if len(s) == 0:
                     break
 
 
-                """
-                KuruczMolLineOld1 = namedtuple("KuruczMolLineOld1",
-                              ["lambda_", "J2l", "Jl", "state2l", "v2l", "spin2l", "statel", "vl",
-                               "spinl", ])
-
-                """
 
 
                 line = KuruczMolLineOld1(
                     float(s[0:9]),
                     float(s[9:15]),
                     float(s[15:21]),
                     s[22:23],
```

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filemain.py` & `pyfant-23.7.24.0/pyfant/filetypes/filemain.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filemod.py` & `pyfant-23.7.24.0/pyfant/filetypes/filemod.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filemolconsts.py` & `pyfant-23.7.24.0/pyfant/filetypes/filemolconsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filemoldb.py` & `pyfant-23.7.24.0/pyfant/filetypes/filemoldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,23 +45,27 @@
             "from_spdf": ["Λ'", "0/1/2/3 meaning Σ/Π/Δ/Φ"],
             "to_label": ['State"', None],
             "to_spdf": ['Λ"', "0/1/2/3 meaning Σ/Π/Δ/Φ"]
         }
 
     }
 
-    def get_molconsts(self, s):
-        """Parse string and return MolConsts object."""
+    def get_molconsts(self, system_str):
+        """
+        Parses string and return MolConsts object.
+
+        Args:
+            system_str: system description as found in moldbed.py --> "System description" box. For example,
+                        "MgH [A 2 Pi - X 2 Sigma]". Also returned by MolConsts.get_str()
+        """
         import pyfant
         ret = pyfant.MolConsts()
-        ret.populate_all_using_str(self, s)
+        ret.populate_all_using_str(self, system_str)
         return ret
 
-
-
     def query_molecule(self, **kwargs):
         """Convenience function to query 'molecule' table
 
         Args:
             **kwargs: filter fieldname=value pairs to be passed to WHERE clause
 
         Returns: sqlite3 cursor
```

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filemolecules.py` & `pyfant-23.7.24.0/pyfant/filetypes/filemolecules.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         bbv=None: TODO ?doc? (calculated from diatomic molecular constants)
         ddv=None: TODO ?doc? (calculated from diatomic molecular constants)
         fact=None: TODO ?doc? (usually =1.)
         state_from=None: letter
         state_to=None: letter
     """
 
-    attrs = ["vl", "v2l", "qqv", "ggv", "bbv", "ddv", "fact", "num_lines", "state_from", "state_to"]
+    attrs = ["vl", "v2l", "qqv", "ggv", "bbv", "ddv", "fact", "num_lines", "state_from", "state_to", "llzero", "llfin"]
 
     @property
     def llzero(self):
         """Minimum wavelength"""
         return min(self.lmbdam)
 
     @property
@@ -82,19 +82,19 @@
         fieldnames = ["lmbdam", "sj", "jj", "branch"]
         for t in zip(self.lmbdam, self.sj, self.jj, self.branch):
             obj = a99.MyDBRow()
             for fieldname, value in zip(fieldnames, t):
                 obj[fieldname] = value
             yield obj
 
-    def cut(self, lzero, lfin):
+    def cut(self, lzero, lfin, jjmax=None):
         """Reduces the number of lines to only the ones whose lmbdam is inside [lzero, lfin]"""
         l, s, j, b = [], [], [], []
         for _l, _s, _j, _b in zip(self.lmbdam, self.sj, self.jj, self.branch):
-            if lzero <= _l <= lfin:
+            if lzero <= _l <= lfin and (jjmax is None or _j <= jjmax):
                 l.append(_l)
                 s.append(_s)
                 j.append(_j)
                 b.append(_b)
         self.lmbdam, self.sj, self.jj, self.branch = l, s, j, b
 
     def append_line(self, lmbdam, sj, jj, branch):
@@ -112,15 +112,15 @@
         self.jj = [self.jj[i] for i in ii]
         self.branch = [self.branch[i] for i in ii]
 
 
 @a99.froze_it
 class Molecule(a99.AttrsPart):
     attrs = ["description", "symbols", "fe", "do", "mm", "am", "bm", "ua", "ub",
-             "te", "cro", "s", "nv", "num_lines"]
+             "te", "cro", "s", "nv", "num_lines", "llzero", "llfin"]
 
     @property
     def llzero(self):
         """Minimum wavelength"""
         return min([a.llzero for a in self.sol])
 
     @property
@@ -208,19 +208,19 @@
     def __iter__(self):
         return iter(self.sol)
 
     def __getitem__(self, *args):
         return self.sol.__getitem__(*args)
 
 
-    def cut(self, lzero, lfin):
+    def cut(self, lzero, lfin, jjmax=None):
         """Reduces the number of lines to only the ones whose lmbdam is inside [lzero, lfin]"""
 
         for i in reversed(list(range(len(self)))):
-            self.sol[i].cut(lzero, lfin)
+            self.sol[i].cut(lzero, lfin, jjmax)
             if len(self.sol[i]) == 0:
                 del self.sol[i]
 
 
 @a99.froze_it
 class FileMolecules(DataFile):
     """
@@ -344,20 +344,20 @@
 
     def __iter__(self):
         return iter(self.molecules)
 
     def __getitem__(self, *args):
         return self.molecules.__getitem__(*args)
 
-    def cut(self, lzero, lfin):
+    def cut(self, lzero, lfin, jjmax=None):
         """Reduces the number of lines to only the ones whose lmbdam is inside [lzero, lfin]"""
 
         for i in reversed(list(range(len(self)))):
             m = self.molecules[i]
-            m.cut(lzero, lfin)
+            m.cut(lzero, lfin, jjmax)
             if len(m) == 0:
                 del self.molecules[i]
 
     def _do_load(self, filename):
         """Clears internal lists and loads from file."""
 
         with open(filename, "r") as h:
@@ -485,15 +485,15 @@
 
     def _do_save_as(self, filename):
         with open(filename, "w") as h:
             a99.write_lf(h, str(len(self.molecules)))
             a99.write_lf(h, self.titm)
             a99.write_lf(h, " ".join([str(x.nv) for x in self.molecules]))
             for i_m, m in enumerate(self.molecules):
-                a99.get_python_logger().info("Saving '{}': molecule {}/{}".format(filename, i_m+1, len(self.molecules)))
+                # todo cleanup a99.get_python_logger().info("Saving '{}': molecule {}/{}".format(filename, i_m+1, len(self.molecules)))
 
                 # # Assembles "titulo"
                 # ## Transitions
                 ltrans = []
                 for sol in m:
                     if sol.vl is None or sol.v2l is None:
                         break
```

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/fileoptions.py` & `pyfant-23.7.24.0/pyfant/filetypes/fileoptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 
         # pfant
         self.fn_dissoc    = None
         self.fn_partit    = None
         self.fn_abonds    = None
         self.fn_atoms   = None
         self.fn_molecules = None
+        self.fn_mollist = None
         self.fn_lines     = None
         self.fn_log       = None
         self.fn_progress = None
         self.flprefix = None
         self.no_molecules = None
         self.no_h = None
         self.no_atoms = None
```

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filepartit.py` & `pyfant-23.7.24.0/pyfant/filetypes/filepartit.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filepleztio.py` & `pyfant-23.7.24.0/pyfant/filetypes/filepleztio.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filetoh.py` & `pyfant-23.7.24.0/pyfant/filetypes/filetoh.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filetraprb.py` & `pyfant-23.7.24.0/pyfant/filetypes/filetraprb.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/filevald3.py` & `pyfant-23.7.24.0/pyfant/filetypes/filevald3.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/filetypes/morespectra.py` & `pyfant-23.7.24.0/pyfant/filetypes/morespectra.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/from_turbospectrum.py` & `pyfant-23.7.24.0/pyfant/from_turbospectrum.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/from_vald.py` & `pyfant-23.7.24.0/pyfant/from_vald.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/__init__.py` & `pyfant-23.7.24.0/pyfant/gui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from .a_XFileMolecules import *
 from .a_XFileOptions import *
 from .a_XMainAbonds import *
 from .a_XMolLinesEditor import *
 from .a_XPFANT import *
 from .a_XRunnableManager import *
 from .a_XMulti import *
+from .a_XFileMoleculeHistogram import *
 from . import _shared
 # from .a_WFileAbonds import *
 # from .a_WFileAbXFwhm import *
 # from .a_WFileMain import *
 # from .a_WOptionsEditor import *
 # from .a_XAtomLinesEditor import *
 # from .a_XFileAbonds import *
```

### Comparing `pyfant-19.12.5.0/pyfant/gui/_shared.py` & `pyfant-23.7.24.0/pyfant/gui/_shared.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WContinua.py` & `pyfant-23.7.24.0/pyfant/gui/a_WContinua.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WContinuum.py` & `pyfant-23.7.24.0/pyfant/gui/a_WContinuum.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WDBFCF.py` & `pyfant-23.7.24.0/pyfant/gui/a_WDBFCF.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WDBMolecule.py` & `pyfant-23.7.24.0/pyfant/gui/a_WDBMolecule.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WDBPFANTMol.py` & `pyfant-23.7.24.0/pyfant/gui/a_WDBPFANTMol.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WDBState.py` & `pyfant-23.7.24.0/pyfant/gui/a_WDBState.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WDBSystem.py` & `pyfant-23.7.24.0/pyfant/gui/a_WDBSystem.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WDBSystemPfantmolFCF.py` & `pyfant-23.7.24.0/pyfant/gui/a_WFileMolDB.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,114 +1,83 @@
 from PyQt5.QtCore import *
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
-from a99 import WDBRegistry
 import a99
-from .a_WDBFCF import *
-from .a_WDBPFANTMol import *
-from .a_WDBSystem import *
-
-__all__ = ["WDBSystemPFANTMolFCF"]
-
-
-class WDBSystemPFANTMolFCF(a99.WBase):
-    """Master-slave widget to lodge System and FCF widgets"""
-
-    # Emitted whenever the value of the 'id' property changes
-    id_changed = pyqtSignal()
-
-    @property
-    def id(self):
-        """System id or None"""
-        return self.w_system._get_id()
-
-    @property
-    def f(self):
-        """Object representing the file being edited (possibly a DataFile object)"""
-        return self._f
-
-    @f.setter
-    def f(self, f):
-        self.w_system.f = f
-        self.w_fcf.f = f
-        self.w_pfantmol.f = f
+from .a_WDBMolecule import WDBMolecule
+from .a_WDBState import WDBState
+from .a_WDBSystemPfantmolFCF import *
+import os
+
+
+__all__ = ["WFileMolDB"]
+
+
+class WFileMolDB(a99.WEditor):
+
 
     def __init__(self, *args):
-        a99.WBase.__init__(self, *args)
+        a99.WEditor.__init__(self, *args)
 
         # # Main layout & splitter
-        lmain = self.keep_ref(QVBoxLayout(self))
-        sp = self.keep_ref(QSplitter(Qt.Horizontal))
+        lmain = self.layout_editor
 
+        sp = self.splitter_bidon = QSplitter(Qt.Horizontal)
 
-        # ## First widget of splitter
+        # ## First widget of splitter: molecules
         w0 = self.keep_ref(QWidget())
         l0 = QVBoxLayout(w0)
-        a99.set_margin(l0, 0)
+        a99.set_margin(l0, 2)
         l0.setSpacing(2)
 
-        a = self.title_mol = QLabel(a99.format_title1("Systems"))
+        a = self.title_mol = QLabel(a99.format_title0("Molecules (Alt+&M)"))
         l0.addWidget(a)
 
-        w = self.w_system = WDBSystem(self.parent_form)
-        w.id_changed.connect(self.id_system_changed)
-        w.id_changed.connect(self.id_changed)
-        w.changed.connect(self.changed)
+        w = self.keep_ref(QLineEdit())
         l0.addWidget(w)
 
-        # ## Second widget of splitter
-        sp1 = self.keep_ref(QSplitter(Qt.Vertical))
-
-        # ### widget 1.1
-
-        w10 = self.keep_ref(QWidget())
-        l10 = QVBoxLayout(w10)
-        a99.set_margin(l10, 0)
-        l10.setSpacing(2)
-
-        a = self.title_state = self.keep_ref(QLabel(a99.format_title1("PFANT molecules")))
-        l10.addWidget(a)
-
-        w = self.w_pfantmol = WDBPFANTMol(self.parent_form)
+        w = self.w_mol = WDBMolecule(self.parent_form)
+        # **Note** Cannot set buddy to w itself because it has a Qt.NoFocus policy
+        a.setBuddy(w.tableWidget)
+        w.id_changed.connect(self.mol_id_changed)
         w.changed.connect(self.changed)
-        l10.addWidget(w)
-
-        # ### widget 1.1
-
-        w11 = self.keep_ref(QWidget())
-        l11 = QVBoxLayout(w11)
-        a99.set_margin(l11, 0)
-        l11.setSpacing(2)
+        l0.addWidget(w)
 
-        a = self.title_state = self.keep_ref(QLabel(a99.format_title1("Franck-Condon Factors")))
-        l11.addWidget(a)
+        # ## Second widget of splitter: tab widget containing the rest
+        w1 = self.tabWidget = QTabWidget(self)
 
-        w = self.w_fcf = WDBFCF(self.parent_form)
+        # ### First tab: systems, PFANT molecules, and Franck-Condon factors
+        w = self.w_system = WDBSystemPFANTMolFCF(self.parent_form)
         w.changed.connect(self.changed)
-        l11.addWidget(w)
-
+        w1.addTab(self.w_system, "Electronic systems (Alt+&E)")
 
-        # ## Adds widgets to splitters
-
-        sp1.addWidget(w10)
-        sp1.addWidget(w11)
+        # ### Second tab: NIST Chemistry Web Book data
+        w = self.w_state = WDBState(self.parent_form)
+        w.changed.connect(self.changed)
+        w1.addTab(self.w_state, "States from NIST (Alt+&S)")
 
         sp.addWidget(w0)
-        sp.addWidget(sp1)
+        sp.addWidget(w1)
+        # sp.setStretchFactor(0, 1)
+        # sp.setStretchFactor(1, 2)
 
         lmain.addWidget(sp)
 
         # # Final adjustments
         a99.nerdify(self)
 
-        self.w_system._move_to_first()
-
-
-    def set_id_molecule(self, id_):
-        """Propagates to self.w_system"""
+    def load(self, fobj):
+        a99.WEditor.load(self, fobj)
+        self.w_mol._move_to_first()
+
+    def _do_load(self, fobj):
+        self._f = fobj
+        self.w_mol.f = fobj
+        self.w_system.f = fobj
+        self.w_state.f = fobj
+
+    def mol_id_changed(self):
+        id_ = self.w_mol.id
+        row = self.w_mol.row
         self.w_system.set_id_molecule(id_)
-        # self._populate()
+        self.w_state.set_id_molecule(id_)
 
-    def id_system_changed(self):
-        self.w_pfantmol.set_id_system(self.w_system.id)
-        self.w_fcf.set_id_system(self.w_system.id)
```

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WFileAbXFwhm.py` & `pyfant-23.7.24.0/pyfant/gui/a_WFileAbXFwhm.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WFileAbonds.py` & `pyfant-23.7.24.0/pyfant/gui/a_WFileAbonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WFileMain.py` & `pyfant-23.7.24.0/pyfant/gui/a_WFileMain.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WFileMolConsts.py` & `pyfant-23.7.24.0/pyfant/gui/a_WFileMolConsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WMolecularConstants.py` & `pyfant-23.7.24.0/pyfant/gui/a_WMolecularConstants.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import a99
 import copy
 import pyfant
 import tabulate
 
 __all__ = ["WMolecularConstants"]
 
+
+# Max J2l / "JJ" for the HLF window
+MAX_JJ = 200
+
 # Spacing for grid layouts
 _LAYSP_GRID = 4
 # Margin for grid layouts
 _LAYMN_GRID = 0
 _SPACE_BETWEEN_FIELDS = 8
 # Spacing between label and combobox
 _LAYSP_CB = 3
@@ -118,15 +122,15 @@
                         try:
                             factor = self.fcfs[(vl, v2l)]
                         except KeyError:
                             l_text.append("Franck-Condon Factor not available")
                             continue
 
                     rows, header = [], None
-                    for J in range(40):
+                    for J in range(MAX_JJ+1):
                         mtools = pyfant.kovacs_toolbox(molconsts, flag_normalize=True)
                         mtools.populate(vl, v2l, J)
 
                         if header is None:
                             branches = [key[3] for key in mtools.dict_sj]
                             header = ["J"]+branches+["Sum"]
```

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_WOptionsEditor.py` & `pyfant-23.7.24.0/pyfant/gui/a_WOptionsEditor.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XAtomLinesEditor.py` & `pyfant-23.7.24.0/pyfant/gui/a_XAtomLinesEditor.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XConvMol.py` & `pyfant-23.7.24.0/pyfant/gui/a_XConvMol.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileAbonds.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileAbonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileAtoms.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileAtoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileAtomsHistogram.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileAtomsHistogram.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileMain.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileMain.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileMolConsts.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileMolConsts.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileMolDB.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileMolDB.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileMolecules.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileMolecules.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
 from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT # as NavigationToolbar2QT
 import matplotlib.pyplot as plt
 import numpy as np
 from .a_XMolLinesEditor import *
+from .a_XFileMoleculeHistogram import *
 import os.path
 import webbrowser
 import sys
 from ._shared import *
 import a99
 import pyfant
 
-
 __all__ = ["XFileMolecules"]
 
 
 NUM_PLOTS = len(SOL_HEADERS_PLOT)-1  # -1 because whe "lambda" does not have its plot
-
+MAX_NUM_BINS = 500
 
 class XFileMolecules(QMainWindow):
 
     def __init__(self, parent=None):
         QMainWindow.__init__(self, parent)
 
         self.f = None  # FileMolecules object
@@ -72,18 +72,54 @@
         a = self.widgetMol = QWidget()
         a.setLayout(self.layoutMol)
 
 
         # ** ** right of splitter
 
         # ** ** ** tab "Molecule info"
+
+        # ** ** ** ** Toolbar with molecule-specific resources
+
+        l2 = self.labelSpinBoxBins = QLabel("&Bins")
+        sb = self.spinBoxBins = QSpinBox()
+        sb.setMaximum(MAX_NUM_BINS)
+        sb.setValue(50)
+        l2.setBuddy(sb)
+
+        am = self.buttonWavelengthHistogram = QPushButton("Wavelength histogram")
+        am.clicked.connect(self.on_buttonWavelengthHistogram_clicked)
+        am.setToolTip("Plots histogram that gives a general profile of where the lines are wavelength-wise")
+
+        self.spacer1625 = QSpacerItem(0, 0, QSizePolicy.Expanding, QSizePolicy.Minimum)
+
+        l0 = self.layoutMolToolbar = QHBoxLayout()
+        l0.addWidget(l2)
+        l0.addWidget(sb)
+        l0.addWidget(am)
+        l0.addItem(self.spacer1625)
+        a99.set_margin(l0, 1)
+        a = self.widgetMolToolbar = QWidget()
+        a.setLayout(l0)
+        a.setFixedHeight(40)
+
+        self.labelMolInfo = QLabel('Molecule summary report')
         a = self.plainTextEditMolInfo = QPlainTextEdit()
         a.setFont(a99.MONO_FONT)
 
-        # ** ** ** tab "Molecular lines"
+        l = self.layoutMolInfo = QVBoxLayout()
+        a99.set_margin(l, 0)
+        l.setSpacing(1)
+        l.addWidget(self.widgetMolToolbar)
+        l.addWidget(self.labelMolInfo)
+        l.addWidget(self.plainTextEditMolInfo)
+
+        a = self.widgetMolInfo = QWidget()
+        a.setLayout(self.layoutMolInfo)
+
+        # ** ** ** tab "Sets of lines (Alt+L)"
 
         # ** ** ** ** left
 
         # P = QSizePolicy(QSizePolicy.Fixed, QSizePolicy.Expanding)
         self.labelSol = QLabel('Sets of lines (Ctrl+2)')
 
         a = self.listWidgetSol = QListWidget()
@@ -184,15 +220,15 @@
         a = self.splitterSol = QSplitter(Qt.Horizontal)
         a.addWidget(self.widgetSol)
         a.addWidget(self.tabWidgetSol)
         a.setStretchFactor(0, 2)
         a.setStretchFactor(1, 10)
 
         a = self.tabWidgetMol = QTabWidget()
-        a.addTab(self.plainTextEditMolInfo, "Molecule info (Alt+&M)")
+        a.addTab(self.widgetMolInfo, "Molecule info (Alt+&M)")
         a.addTab(self.splitterSol, "Sets of lines (Alt+&L)")
         a.setCurrentIndex(1)
         a.setFont(a99.MONO_FONT)
 
         # ** splitter: (list of molecules) | (molecules tab widget)
         a = self.splitterMol = QSplitter(Qt.Horizontal)
         a.addWidget(self.widgetMol)
@@ -254,14 +290,17 @@
                 if source == self.listWidgetSol:
                     self.edit_sol()
                     return True
             if event.key() == Qt.Key_Delete:
                 if source == self.listWidgetMol:
                     self.delete_mol()
                     return True
+                elif source == self.listWidgetSol:
+                    self.delete_sol()
+                    return True
         return False
 
     def closeEvent(self, event):
         if self.flag_changed:
             # http://straightedgelinux.com/blog/python/html/pyqtxt.html
             r = QMessageBox.question(self,
                         "About to exit",
@@ -344,24 +383,35 @@
             self.edit_mol()
         elif action == a_delete:
             self.delete_mol()
 
     def on_listWidgetSol_customContextMenuRequested(self, position):
         menu = QMenu()
         a_edit = menu.addAction("&Edit")
+        a_delete = menu.addAction("&Delete")
         action = menu.exec_(self.listWidgetSol.mapToGlobal(position))
         if action == a_edit:
             self.edit_sol()
+        elif action == a_delete:
+            self.delete_sol()
 
     def on_listWidgetMol_doubleClicked(self):
         self.edit_mol()
 
     def on_listWidgetSol_doubleClicked(self):
         self.edit_sol()
 
+    def on_buttonWavelengthHistogram_clicked(self):
+        f = plt.figure()
+        pyfant.plot_molhistogram(self.mol, num_bins=self.spinBoxBins.value())
+        plt.title(self.mol.description)
+        f.show()
+        # form = XFileMoleculeHistogram(self.mol)
+        # form.show()
+
     # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * #
 
     def load(self, f):
         """Loads file into GUI."""
         assert isinstance(f, pyfant.FileMolecules)
 
         self.f = f
@@ -406,14 +456,17 @@
                 item = QListWidgetItem(self.get_sol_string(i, sol))
                 w.addItem(item)
 
             if len(m) > 0:
                 w.setCurrentRow(0)
 
     def set_sol(self, j):
+        # TODO what if molecule has no set of lines (SOL)? Actually I can't allow molecule to have 0 SOLs
+        j = min(j, len(self.mol)-1)
+
         self.marker_row = None  # no longer valid, whatever it was
         self.sol_index = j
         self.sol = self.f.molecules[self.mol_index].sol[j]
         self.update_sol_info()
         self.plot_lines()
         self.set_editor_sol()
 
@@ -427,14 +480,15 @@
                 n = sum([info.flag for info in self.plot_info])  # number of subplots (0, 1 or 2)
                 # map to reuse plotting routine, contains what differs between each plot
 
                 map_ = [(SOL_HEADERS_PLOT[i], o.__getattribute__(SOL_ATTR_NAMES[i]))
                         for i in range(1, len(SOL_HEADERS_PLOT))]
 
                 i_subplot = 1
+                refaxis = None
                 for i in range(len(map_)):
                     y_label = map_[i][0]
                     pi = self.plot_info[i]
                     pi.y_vector = _y = map_[i][1]
 
                     if pi.flag:
                         if not self.flag_sort:
@@ -445,16 +499,17 @@
                             _y = np.array(_y)
                             ii = np.argsort(_x)
                             x = _x[ii]
                             y = _y[ii]
 
                         a99.format_BLB()
 
-                        self.figure.add_subplot(n, 1, i_subplot)
+                        self.figure.add_subplot(n, 1, i_subplot, sharex=refaxis)
                         pi.axis = ax = self.figure.gca()
+                        if i == 0: refaxis = ax  # for sharex next i-iteration
                         ax.clear()
                         ax.plot(x, y, 'k'+('' if len(x) > 1 else 'x'))
                         ax.set_xlabel('Wavelength ($\AA$)')
                         ax.set_ylabel(y_label)
 
                         # x-limits
                         xmin, xmax = min(x), max(x)
@@ -535,14 +590,27 @@
         if flag_changed:
             self.flag_changed = True
             item.setText(self.get_sol_string(self.listWidgetSol.currentRow(), obj))
             # item.setTextColor(QColor(255, 0, 0))
             self.update_sol_info()
             self.update_window_title()
 
+    def delete_sol(self):
+        sol = self.sol
+        if sol is None:
+            return
+        i = self.listWidgetSol.currentRow()
+        if i >= len(self.mol.sol):
+            return
+        del self.mol.sol[i]
+        self.listWidgetSol.takeItem(i)
+        self.flag_changed = True
+        self.update_window_title()
+
+
     # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * # * #
 
     def update_mol_info(self):
         """Makes report for the current molecule."""
         m = self.mol
         s = str(m)
         # No need to repeat this information, already shown in listWidgetSol
@@ -660,8 +728,8 @@
 
     @staticmethod
     def get_mol_string(m):
         return m.description
 
     @staticmethod
     def get_sol_string(index, sol):
-        return "%3d %7s" % (index+1, '(%d)' % len(sol))
+        return "%3d (%2d, %2s) %7s" % (index+1, sol.vl, sol.v2l, '(%d)' % len(sol))
```

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XFileOptions.py` & `pyfant-23.7.24.0/pyfant/gui/a_XFileOptions.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XMainAbonds.py` & `pyfant-23.7.24.0/pyfant/gui/a_XMainAbonds.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XMolLinesEditor.py` & `pyfant-23.7.24.0/pyfant/gui/a_XMolLinesEditor.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XMulti.py` & `pyfant-23.7.24.0/pyfant/gui/a_XMulti.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XPFANT.py` & `pyfant-23.7.24.0/pyfant/gui/a_XPFANT.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/gui/a_XRunnableManager.py` & `pyfant-23.7.24.0/pyfant/gui/a_XRunnableManager.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/kovacs.py` & `pyfant-23.7.24.0/pyfant/kovacs.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,17 @@
 
         return value
 
     def __update_with_data(self, vl, v2l, J, data):
         normalization_factor = 1.
         if self._flag_normalize:
             cc = self._molconsts
-            normalization_factor = 2. / ((2 * cc.get_S2l() + 1) * (2 * J + 1) * (2 - cc.get_deltak()))
+            # TODO 20230415 Was 2, I put 1
+            normalization_factor = 1. / ((2 * cc.get_S2l() + 1) * (2 * J + 1) * (2 - cc.get_deltak()))
+            # normalization_factor = 2. / ((2 * cc.get_S2l() + 1) * (2 * J + 1) * (2 - cc.get_deltak()))
 
         for branch, function in data:
             try:
                 value = function(J) * normalization_factor
 
                 if isinstance(value, complex):
                     value = NO_LINE_STRENGTH
```

### Comparing `pyfant-19.12.5.0/pyfant/molconsts.py` & `pyfant-23.7.24.0/pyfant/molconsts.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,23 @@
                 ti = db.get_table_info(tablename)
                 row = db.get_conn().execute("select * from {} where id = ?".format(tablename),
                                             (id_,)).fetchone()
 
                 if row is None:
                     raise ValueError("Invalid {}: id {} does not exist in table '{}'".format(keyname, id_, tablename))
 
-                for fieldname in ti:
+                for fieldname, fieldspecs in ti.items():
                     if not fieldname.startswith("id"):
-                        self[prefix + fieldname] = row[fieldname]
+                        # 20230612: convert empty string ('') to None
+                        value = row[fieldname]
+                        if fieldspecs["type"] == "real" and isinstance(value, str) and value == "":
+                            value = None
+
+
+                        self[prefix + fieldname] = value
 
             self[keyname] = id_
 
     def populate_ids(self, db):
         """Populates (id_*) with values found using (molecule name) and (from_*) and (to_*)."""
 
         assert isinstance(db, pyfant.FileMolDB)
```

### Comparing `pyfant-19.12.5.0/pyfant/run/conf.py` & `pyfant-23.7.24.0/pyfant/run/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,37 @@
 FOR_HYDRO2 = 1
 FOR_PFANT = 2
 FOR_NULBAD = 3
 
 _sequence_dict = {"innewmarcs": FOR_INNEWMARCS, "hydro2": FOR_HYDRO2, "pfant": FOR_PFANT, "nulbad": FOR_NULBAD}
 
 def translate_sequence(sequence):
-    """Convenience/tolerance function to convert strings with executable names to FOR_*"""
-    ret = []
-    return [_sequence_dict[x] if isinstance(x, str) else x for x in sequence]
+    """
+    Convenience/tolerance function to convert strings with executable names to FOR_*
+
+    Args:
+        sequence: examples:
+            ["innewmarcs", "hydro2", "pfant", "nulbad"]
+            [FOR_INNEWMARCS, FOR_HYDRO2, FOR_PFANT, FOR_NULBAD]
+            [True, True, True, True]
+            1111
+            "1111"
+            (all these examples evaluate to [FOR_INNEWMARCS, FOR_HYDRO2, FOR_PFANT, FOR_NULBAD])
+    """
+
+    if isinstance(sequence, int):
+        sequence = f"{sequence:04}"
+
+    if isinstance(sequence, str):
+        ret = [i for i, b in enumerate(sequence) if int(b)]
+    else:
+        ret = [_sequence_dict[x] if isinstance(x, str) else i if isinstance(x, bool) else x
+               for i, x in enumerate(sequence) if not isinstance(x, bool) or x]
+    return ret
+
 
 @a99.froze_it
 class SID(object):
     """
     SID -- Session Id and Directory
 
     Part of code that finds new session id and creates corresponding directory
@@ -258,14 +278,16 @@
         self.file_dissoc = None
         # ## FileHmap instance
         self.file_hmap = None
         # ## FileAtoms instance
         self.file_atoms = None
         # ## FileMolecules instance
         self.file_molecules = None
+        # ## FileMollist instance
+        self.file_mollist = None
 
         # # Command-line options
         self.__opt = pyfant.FileOptions()
 
         # # Read-only properties
         self.__popen_text_dest = None
         self.__logger = None
@@ -438,15 +460,15 @@
 
     def rename_outputs(self, sequence, opt=None, sid=None):
         """
         Adds session dir to names of files that will be created by any of the
         executables. To be called *before* create_data_files
 
         Args:
-            sequence: list containing one or more i_* values such as innewmarcs etc
+            sequence: list containing one or more i_* values such as innewmarcs etc.
             opt:
             sid:
 
         Note: in order to link pfant->nulbad correctly,
               nulbad "--fn_flux" option will not be used.
         """
         self.__rename_outputs(sequence, opt, sid)
```

### Comparing `pyfant-19.12.5.0/pyfant/run/multirunnable.py` & `pyfant-23.7.24.0/pyfant/run/multirunnable.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/run/rm.py` & `pyfant-23.7.24.0/pyfant/run/rm.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/run/runnables.py` & `pyfant-23.7.24.0/pyfant/run/runnables.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,18 @@
 
     def get_status(self):
         raise NotImplementedError()
 
     def run(self):
         raise NotImplementedError()
 
+    def clean(self):
+        """Deletes session directory"""
+        self.sid.clean()
+
     def kill(self):
         raise NotImplementedError()
 
     def load_result(self):
         """Abstract. Override this method to open the result file(s) particular to the
         executable.
 
@@ -142,18 +146,14 @@
         self._flag_finished = False
         self._flag_killed = False
         self._flag_error = False
         self._error_message = ""
         if self.sid.id:
             self.sid.clean(False)
 
-    def clean(self, *args):
-        """Wraps self.sid.clean(). See ftpyfant.SID"""
-        self.sid.clean(*args)
-
     def _get_sid(self):
         raise NotImplementedError()
 
 
 class PFANTExecutable(Runnable):
     """
     PFANT executables common ancestor class, or any other program
@@ -218,14 +218,18 @@
         self.conf.configure([self.sequence_index])
         try:
             self.conf.logger.debug("Running %s '%s'" % (self.__class__.__name__.lower(), self.name))
             self.__run()
         finally:
             self.conf.close_popen_text_dest()
 
+    def clean(self):
+        """Deletes session directory"""
+        self.sid.clean()
+
     def run_from_combo(self):
         """Alternative to run executable (called from Combo class).
 
         This routine bypasses all the configuration that is done prior to running.
         (Combo.configure() will do the necessary configuration).
         """
         assert not self._flag_running, "Already running"
@@ -423,15 +427,19 @@
 
         # nulbad output
         self.convolved = None
 
     def load_result(self):
         file_sp = pyfant.FileSpectrumNulbad()
         filepath = self.conf.get_nulbad_output_filepath()
-        file_sp.load(filepath)
+        try:
+            file_sp.load(filepath)
+        except:
+            print("WWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWWW")
+            raise
         self.convolved = file_sp.spectrum
         self._result["convolved"] = file_sp.spectrum
 
 
 @a99.froze_it
 
 class Combo(Runnable):
```

### Comparing `pyfant-19.12.5.0/pyfant/run/traprbclass.py` & `pyfant-23.7.24.0/pyfant/run/traprbclass.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/_copy-from-sessions.py` & `pyfant-23.7.24.0/pyfant/scripts/_copy-from-sessions.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/_diff-molecules.py` & `pyfant-23.7.24.0/pyfant/scripts/_diff-molecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/_plot-innewmarcs-result.py` & `pyfant-23.7.24.0/pyfant/scripts/_plot-innewmarcs-result.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/_recreate-hitrandb.py` & `pyfant-23.7.24.0/pyfant/scripts/_recreate-hitrandb.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/_save-pdf.py` & `pyfant-23.7.24.0/pyfant/scripts/_save-pdf.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/abed.py` & `pyfant-23.7.24.0/pyfant/scripts/abed.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/ated.py` & `pyfant-23.7.24.0/pyfant/scripts/ated.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/convmol.py` & `pyfant-23.7.24.0/pyfant/scripts/convmol.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/copy-star.py` & `pyfant-23.7.24.0/pyfant/scripts/copy-star.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/create-grid.py` & `pyfant-23.7.24.0/pyfant/scripts/create-grid.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/cut-atoms.py` & `pyfant-23.7.24.0/pyfant/scripts/cut-atoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/cut-molecules.py` & `pyfant-23.7.24.0/pyfant/scripts/cut-molecules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-#!/usr/bin/env python
+7#!/usr/bin/env python
 """
 Cuts molecular lines file to wavelength interval specified
 
 The interval is [llzero, llfin]
 """
 
-# TODO add this functionality to mled.py
-
 import argparse
 import logging
 import a99
 import pyfant
 
 
 a99.logging_level = logging.INFO
```

### Comparing `pyfant-19.12.5.0/pyfant/scripts/hitran-scraper.py` & `pyfant-23.7.24.0/pyfant/scripts/hitran-scraper.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/link.py` & `pyfant-23.7.24.0/pyfant/scripts/link.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/mained.py` & `pyfant-23.7.24.0/pyfant/scripts/mained.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/mced.py` & `pyfant-23.7.24.0/pyfant/scripts/mced.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/merge-molecules.py` & `pyfant-23.7.24.0/pyfant/scripts/merge-molecules.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/mled.py` & `pyfant-23.7.24.0/pyfant/scripts/mled.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/moldbed.py` & `pyfant-23.7.24.0/pyfant/scripts/moldbed.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/nist-scraper.py` & `pyfant-23.7.24.0/pyfant/scripts/nist-scraper.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/nulbad.py` & `pyfant-23.7.24.0/pyfant/scripts/nulbad.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/optionsed.py` & `pyfant-23.7.24.0/pyfant/scripts/optionsed.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/run-multi.py` & `pyfant-23.7.24.0/pyfant/scripts/run-multi.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/run4.py` & `pyfant-23.7.24.0/pyfant/scripts/run4.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/tune-zinf.py` & `pyfant-23.7.24.0/pyfant/scripts/tune-zinf.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/turbospectrum-to-atoms.py` & `pyfant-23.7.24.0/pyfant/scripts/turbospectrum-to-atoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/vald3-to-atoms.py` & `pyfant-23.7.24.0/pyfant/scripts/vald3-to-atoms.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/scripts/x.py` & `pyfant-23.7.24.0/pyfant/scripts/x.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/util.py` & `pyfant-23.7.24.0/pyfant/util.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/vis/modgrid.py` & `pyfant-23.7.24.0/pyfant/vis/modgrid.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/vis/vismany.py` & `pyfant-23.7.24.0/pyfant/vis/vismany.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant/vis/vismod.py` & `pyfant-23.7.24.0/pyfant/vis/vismod.py`

 * *Files identical despite different names*

### Comparing `pyfant-19.12.5.0/pyfant.egg-info/SOURCES.txt` & `pyfant-23.7.24.0/pyfant.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,17 @@
 pyfant/basic/conversion.py
 pyfant/basic/errors.py
 pyfant/basic/misc.py
 pyfant/basic/paths.py
 pyfant/convmol/__init__.py
 pyfant/convmol/calc_qgbd.py
 pyfant/convmol/conv.py
+pyfant/convmol/conv_brooke2014.py
 pyfant/convmol/conv_hitran.py
+pyfant/convmol/conv_hitran160.py
 pyfant/convmol/conv_kurucz.py
 pyfant/convmol/conv_plez.py
 pyfant/convmol/conv_vald3.py
 pyfant/convmol/convlog.py
 pyfant/data/default/abonds.dat
 pyfant/data/default/absoru2.dat
 pyfant/data/default/abxfwhm.py
@@ -43,24 +45,28 @@
 pyfant/downloaders/downhitran.py
 pyfant/downloaders/downnist.py
 pyfant/filetypes/__init__.py
 pyfant/filetypes/fileabonds.py
 pyfant/filetypes/fileabsoru2.py
 pyfant/filetypes/fileabxfwhm.py
 pyfant/filetypes/fileatoms.py
+pyfant/filetypes/filebrooke2014.py
+pyfant/filetypes/filecojm1998.py
 pyfant/filetypes/fileconfconvmol.py
 pyfant/filetypes/filedissoc.py
+pyfant/filetypes/filehitran160.py
 pyfant/filetypes/filehitrandb.py
 pyfant/filetypes/filehmap.py
 pyfant/filetypes/filekuruczmol.py
 pyfant/filetypes/filemain.py
 pyfant/filetypes/filemod.py
 pyfant/filetypes/filemolconsts.py
 pyfant/filetypes/filemoldb.py
 pyfant/filetypes/filemolecules.py
+pyfant/filetypes/filemollist.py
 pyfant/filetypes/fileoptions.py
 pyfant/filetypes/filepartit.py
 pyfant/filetypes/fileplezlinelist.py
 pyfant/filetypes/filepleztio.py
 pyfant/filetypes/filetoh.py
 pyfant/filetypes/filetraprb.py
 pyfant/filetypes/filevald3.py
@@ -86,21 +92,24 @@
 pyfant/gui/a_XConvMol.py
 pyfant/gui/a_XFileAbonds.py
 pyfant/gui/a_XFileAtoms.py
 pyfant/gui/a_XFileAtomsHistogram.py
 pyfant/gui/a_XFileMain.py
 pyfant/gui/a_XFileMolConsts.py
 pyfant/gui/a_XFileMolDB.py
+pyfant/gui/a_XFileMoleculeHistogram.py
 pyfant/gui/a_XFileMolecules.py
 pyfant/gui/a_XFileOptions.py
 pyfant/gui/a_XMainAbonds.py
 pyfant/gui/a_XMolLinesEditor.py
 pyfant/gui/a_XMulti.py
 pyfant/gui/a_XPFANT.py
 pyfant/gui/a_XRunnableManager.py
+pyfant/misc/__init__.py
+pyfant/misc/molhistogram.py
 pyfant/run/__init__.py
 pyfant/run/conf.py
 pyfant/run/multirunnable.py
 pyfant/run/rm.py
 pyfant/run/runnables.py
 pyfant/run/traprbclass.py
 pyfant/scripts/_copy-from-sessions.py
@@ -123,14 +132,16 @@
 pyfant/scripts/mled.py
 pyfant/scripts/moldbed.py
 pyfant/scripts/nist-scraper.py
 pyfant/scripts/nulbad.py
 pyfant/scripts/optionsed.py
 pyfant/scripts/run-multi.py
 pyfant/scripts/run4.py
+pyfant/scripts/search-mollines.py
+pyfant/scripts/split-molecules.py
 pyfant/scripts/tune-zinf.py
 pyfant/scripts/turbospectrum-to-atoms.py
 pyfant/scripts/vald3-to-atoms.py
 pyfant/scripts/x.py
 pyfant/vis/__init__.py
 pyfant/vis/modgrid.py
 pyfant/vis/vismany.py
```

### Comparing `pyfant-19.12.5.0/setup.py` & `pyfant-23.7.24.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 pkgs = find_packages()
 scripts = find_scripts([PACKAGE_NAME])
 
 setup(
     name=PACKAGE_NAME,
     packages=find_packages(),
     include_package_data=True,
-    version='19.12.5.0',
+    version='23.7.24.0',
     license='GNU GPLv3',
     platforms='any',
     description='Python interface to the PFANT spectral synthesis code, with a varied set of extra tools',
     author='Julio Trevisan',
     author_email='juliotrevisan@gmail.com',
     url='https://github.com/trevisanj/pyfant',
     keywords= ['astronomy', "stellar", "spectroscopy", "spectral", "synthesis",
                "honl-london", "nist", "hitran", "multiplicity", "line strength", "kovacs", "franck-condon"],
     install_requires=["numpy", "scipy", "matplotlib", "astropy", "configobj", "bs4", "lxml",
                       "robobrowser", "requests", "fortranformat", "tabulate", "rows", "pyqt5",
-                      "f311>=18.3.1.0", "airvacuumvald"],
+                      "f311>18.3.1.0", "airvacuumvald"],
     scripts=scripts
 )
 
 
 # TODO later install_requires=['numpy', 'matplotlib', 'pyqt5'],  # matplotlib never gets installed correctly by pip, but anyway...
```

