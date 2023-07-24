# Comparing `tmp/nadia-proof-0.1.6.tar.gz` & `tmp/nadia-proof-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadia-proof-0.1.6.tar", last modified: Mon May  1 15:18:16 2023, max compression
+gzip compressed data, was "nadia-proof-0.1.7.tar", last modified: Mon Jul 24 18:42:53 2023, max compression
```

## Comparing `nadia-proof-0.1.6.tar` & `nadia-proof-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 15:18:16.029686 nadia-proof-0.1.6/
--rw-rw-rw-   0        0        0     4898 2023-05-01 15:18:16.027686 nadia-proof-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     4311 2023-03-08 00:14:38.000000 nadia-proof-0.1.6/README.md
--rw-rw-rw-   0        0        0     1094 2022-11-18 21:07:18.000000 nadia-proof-0.1.6/license.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 15:18:16.029686 nadia-proof-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      986 2023-05-01 14:58:48.000000 nadia-proof-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:18:15.959688 nadia-proof-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 15:18:15.985686 nadia-proof-0.1.6/src/nadia/
--rw-rw-rw-   0        0        0        0 2023-05-01 15:14:32.000000 nadia-proof-0.1.6/src/nadia/__init__.py
--rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 nadia-proof-0.1.6/src/nadia/example_theorems.py
--rw-rw-rw-   0        0        0     1498 2023-05-01 14:59:06.000000 nadia-proof-0.1.6/src/nadia/nadia_pt.py
--rw-rw-rw-   0        0        0      301 2023-05-01 14:57:00.000000 nadia-proof-0.1.6/src/nadia/nadia_pt_basic_usage.py
--rw-rw-rw-   0        0        0   121044 2023-05-01 15:01:54.000000 nadia-proof-0.1.6/src/nadia/nadia_pt_fo.py
--rw-rw-rw-   0        0        0    18420 2023-03-08 00:12:28.000000 nadia-proof-0.1.6/src/nadia/nadia_pt_gui.py
-drwxrwxrwx   0        0        0        0 2023-05-01 15:18:16.025685 nadia-proof-0.1.6/src/nadia_proof.egg-info/
--rw-rw-rw-   0        0        0     4898 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-01 15:18:15.000000 nadia-proof-0.1.6/src/nadia_proof.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 18:42:53.051271 nadia-proof-0.1.7/
+-rw-rw-rw-   0        0        0     4898 2023-07-24 18:42:53.050264 nadia-proof-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4311 2023-03-08 00:14:38.000000 nadia-proof-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1094 2022-11-18 21:07:18.000000 nadia-proof-0.1.7/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 18:42:53.052262 nadia-proof-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-07-24 18:42:46.000000 nadia-proof-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:42:52.990261 nadia-proof-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:42:53.017261 nadia-proof-0.1.7/src/nadia/
+-rw-rw-rw-   0        0        0        0 2023-05-01 15:14:32.000000 nadia-proof-0.1.7/src/nadia/__init__.py
+-rw-rw-rw-   0        0        0     2114 2022-12-23 14:27:18.000000 nadia-proof-0.1.7/src/nadia/example_theorems.py
+-rw-rw-rw-   0        0        0     1498 2023-05-01 14:59:06.000000 nadia-proof-0.1.7/src/nadia/nadia_pt.py
+-rw-rw-rw-   0        0        0      301 2023-05-01 14:57:00.000000 nadia-proof-0.1.7/src/nadia/nadia_pt_basic_usage.py
+-rw-rw-rw-   0        0        0   121095 2023-07-24 18:30:48.000000 nadia-proof-0.1.7/src/nadia/nadia_pt_fo.py
+-rw-rw-rw-   0        0        0    18419 2023-07-24 18:30:48.000000 nadia-proof-0.1.7/src/nadia/nadia_pt_gui.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:42:53.046266 nadia-proof-0.1.7/src/nadia_proof.egg-info/
+-rw-rw-rw-   0        0        0     4898 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 18:42:52.000000 nadia-proof-0.1.7/src/nadia_proof.egg-info/top_level.txt
```

### Comparing `nadia-proof-0.1.6/PKG-INFO` & `nadia-proof-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadia-proof
-Version: 0.1.6
+Version: 0.1.7
 Summary: NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/nadia
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Natural Deduction,Teaching Logic,Educational Software
 Platform: UNKNOWN
```

### Comparing `nadia-proof-0.1.6/README.md` & `nadia-proof-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.6/license.txt` & `nadia-proof-0.1.7/license.txt`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.6/setup.py` & `nadia-proof-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='nadia-proof',
-    version='0.1.6',
+    version='0.1.7',
     license='MIT',
     author="Davi Romero de Vasconcelos",
     author_email='daviromero@ufc.br',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/daviromero/nadia',
     description='''NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.''',
```

### Comparing `nadia-proof-0.1.6/src/nadia/example_theorems.py` & `nadia-proof-0.1.7/src/nadia/example_theorems.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.6/src/nadia/nadia_pt.py` & `nadia-proof-0.1.7/src/nadia/nadia_pt.py`

 * *Files identical despite different names*

### Comparing `nadia-proof-0.1.6/src/nadia/nadia_pt_fo.py` & `nadia-proof-0.1.7/src/nadia/nadia_pt_fo.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
 
         return self.forAll == other.forAll and self.variable == other.variable and self.formula == other.formula
     
     def __ne__(self, other): 
         if not isinstance(other, QuantifierFormula):
             return NotImplemented
 
-        return self.forAll != other.forAll and self.variable != other.variable and self.formula != other.formula
+        return self.forAll != other.forAll or self.variable != other.variable or self.formula != other.formula
 
     def is_universal(self):
       return self.forAll
 
     def is_existential(self):
       return not self.forAll
 
@@ -312,14 +312,16 @@
     def is_substitutable(self, x, y):
       if (self.variable == y and x in self.formula.free_variables()):
         return False
       return self.formula.is_substitutable(x,y)# and (self.variable == y or x in self.formula.free_variables())
 
     def valid_substitution(self, formula):
       free_vars = formula.free_variables()
+      if len(free_vars)==0:
+         return self.formula==formula
       for v in free_vars:
         fAux = self.formula.substitution(self.variable, v)
         if (fAux==formula):
           return True
       return False
 
     def substitution(self, var_x, a):
@@ -740,38 +742,37 @@
   HYPOTHESIS_WITHOUT_BOX = 14
   CLOSE_BRACKET_WITHOUT_BOX = 15
   HYPOTHESIS_WITHOUT_CLOSED_BOX = 16
   BOX_MUST_BE_DISPOSED = 17
   LINES_MUST_BE_SEQUENCE = 18
   INVALID_SUBSTITUTION_UNIVERSAL = 19
   INVALID_UNIVERSAL_FORMULA = 20
-  INVALID_SUBSTITUTION_EXISTS = 21
-  INVALID_EXISTENCIAL_FORMULA = 22
-  INVALID_SUBSTITUTION_EXISTENCIAL = 23
-  VARIABLE_IS_NOT_FRESH_VARIABLE = 24
-  INVALID_CONCLUSION_EXISTENCIAL = 25
-  INVALID_CONCLUSION_UNIVERSAL = 26
-  INVALID_SCOPE_DELIMITER = 27
-  BOX_MUST_HAVE_A_VARIABLE = 28
-  BOX_MUST_BE_DISPOSED_BY_RULE = 29
-  INVALID_CONCLUSION_EXISTENCIAL_LAST_RULE = 30
-  INVALID_BOX_RESULT = 31
-  IS_NOT_DISJUNCTION = 32
-  IS_NOT_CONJUNCTION = 33
-  IS_NOT_IMPLICATION = 34
-  INVALID_LEFT_CONJUNCTION = 35
-  INVALID_RIGHT_CONJUNCTION = 36
-  INVALID_NEGATION = 37
-  INVALID_LEFT_OR_RIGHT_DISJUNCTION = 38
-  INVALID_LEFT_OR_RIGHT_CONJUNCTION = 39
-  IS_NOT_BOTTOM = 40
-  INVALID_CONCLUSION_UNIVERSAL_LAST_RULE = 41
-  BOX_MUST_HAVE_ONLY_A_VARIABLE = 42
-  INVALID_RULE = 43
-  INVALID_RULE_ONE_REFERENCE = 44
+  INVALID_EXISTENTIAL_FORMULA = 21
+  INVALID_SUBSTITUTION_EXISTENTIAL = 22
+  VARIABLE_IS_NOT_FRESH_VARIABLE = 23
+  INVALID_CONCLUSION_EXISTENTIAL = 24
+  INVALID_CONCLUSION_UNIVERSAL = 25
+  INVALID_SCOPE_DELIMITER = 26
+  BOX_MUST_HAVE_A_VARIABLE = 27
+  BOX_MUST_BE_DISPOSED_BY_RULE = 28
+  INVALID_CONCLUSION_EXISTENTIAL_LAST_RULE = 29
+  INVALID_BOX_RESULT = 30
+  IS_NOT_DISJUNCTION = 31
+  IS_NOT_CONJUNCTION = 32
+  IS_NOT_IMPLICATION = 33
+  INVALID_LEFT_CONJUNCTION = 34
+  INVALID_RIGHT_CONJUNCTION = 35
+  INVALID_NEGATION = 36
+  INVALID_LEFT_OR_RIGHT_DISJUNCTION = 37
+  INVALID_LEFT_OR_RIGHT_CONJUNCTION = 38
+  IS_NOT_BOTTOM = 39
+  INVALID_CONCLUSION_UNIVERSAL_LAST_RULE = 40
+  BOX_MUST_HAVE_ONLY_A_VARIABLE = 41
+  INVALID_RULE = 42
+  INVALID_RULE_ONE_REFERENCE = 43
 
 
 ## File ast.py
 hypothesis = {}
 
 def limpaHipotese():
     global hypothesis
@@ -900,15 +901,15 @@
               parser.has_error = True
               deduction_result.add_error(parser.get_error(constants.INVALID_BOX_RESULT, self.reference2, self))
 
 
     def toLatex(self, symbol_table):
         hypothesis_number = str(len(hypothesis) + 1)
         hypothesis[self.reference1.value] = hypothesis_number
-        latex = '\\infer[\\!\\!{\\rightarrow\\text{i, }'+ hypothesis_number +'}]{'+self.formula.toLatex()+'}{'+symbol_table.get_rule(self.reference2.value).toLatex(symbol_table)+'}'
+        latex = '\\infer[\\!\\!{\\rightarrow\\text{i}^{_'+ hypothesis_number +'}}]{'+self.formula.toLatex()+'}{'+symbol_table.get_rule(self.reference2.value).toLatex(symbol_table)+'}'
         return latex
 
 class DisjunctionIntroductionDef():
     def __init__(self, line, formula, reference1):
         self.line = line
         self.formula = formula
         self.reference1 = reference1
@@ -1064,15 +1065,15 @@
               deduction_result.add_error(parser.get_error(constants.INVALID_BOX_RESULT, self.reference5, self))
 
     def toLatex(self, symbol_table):
         hypothesis_number1 = str(len(hypothesis) + 1)
         hypothesis[self.reference2.value] = hypothesis_number1
         hypothesis_number2 = str(len(hypothesis) + 1)
         hypothesis[self.reference4.value] = hypothesis_number2
-        latex = '\\infer[\\!\\!{\\lor\\text{e, }'+ hypothesis_number1 + ', ' + hypothesis_number2 +'}]{'+self.formula.toLatex()+'}{{'+symbol_table.get_rule(self.reference1.value).toLatex(symbol_table)+'}&{'+symbol_table.get_rule(self.reference3.value).toLatex(symbol_table)+'}&{'+symbol_table.get_rule(self.reference5.value).toLatex(symbol_table)+'}}'
+        latex = '\\infer[\\!\\!{\\lor\\text{e}^{_{'+ hypothesis_number1 + ', ' + hypothesis_number2 +'} } }]{'+self.formula.toLatex()+'}{{'+symbol_table.get_rule(self.reference1.value).toLatex(symbol_table)+'}&{'+symbol_table.get_rule(self.reference3.value).toLatex(symbol_table)+'}&{'+symbol_table.get_rule(self.reference5.value).toLatex(symbol_table)+'}}'
         return latex
 
 class NegationIntroductionDef():
     def __init__(self,line, formula, reference1, reference2):
         self.line = line
         self.formula = formula
         self.reference1 = reference1
@@ -1103,15 +1104,15 @@
           if(formula2.toString() != '@'):
               parser.has_error = True
               deduction_result.add_error(parser.get_error(constants.INVALID_BOX_RESULT, self.reference2, self))
 
     def toLatex(self, symbol_table):
         hypothesis_number = str(len(hypothesis) + 1)
         hypothesis[self.reference1.value] = hypothesis_number
-        latex = '\\infer[\\!\\!{\\lnot\\text{i, }'+ hypothesis_number +'}]{'+self.formula.toLatex()+'}{'+symbol_table.get_rule(self.reference2.value).toLatex(symbol_table)+'}'
+        latex = '\\infer[\\!\\!{\\lnot\\text{i}^{_'+ hypothesis_number +'}}]{'+self.formula.toLatex()+'}{'+symbol_table.get_rule(self.reference2.value).toLatex(symbol_table)+'}'
         return latex
 
 class NegationEliminationDef():
     def __init__(self,line, formula, reference1, reference2):
         self.line = line
         self.formula = formula
         self.reference1 = reference1
@@ -1200,15 +1201,15 @@
       if(formula2.toString() != '@'):
           parser.has_error = True
           deduction_result.add_error(parser.get_error(constants.INVALID_BOX_RESULT, self.reference2, self))
 
     def toLatex(self, symbol_table):
         hypothesis_number = str(len(hypothesis) + 1)
         hypothesis[self.reference1.value] = hypothesis_number
-        latex = '\\infer[\\!\\!{\\text{raa}, '+ hypothesis_number +'}]{'+self.formula.toLatex()+'}{'+symbol_table.get_rule(self.reference2.value).toLatex(symbol_table)+'}'
+        latex = '\\infer[\\!\\!{\\text{raa}^_{'+ hypothesis_number +'} }]{'+self.formula.toLatex()+'}{'+symbol_table.get_rule(self.reference2.value).toLatex(symbol_table)+'}'
         return latex
 
 class CopyDef():
     def __init__(self, line, formula, reference1):
         self.line = line
         self.formula = formula
         self.reference1 = reference1
@@ -1299,19 +1300,19 @@
       formula_reference = parser.symbol_table.find_token(self.line)
       formula1 = parser.symbol_table.lookup_formula_by_line(self.line, self.reference1.value)
       if(formula1==None):
         return
       # If the formula is not a existential formula
       if(not isinstance(self.formula, QuantifierFormula) or (isinstance(self.formula, QuantifierFormula) and not self.formula.is_existential())):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_EXISTENCIAL_FORMULA, formula_reference, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_EXISTENTIAL_FORMULA, formula_reference, self))
       # If the conclusion is a valid substitution for the variable in formula1
       if(isinstance(self.formula, QuantifierFormula) and not self.formula.valid_substitution(formula1)):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_SUBSTITUTION_EXISTS, formula_reference, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_SUBSTITUTION_EXISTENTIAL, formula_reference, self))
 
     def toLatex(self, symbol_table):
         latex = '\\infer[\\!\\!\\exists\\text{i}]{'
         latex += self.formula.toLatex()
         latex += '}{'
         latex += symbol_table.get_rule(self.reference1.value).toLatex(symbol_table)
         latex += '}'
@@ -1351,32 +1352,32 @@
       formula2, formula3 = parser.symbol_table.check_scope_delimiter(self.reference2.value, self.reference3.value)
       if(formula1==None or formula2==None or formula3==None or formula_reference==None):
         return
 
       # If the rule conclusion is the same as the last formula of the box
       if(self.formula != formula3):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_CONCLUSION_EXISTENCIAL_LAST_RULE, self.reference3, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_CONCLUSION_EXISTENTIAL_LAST_RULE, self.reference3, self))
       # If the formula of the first reference is not a existential formula
       if(not isinstance(formula1, QuantifierFormula) or (isinstance(formula1, QuantifierFormula) and not formula1.is_existential())):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_EXISTENCIAL_FORMULA, formula_reference, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_EXISTENTIAL_FORMULA, formula_reference, self))
       # If the hypothesis formula (reference line 2) is a valid subtitutotion of the existential formula (reference line 1)
       if(isinstance(formula1, QuantifierFormula) and formula1.formula.substitution(formula1.variable, variable)!=formula2):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_SUBSTITUTION_EXISTENCIAL, self.reference2, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_SUBSTITUTION_EXISTENTIAL, self.reference2, self))
       # if the variable is a free variable at the conclusion formula (referecne line 3)
       if(variable in formula3.free_variables()):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_CONCLUSION_EXISTENCIAL, self.reference2, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_CONCLUSION_EXISTENTIAL, self.reference2, self))
 
     def toLatex(self, symbol_table):
         hypothesis_number = str(len(hypothesis) + 1)
         hypothesis[self.reference2.value] = hypothesis_number
-        latex = '\\infer[\\!\\!{\\exists\\text{e, }'+ hypothesis_number +'}]{'
+        latex = '\\infer[\\!\\!{\\exists\\text{e}^{_'+ hypothesis_number +'} }]{'
         latex += self.formula.toLatex()+'}{'
         latex += symbol_table.get_rule(self.reference1.value).toLatex(symbol_table)
         latex += ' & '+symbol_table.get_rule(self.reference3.value).toLatex(symbol_table)+ '}'
         return latex
 
 class ForAllIntroductiontionDef():
     def __init__(self,line, formula, reference1, reference2):
@@ -1413,15 +1414,15 @@
       formula1, formula2 = parser.symbol_table.check_scope_delimiter(self.reference1.value, self.reference2.value)
       if(formula1==None or formula2==None or formula_reference==None):
         return
 
       # If the formula of the first reference is not a existential formula
       if(not isinstance(self.formula, QuantifierFormula) or (isinstance(self.formula, QuantifierFormula) and not self.formula.is_universal())):
           parser.has_error = True
-          deduction_result.add_error(parser.get_error(constants.INVALID_EXISTENCIAL_FORMULA, formula_reference, self))
+          deduction_result.add_error(parser.get_error(constants.INVALID_EXISTENTIAL_FORMULA, formula_reference, self))
       # If the conclusion is a universal formula of the last formula (reference line 2) by substitution of the variable
       if(isinstance(self.formula, QuantifierFormula) and self.formula.formula.substitution(self.formula.variable, variable)!=formula2):
           parser.has_error = True
           deduction_result.add_error(parser.get_error(constants.INVALID_CONCLUSION_UNIVERSAL_LAST_RULE, self.reference2, self))
       # if the variable is a free variable at the conclusion formula (reference line 3)
       if(variable in self.formula.free_variables()):
           parser.has_error = True
@@ -2146,30 +2147,30 @@
             erro += "^, É necessário fechar o escopo desta caixa."
         elif type_error == constants.BOX_MUST_BE_DISPOSED:
             erro += "^, A hipótese que foi introduzida por essa caixa dever ser descartada pela regra que a introduziu em linha imediatamente posterior ao fechamento desta caixa."
         elif type_error == constants.BOX_MUST_BE_DISPOSED_BY_RULE:
             erro += "^, Esta caixa dever ser fechada em linha imediatamente posterior pela regra que a introduziu."
         elif type_error == constants.INVALID_SUBSTITUTION_UNIVERSAL:
             erro += "^, A fórmula {} não é uma substituição válida da fórmula universal refenciada na linha {}.".format(rule.formula.toString(), rule.reference1.value)
-        elif type_error == constants.INVALID_CONCLUSION_EXISTENCIAL_LAST_RULE:
+        elif type_error == constants.INVALID_CONCLUSION_EXISTENTIAL_LAST_RULE:
             erro += "^, A formula da conclusão desta regra deve ser a mesma fórmula refenciada na linha {}.".format(token_error.value)
         elif type_error == constants.INVALID_CONCLUSION_UNIVERSAL_LAST_RULE:
             erro += "^, A formula da conclusão desta regra deve ser a quantificação universal da fórmula refenciada na linha {} com a variável definida neste escopo.".format(token_error.value)
         elif type_error == constants.INVALID_UNIVERSAL_FORMULA:
             erro += "^, A fórmula referenciada na regra do universal não é uma fórmula do tipo universal."
-        elif type_error == constants.INVALID_SUBSTITUTION_EXISTENCIAL:
+        elif type_error == constants.INVALID_SUBSTITUTION_EXISTENTIAL:
             erro += "^, A fórmula {} não é uma substituição válida da fórmula existencial refenciada na linha {}.".format(rule.formula.toString(), rule.reference1.value)
 #            erro += "^, A fórmula refenciada na linha {} não é uma substituição correta da variável na fórmula do existencial desta regra.".format(token_error.value)
         elif type_error == constants.VARIABLE_IS_NOT_FRESH_VARIABLE:
             erro += "^, A variável utilizada na linha {} é uma variável livre de uma fórmula definida anteriormente e, portanto, não pode ser utilizada nesta regra.".format(token_error.value)
         elif type_error == constants.BOX_MUST_HAVE_A_VARIABLE:
             erro += "^, A caixa que inicia na linha {} deve iniciar com uma variável para esta regra.".format(token_error.value) 
         elif type_error == constants.BOX_MUST_HAVE_ONLY_A_VARIABLE:
             erro += "^, A caixa que inicia na linha {} não tem hipótese. A caixa deve iniciar com uma variável apenas para a regra da introdução do universal.".format(token_error.value) 
-        elif type_error == constants.INVALID_CONCLUSION_EXISTENCIAL:
+        elif type_error == constants.INVALID_CONCLUSION_EXISTENTIAL:
             erro += "^, A variável utilizada na conclusão dessa regra não pode ser a variável utilizada na caixa que inicia na linha {}.".format(token_error.value)
         elif type_error == constants.INVALID_CONCLUSION_UNIVERSAL:
             erro += "^, A variável utilizada na caixa que inicia na linha {} não pode ocorrer como variável livre na conclusão da fórmula e, portanto, não pode ser utilizada nesta regra.".format(token_error.value)
         
         return erro
     
     def get_parser(self):
```

### Comparing `nadia-proof-0.1.6/src/nadia/nadia_pt_gui.py` & `nadia-proof-0.1.7/src/nadia/nadia_pt_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         if result!=None:
           if(result.errors==[]):
               s_theorem = ParserNadia.toString(result.premisses, result.conclusion)
               l_theorem = ParserNadia.toLatex(result.premisses, result.conclusion)
               set_premisses = set([p.toString() for p in premisses])
               set_premisses_result = set([p.toString() for p in result.premisses])
               if(conclusion==result.conclusion and set_premisses==set_premisses_result):
-                display(HTML(rf'<font color="blue">Parabéns! A demonstraçãoo de {s_theorem} está correta.</font>'))
+                display(HTML(rf'<font color="blue">Parabéns! A demonstração de {s_theorem} está correta.</font>'))
                 msg =[]
                 if(cGentzen.value):
                   msg.append("Código Latex no Estilo de Gentzen:")
                   msg.append("%"+l_theorem )
                   msg.append(result.gentzen)
                 if(cFitch.value):
                   msg.append("Código Latex no Estilo de Fitch:")
```

### Comparing `nadia-proof-0.1.6/src/nadia_proof.egg-info/PKG-INFO` & `nadia-proof-0.1.7/src/nadia_proof.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadia-proof
-Version: 0.1.6
+Version: 0.1.7
 Summary: NADIA is a proof assistant for teaching natural deduction to computer science students. NADIA allows students to write their proofs and automatically checks whether the proofs are correct and, if not, displays any errors found.
 Home-page: https://github.com/daviromero/nadia
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Natural Deduction,Teaching Logic,Educational Software
 Platform: UNKNOWN
```

