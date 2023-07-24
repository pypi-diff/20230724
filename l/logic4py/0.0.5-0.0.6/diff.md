# Comparing `tmp/logic4py-0.0.5.tar.gz` & `tmp/logic4py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logic4py-0.0.5.tar", last modified: Tue Mar  7 23:56:46 2023, max compression
+gzip compressed data, was "logic4py-0.0.6.tar", last modified: Mon Jul 24 18:48:50 2023, max compression
```

## Comparing `logic4py-0.0.5.tar` & `logic4py-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 23:56:46.296887 logic4py-0.0.5/
--rw-rw-rw-   0        0        0     1033 2023-03-07 23:56:46.293889 logic4py-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      586 2023-03-07 23:55:16.000000 logic4py-0.0.5/README.md
--rw-rw-rw-   0        0        0     1089 2023-02-06 21:16:53.000000 logic4py-0.0.5/license.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 23:56:46.296887 logic4py-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      912 2023-03-07 23:54:14.000000 logic4py-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-07 23:56:46.224888 logic4py-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-07 23:56:46.259899 logic4py-0.0.5/src/logic4py/
--rw-rw-rw-   0        0        0        0 2023-02-06 21:16:53.000000 logic4py-0.0.5/src/logic4py/__init__.py
--rw-rw-rw-   0        0        0     2553 2023-02-27 23:18:45.000000 logic4py-0.0.5/src/logic4py/decoder.py
--rw-rw-rw-   0        0        0    10680 2023-03-07 23:51:58.000000 logic4py-0.0.5/src/logic4py/example_reasoning.py
--rw-rw-rw-   0        0        0     2114 2023-02-06 21:16:53.000000 logic4py-0.0.5/src/logic4py/example_theorems.py
--rw-rw-rw-   0        0        0    27860 2023-02-16 15:33:24.000000 logic4py-0.0.5/src/logic4py/formula.py
--rw-rw-rw-   0        0        0     1432 2023-02-06 21:16:53.000000 logic4py-0.0.5/src/logic4py/lexer.py
--rw-rw-rw-   0        0        0    55958 2023-02-27 23:31:26.000000 logic4py-0.0.5/src/logic4py/logic_gui.py
--rw-rw-rw-   0        0        0    16255 2023-02-27 21:39:57.000000 logic4py-0.0.5/src/logic4py/parser_def_formula.py
--rw-rw-rw-   0        0        0     6426 2023-02-06 21:16:53.000000 logic4py-0.0.5/src/logic4py/parser_formula.py
--rw-rw-rw-   0        0        0     8101 2023-02-06 21:16:53.000000 logic4py-0.0.5/src/logic4py/parser_theorem.py
-drwxrwxrwx   0        0        0        0 2023-03-07 23:56:46.292888 logic4py-0.0.5/src/logic4py.egg-info/
--rw-rw-rw-   0        0        0     1033 2023-03-07 23:56:46.000000 logic4py-0.0.5/src/logic4py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      494 2023-03-07 23:56:46.000000 logic4py-0.0.5/src/logic4py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 23:56:46.000000 logic4py-0.0.5/src/logic4py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-07 23:56:46.000000 logic4py-0.0.5/src/logic4py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-07 23:56:46.000000 logic4py-0.0.5/src/logic4py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:50.599594 logic4py-0.0.6/
+-rw-rw-rw-   0        0        0     1033 2023-07-24 18:48:50.597611 logic4py-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      586 2023-03-07 23:55:16.000000 logic4py-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1089 2023-02-06 21:16:53.000000 logic4py-0.0.6/license.txt
+-rw-rw-rw-   0        0        0       42 2023-07-24 18:48:50.599594 logic4py-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      912 2023-07-24 18:47:50.000000 logic4py-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:50.509664 logic4py-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:50.553598 logic4py-0.0.6/src/logic4py/
+-rw-rw-rw-   0        0        0        0 2023-02-06 21:16:53.000000 logic4py-0.0.6/src/logic4py/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-07-24 18:31:30.000000 logic4py-0.0.6/src/logic4py/decoder.py
+-rw-rw-rw-   0        0        0    12099 2023-06-19 22:23:24.000000 logic4py-0.0.6/src/logic4py/example_reasoning.py
+-rw-rw-rw-   0        0        0     2114 2023-02-06 21:16:53.000000 logic4py-0.0.6/src/logic4py/example_theorems.py
+-rw-rw-rw-   0        0        0    28139 2023-07-24 18:31:30.000000 logic4py-0.0.6/src/logic4py/formula.py
+-rw-rw-rw-   0        0        0     1432 2023-02-06 21:16:53.000000 logic4py-0.0.6/src/logic4py/lexer.py
+-rw-rw-rw-   0        0        0    59631 2023-07-24 18:31:30.000000 logic4py-0.0.6/src/logic4py/logic_gui.py
+-rw-rw-rw-   0        0        0    17270 2023-03-20 22:08:30.000000 logic4py-0.0.6/src/logic4py/parser_def_formula.py
+-rw-rw-rw-   0        0        0     6426 2023-02-06 21:16:53.000000 logic4py-0.0.6/src/logic4py/parser_formula.py
+-rw-rw-rw-   0        0        0     8101 2023-02-06 21:16:53.000000 logic4py-0.0.6/src/logic4py/parser_theorem.py
+drwxrwxrwx   0        0        0        0 2023-07-24 18:48:50.594622 logic4py-0.0.6/src/logic4py.egg-info/
+-rw-rw-rw-   0        0        0     1033 2023-07-24 18:48:50.000000 logic4py-0.0.6/src/logic4py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      494 2023-07-24 18:48:50.000000 logic4py-0.0.6/src/logic4py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 18:48:50.000000 logic4py-0.0.6/src/logic4py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-24 18:48:50.000000 logic4py-0.0.6/src/logic4py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 18:48:50.000000 logic4py-0.0.6/src/logic4py.egg-info/top_level.txt
```

### Comparing `logic4py-0.0.5/PKG-INFO` & `logic4py-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logic4py
-Version: 0.0.5
+Version: 0.0.6
 Summary: logic4py is a libray for teaching logic to computer science students.
 Home-page: https://github.com/daviromero/logic4py
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Propositional Logic,First-Order Logia,Teaching Logic,Educational Software
 Platform: UNKNOWN
```

### Comparing `logic4py-0.0.5/README.md` & `logic4py-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `logic4py-0.0.5/license.txt` & `logic4py-0.0.6/license.txt`

 * *Files identical despite different names*

### Comparing `logic4py-0.0.5/setup.py` & `logic4py-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='logic4py',
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     author="Davi Romero de Vasconcelos",
     author_email='daviromero@ufc.br',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/daviromero/logic4py',
     description='''logic4py is a libray for teaching logic to computer science students.''',
```

### Comparing `logic4py-0.0.5/src/logic4py/decoder.py` & `logic4py-0.0.6/src/logic4py/decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import ruamel.yaml
 
 def decode_fo_interpretation(input_fo_interpretatio, universe_key='U'):
   data_fo_interpretatio = input_fo_interpretatio.replace('=',':').replace('{','[').replace('}',']').replace('set()','[]').replace('(','[').replace(')',']')
   yaml = ruamel.yaml.YAML(typ='safe')
   data = yaml.load(data_fo_interpretatio)
   U = set([str(s) for s in data[universe_key]])
+  if len(U)==0: 
+    raise ValueError(f'O conjunto universo não pode ser vazio.')
   preds = {}
   s = {}
   for key in data.keys():
     if key==universe_key:
       continue
     elif key[0].isupper() and (data[key]==1 or data[key]==0):
       preds[key] = data[key]
```

### Comparing `logic4py-0.0.5/src/logic4py/example_reasoning.py` & `logic4py-0.0.6/src/logic4py/example_reasoning.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     'result_value': False
     }
 
 EXAMPLES['q4'] = {  
     'input_assumptions_pt': ['Se o dólar sobe, então os produtos ficam mais caros.',
                                 'O dólar não subiu.'], 
     'input_conclusion_pt' : 'Os produtos não ficaram mais caros.',
-    'result_value': True
+    'result_value': False
     }
 
 EXAMPLES['q5'] = {  
     'input_assumptions_pt': ['Se o dólar sobe, então os produtos ficam mais caros.',
                                 'O dólar não subiu.'], 
     'input_conclusion_pt' : 'Os produtos ficaram mais caros.',
     'result_value': False
@@ -237,7 +237,34 @@
     }
 
 EXAMPLES['q12_fo'] = {  
     'input_assumptions_pt': ['Todos que frequentam as aulas e fazem os exercícios são aprovados.', 'Alguém não é aprovado.'] , 
     'input_conclusion_pt' : 'Existe alguém que não frequenta as aulas e não faz os exercícios.',
     'result_value': False
     }
+
+
+def to_str(input_assumptions, input_conclusion, result_value=False, language_pt=True):
+    result = 'Considere as seguintes afirmações:' if language_pt else 'Consider the following statements:'
+    i = 1
+    for s in input_assumptions:
+        result+=f'\n{i}. '+s
+        i+=1
+    result+= f'\nPodemos concluir que a afirmação abaixo segue logicamente das afirmações acima?' if language_pt else 'Can we conclude that the statement below follows logically from the statements above?'
+    result+=f'\n{i}.'+input_conclusion
+    result+="\nA) Sim" if language_pt else "\nA) Yes"
+    result+="\nB) Não" if language_pt else "\nB) No"
+    return result
+
+def to_aiken(input_assumptions, input_conclusion, result_value=False, language_pt=True):
+    result = 'Considere as seguintes afirmações:' if language_pt else 'Consider the following statements:'
+    i = 1
+    for s in input_assumptions:
+        result+=f' {i}. '+s
+        i+=1
+    result+= f' Podemos concluir que a afirmação a seguir segue logicamente das afirmações anteriores?' if language_pt else ' Can we conclude that the following statement follows logically from the previous statements?'
+    result+=f' {i}.'+input_conclusion
+    result+="\nA) Sim" if language_pt else "\nA) Yes"
+    result+="\nB) Não" if language_pt else "\nB) No"
+    result+="\nANSWER: "+ ("A" if result_value else "B")
+    return fr'{result}'
+
```

### Comparing `logic4py-0.0.5/src/logic4py/example_theorems.py` & `logic4py-0.0.6/src/logic4py/example_theorems.py`

 * *Files identical despite different names*

### Comparing `logic4py-0.0.5/src/logic4py/formula.py` & `logic4py-0.0.6/src/logic4py/formula.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     def bound_variables(self):
       return self.all_variables().difference(self.free_variables())
 
     def free_variables(self):
       return self.left.free_variables().union(self.right.free_variables())
 
     def is_substitutable(self, x, y):
-      return self.left.substitutable(x,y) and self.right.substitutable(x,y) 
+      return self.left.is_substitutable(x,y) and self.right.is_substitutable(x,y) 
 
     def substitution(self, var_x, a):
       return BinaryFormula(self.key, self.left.substitution(var_x, a), self.right.substitution(var_x, a))
 
     def get_values_x_substitution(self, var_x, formula):
       if not (isinstance(formula,BinaryFormula) and self.key==formula.key):
         return set()
@@ -135,15 +135,15 @@
             string = '\\lnot ' + self.formula.toLatex()
         else:
             string = '\\lnot({})'.format(self.formula.toLatex())
         return string   
 
     def toString(self, parentheses= False):
         if parentheses:
-            string = '(~' + self.formula.toString()+')'
+            string = '(~' + self.formula.toString(parentheses=parentheses)+')'
         elif not isinstance(self.formula, BinaryFormula):
             string = '~' + self.formula.toString()
         else:
             string = '~({})'.format(self.formula.toString())
         return string 
 
     def all_variables(self):
@@ -152,15 +152,15 @@
     def bound_variables(self):
       return self.all_variables().difference(self.free_variables())
 
     def free_variables(self):
       return self.formula.free_variables()
 
     def is_substitutable(self, x, y):
-      return self.formula.substitutable(x,y)
+      return self.formula.is_substitutable(x,y)
 
     def substitution(self, var_x, a):
       return NegationFormula(self.formula.substitution(var_x, a))
 
     def get_values_x_substitution(self, var_x, formula):
       values = set()
       if not isinstance(formula,NegationFormula):
@@ -298,15 +298,15 @@
 
         return self.forAll == other.forAll and self.variable == other.variable and self.formula == other.formula
     
     def __ne__(self, other): 
         if not isinstance(other, QuantifierFormula):
             return NotImplemented
 
-        return self.forAll != other.forAll and self.variable != other.variable and self.formula != other.formula
+        return self.forAll != other.forAll or self.variable != other.variable or self.formula != other.formula
 
     def __hash__(self):
       return hash(self.toString())
 
     def is_universal(self):
       return self.forAll
 
@@ -363,14 +363,16 @@
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
@@ -624,14 +626,20 @@
 
 def is_countermodel(premises, conclusion,u,s,preds):
   for p in premises:
     if not sat(p, u,s,preds):
       return False
   return False if sat(conclusion, u, s,preds) else True
 
+def is_valid_interpretation(premises, conclusion,u,s,preds):
+  for p in premises:
+    if not sat(p, u,s,preds):
+      return False
+  return sat(conclusion, u, s,preds)
+
 
 def sat(formula, u, s, preds):
   """" Função que testa se uma fórmula f é satisfeita em um interpretação com o universo u, predicados preds e interpretação de variáveis s.
   """
   if isinstance(formula, PredicateFormula):
     arity = len(formula.variables)
     if not (formula.name, arity) in preds.keys():
@@ -736,15 +744,15 @@
   else:   
     for f in premises:
       df[f.toString(parentheses=parentheses)] = [v_bar(f,v) for v in vs]
   df[formula.toString(parentheses=parentheses)] = [v_bar(formula,v) for v in vs]
 #  df_columns = sorted(df.columns,key=len)
   df = df.reindex(columns=sorted(df.columns,key=len))
  # df.columns = df_columns  
-  df.head().style.hide_index()
+  df.head().style.hide(axis='index')
   return df
 
 def consequence_logic(formula, premises=[], show_subformulas=True,parentheses=False):
   df_truth_table = truth_table(formula, premises=premises, show_subformulas=show_subformulas,parentheses=parentheses)
   df_true = df_truth_table
   for p in premises:
     df_true = df_true[df_true[p.toString(parentheses=parentheses)]==1]
```

### Comparing `logic4py-0.0.5/src/logic4py/lexer.py` & `logic4py-0.0.6/src/logic4py/lexer.py`

 * *Files identical despite different names*

### Comparing `logic4py-0.0.5/src/logic4py/logic_gui.py` & `logic4py-0.0.6/src/logic4py/logic_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import ipywidgets as widgets
 from IPython.display import display, Markdown, HTML
 from logic4py.parser_formula import get_formula
 from logic4py.parser_theorem import get_theorem
 from logic4py.parser_def_formula import check_proof
-from logic4py.formula import get_atoms, v_bar, get_vs, consequence_logic, truth_table, is_falsiable, is_unsatisfiable, is_satisfiable, is_valid, sat, is_countermodel, get_signature_predicates, get_propositional_atoms, get_signature_propositional_atoms
+from logic4py.formula import get_atoms, v_bar, get_vs, consequence_logic, truth_table, is_falsiable, is_unsatisfiable, is_satisfiable, is_valid, sat, is_countermodel, get_signature_predicates, get_propositional_atoms, get_signature_propositional_atoms, is_valid_interpretation
 from logic4py.decoder import decode_fo_interpretation
 from logic4py.example_reasoning import EXAMPLES
 from random import randrange
 import traceback
 from graphviz import Digraph
 
 def visualiza_relacao(A, R, labelSet=""):
@@ -635,14 +635,15 @@
       result = (s.split("@@"))[-1]
       print (f'{result}')
   else:
       pass
 
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       erro = False
       if(is_satisfiable(formula)!=cSat.value):
         erro = True
         display(HTML(r'<b><font color="red">Revise a sua reposta sobre satisfatível.</font>'))  
       if(is_valid(formula)!=cVal.value):
         erro = True
@@ -673,19 +674,20 @@
   wButtons = widgets.HBox([run, cParentheses, cSubformulas])
   
   display(HTML(r'<b>Digite sua fórmula para gerar a Tabela-Verdade:'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       try:
           formula = get_formula(input.value)
           if(formula!=None):
-              display(truth_table(formula, show_subformulas=cSubformulas.value,parentheses=cParentheses.value).style.hide_index())
+              display(truth_table(formula, show_subformulas=cSubformulas.value,parentheses=cParentheses.value).style.hide(axis='index'))
           else:
             display(HTML(r'<b><font color="red">A definição da fórmula não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ P | P & Q | P | Q | P -> Q | P <-> Q | (P), onde P,Q (em caixa alta) são átomos.</font>'))
       except ValueError:
           s = traceback.format_exc()
           result = (s.split("@@"))[-1]
           print (f'{result}')
       else:
@@ -719,14 +721,15 @@
       result = (s.split("@@"))[-1]
       print (f'{result}')
   else:
       pass
 
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       if(v_bar(formula,v)!=cTrue.value):
         erro = True
         display(HTML(r'<b><font color="red">Você errou, revise a sua reposta.</font>'))  
       else:
         display(HTML(r'<b><font color="blue">Parabéns, você acertou todas as respostas!</font>'))
       if response!='':
@@ -749,24 +752,25 @@
   wButtons = widgets.HBox([run, cParentheses, cSubformulas, cTabelaVerdade])
   
   display(HTML(r'<b>Digite seu teorema:'))
   display(input, wButtons, output)
 
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       try:
           premises, conclusion = get_theorem(input.value)
           if(conclusion!=None):
               result= consequence_logic(conclusion,premises=premises)
               if(result==None):
                 display(HTML(r'<b><font color="blue">O teorema é válido!</font>'))
                 if(cTabelaVerdade.value):
                   df = truth_table(conclusion,premises=premises, show_subformulas=cSubformulas.value,parentheses=cParentheses.value)
-                  display(df.style.hide_index())
+                  display(df.style.hide(axis='index'))
               else:
                 display(HTML(fr'<b><font color="red">O teorema é inválido. A linha {result} da Tabela-Verdade abaixo é um contraexemplo.</font>'))  
                 df = truth_table(conclusion,premises=premises, show_subformulas=cSubformulas.value,parentheses=cParentheses.value)                
                 display(df)
           else:
             display(HTML(r'<b><font color="red">A definição do teorema não está correta, verifique se todas regras foram aplicadas corretamente. Lembre-se que uma fórmula é definida pela seguinte BNF: F :== P | ~ F | F & F | F | F | F -> F | F <-> F | (F), onde P (em caixa alta) é um átomo e F é uma fórmula qualquer. Um Teorema é forma por uma lista de fórmula, |= e uma fórmula.</font>'))
       except ValueError:
@@ -841,30 +845,31 @@
 
       if len(s)>0:
         if language_pt:
           display(HTML(fr'<b>- Variáveis:</b> {", ".join(["<b>"+x_key+"</b>="+x_values for x_key, x_values in s.items()])}'))
         else:
           display(HTML(fr'<b>- Variables:</b> {", ".join(["<b>"+x_key+"</b>="+x_values for x_key, x_values in s.items()])}'))
       if language_pt:
-        display(HTML(fr'<b>Marque as fórmulas abaixo que são verdadeiras para o grafo acima:</b>'))
+        display(HTML(fr'<b>Marque as fórmulas abaixo que são verdadeiras para a interpretação acima:</b>'))
       else:
-        display(HTML(fr'<b>Check the formulas below which are true for the above graph:</b>'))
+        display(HTML(fr'<b>Check the formulas below which are true for the above interpretation:</b>'))
       display(*tuple(cFormulas + [run, output]))
       l_formulas = [get_formula(f) for f in formulas]
   except ValueError:
       if language_pt:
         display(HTML(r'<b><font color="red">A definição de alguma das fórmulas não está correta</font>'))
       s = traceback.format_exc()
       result = (s.split("@@"))[-1]
       print (f'{result}')
   else:
       pass
 
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       erro = False
       erro_formulas = []
       formulas_sat = [sat(f,universe,s,preds) for f in l_formulas]
       
       for i in range(len(formulas)):
         if formulas_sat[i]!=cFormulas[i].value:
@@ -881,44 +886,50 @@
           display(HTML(r'<b><font color="red">Você errou as seguintes fórmulas:</font></b>'))  
         else:
           display(HTML(r'<b><font color="red">You got wrong the following fórmulas:</font></b>'))  
         s_formulas = '<br> '.join(erro_formulas)
         display(HTML(f'{s_formulas}'))  
   run.on_click(on_button_run_clicked)
 
-def display_graph_truth_formulas(formulas, arcs, universe=None, s={}, parentheses=False, language_pt=True):
+def display_graph_truth_formulas(formulas, edges, universe=None, s={}, parentheses=False, language_pt=True):
   run = widgets.Button(description="Verificar") if language_pt else widgets.Button(description="Check")
   cFormulas = [widgets.Checkbox(value=False, description=f) for f in formulas]
   output = widgets.Output()
   
   try:
       preds={}
-      preds['E',2]= arcs
+      preds['E',2]= edges
       if language_pt:
         display(HTML(fr'<b>Considere o seguinte grafo:'))
       else:
         display(HTML(fr'<b>Consider the following graph:'))
         
       if universe==None:
         universe = set()
-        for (x,y) in arcs:
+        for (x,y) in edges:
           universe.add(x)
           universe.add(y)      
           
       if language_pt:
         display(HTML(fr"- <b>Conjunto universo:</b> {'{'+', '.join(sorted(list(universe)))+'}'}"))
       else:
         display(HTML(fr"- <b>Universe set:</b> {'{'+', '.join(sorted(list(universe)))+'}'}"))
+      for p_key, p_values in preds.items():
+        s_values = '{'+', '.join(['('+','.join([k for k in r])+')' if type(r)==tuple else '('+r+')' for r in sorted(list(p_values))])+'}'
+        if language_pt:
+          display(HTML(fr'<b>- Arcos {p_key[0]}</b>= {s_values}')) 
+        else:
+          display(HTML(fr'<b>- Edges {p_key[0]}=</b> {s_values}')) 
 
-      display(visualiza_relacao(universe, arcs))
       if len(s)>0:
         if language_pt:
           display(HTML(fr'<b>- <b>Variáveis:</b> {", ".join([x_key+"="+x_values for x_key, x_values in s.items()])}'))
         else:
           display(HTML(fr'<b>- <b>Variables:</b> {", ".join([x_key+"="+x_values for x_key, x_values in s.items()])}'))
+      display(visualiza_relacao(universe, edges))
       if language_pt:
         display(HTML(fr'<b>Marque as fórmulas abaixo que são verdadeiras para o grafo acima:'))
       else:
         display(HTML(fr'<b>Check the formulas below which are true for the above graph:'))
 
       display(*tuple(cFormulas + [run, output]))
       l_formulas = [get_formula(f) for f in formulas]
@@ -929,14 +940,15 @@
       result = (s.split("@@"))[-1]
       print (f'{result}')
   else:
       pass
 
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       erro = False
       erro_formulas = []
       formulas_sat = [sat(f,universe,s,preds) for f in l_formulas]
       
       for i in range(len(formulas)):
         if formulas_sat[i]!=cFormulas[i].value:
@@ -1011,14 +1023,15 @@
         input_string += "\n# Set the variables:"
       for x in free_variables:
         input_string+=f"\n{x} = "
     input.value = input_string
   display(input, run, output)
   def on_button_run_clicked(_):
     output.clear_output()
+    run.disabled=True
     with output:
       try:
         universe, preds, s  = decode_fo_interpretation(input.value)
         if is_countermodel(premises,conclusion,universe,s, preds):
           if language_pt:
             display(HTML(fr'<b><font color="blue">Parabéns, a interpretração acima é um contraexemplo para o teorema {input_theorem}!</font>'))
           else:
@@ -1031,14 +1044,75 @@
       except ValueError as error:
         display(HTML(fr'<b><font color="red">{error}</font>'))   
       else:
           pass
   run.on_click(on_button_run_clicked)
 
 
+def display_valid_model_decoder(input_theorem, input_interpretation = '', height_layout='140px', language_pt=True):
+  layout = widgets.Layout(width='90%', height=height_layout)
+  output = widgets.Output()
+  run = widgets.Button(description="Verificar" if language_pt else "Check")
+  input = widgets.Textarea(
+      value=input_interpretation,
+      placeholder='Digite a interpretação' if language_pt else 'Enter the interpretation',
+      description='',
+      layout=layout
+      )
+  if language_pt:
+    display(HTML(fr'<b>Apresente uma interpretação para o teorema {input_theorem} que torne verdadeira a conclusão e cada uma das premissas.'))
+  else:
+    display(HTML(fr'<b>Define an interpretation for the theorem {input_theorem} that the conclusion and every premise are true.')) 
+  premises, conclusion = get_theorem(input_theorem)
+  signature_preds = get_signature_predicates(conclusion, premises)
+  l_preds = sorted(list(signature_preds.keys()))
+  if input_interpretation=='':
+    if language_pt:
+      input_string = "# Defina o conjunto universo:\nU = {}\n# Defina os predicados:"
+    else: 
+      input_string = "# Set the universe set:\nU = {}\n# Set the Predicates:"
+    for p in l_preds:
+        for arity in signature_preds[p]:
+          input_string+=f"\n{p} = "+"{("+','.join([' ' for x in range(arity)])+")}"
+    free_variables = conclusion.free_variables()
+    for prem in premises:
+      free_variables = free_variables.union(prem.free_variables())
+    free_variables=sorted(list(free_variables))
+    if len(free_variables)>0:
+      if language_pt:
+        input_string += "\n# Defina as variáveis:"
+      else: 
+        input_string += "\n# Set the variables:"
+      for x in free_variables:
+        input_string+=f"\n{x} = "
+    input.value = input_string
+  display(input, run, output)
+  def on_button_run_clicked(_):
+    output.clear_output()
+    run.disabled=True
+    with output:
+      try:
+        universe, preds, s  = decode_fo_interpretation(input.value)
+        if is_valid_interpretation(premises,conclusion,universe,s, preds):
+          if language_pt:
+            display(HTML(fr'<b><font color="blue">Parabéns, a interpretração acima é uma interpretação válida para o teorema {input_theorem}!</font>'))
+          else:
+            display(HTML(fr'<b><font color="blue">Congratulations, the interpretation is a valid interpretation for the theorem {input_theorem}!</font>'))              
+        else:
+          if language_pt:
+            display(HTML(fr'<b><font color="red">Infelizmente, você errou a questão! A interpretação não é uma interpretação válida para o teorema {input_theorem}!</font>'))  
+          else:
+            display(HTML(fr'<b><font color="red">Unfortunately, you got the question wrong. The interpretation is not a valid interpretation for the theorem {input_theorem}!</font>'))  
+      except ValueError as error:
+        display(HTML(fr'<b><font color="red">{error}</font>'))   
+      else:
+          pass
+  run.on_click(on_button_run_clicked)
+
+
 def display_countermodel(input_theorem, language_pt=True):
   output = widgets.Output()
   output_interpretation = widgets.Output()
   output_variables = widgets.Output()
   output_run = widgets.Output()
   output_result = widgets.Output()
   layout = widgets.Layout(width='70%')
```

### Comparing `logic4py-0.0.5/src/logic4py/parser_def_formula.py` & `logic4py-0.0.6/src/logic4py/parser_def_formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 
 
 
 class ParserDefFormula():
     ERROR_NUM_NOT_DEFINED_BEFORE = 1
     ERROR_NUM_LINE_IS_ALREADY_DEFINED = 2
     ERROR_FORMULA_IS_NOT_VALID_FOR_RULE = 3
+    ERROR_FORMULA_IS_NOT_VALID_FOR_RULE_BINARY = 4
     def __init__(self, state):
         self.state = state
         self.pg = ParserGenerator(
             # A list of all token names accepted by the parser.
             ['NUM', 'DOT', 'COMMA', 'OPEN_PAREN', 'CLOSE_PAREN', 'NOT',
              'AND', 'OR',  'BOTTOM','ATOM', 'IMPLIE', 'IFF',
              'VAR','EXT','ALL',
@@ -244,14 +245,29 @@
                       is_binary=True
                       break
                 if is_binary:
                   self.symbol_table[number_line] = [formula]
                 else:
                   self.set_error(ParserDefFormula.ERROR_FORMULA_IS_NOT_VALID_FOR_RULE, line_error, formula.toString())
 
+        @self.pg.production('step : NUM DOT formula DEF_AND NUM')
+        @self.pg.production('step : NUM DOT formula DEF_OR NUM')
+        @self.pg.production('step : NUM DOT formula DEF_IMPLIE NUM')
+        @self.pg.production('step : NUM DOT formula DEF_IFF NUM')
+        def step(p):
+            number_line = p[0].value
+            formula = p[2][1]
+
+            source_position = p[0].getsourcepos()
+            line_error = source_position.lineno
+
+            self.symbol_table[number_line] = [formula]
+            self.set_error(ParserDefFormula.ERROR_FORMULA_IS_NOT_VALID_FOR_RULE_BINARY, line_error, number_line)
+            return
+
 
         @self.pg.production('formula : EXT formula')
         @self.pg.production('formula : ALL formula')
         @self.pg.production('formula : formula OR formula')
         @self.pg.production('formula : formula AND formula')
         @self.pg.production('formula : formula IMPLIE formula')
         @self.pg.production('formula : formula IFF formula')
@@ -352,14 +368,16 @@
         productions = self.state.splitlines()
         if type == ParserDefFormula.ERROR_NUM_LINE_IS_ALREADY_DEFINED:
             self.error['messages'].append("A linha {} utiliza uma mesma numeração que já foi definida anteriormente a linha {}:\n  {}".format(token_error, line_error, productions[line_error-1]))
         elif type == ParserDefFormula.ERROR_NUM_NOT_DEFINED_BEFORE:
             self.error['messages'].append("A linha {} não foi definida anteriormente a linha {}:\n  {}".format(token_error, line_error, productions[line_error-1]))
         elif type == ParserDefFormula.ERROR_FORMULA_IS_NOT_VALID_FOR_RULE:
             self.error['messages'].append("A fórmula {} na linha {} não é uma conclusão válida para a regra definida com a linha referenciada:\n  {}".format(token_error, line_error, productions[line_error-1]))
+        elif type == ParserDefFormula.ERROR_FORMULA_IS_NOT_VALID_FOR_RULE_BINARY:
+            self.error['messages'].append("A fórmula {} na linha {} é uma fórmula com conectivo binário e portanto devem ser referenciada duas linhas:\n  {}".format(token_error, line_error, productions[line_error-1]))
             
     def get_parser(self):
         return self.pg.build()
 
     @staticmethod
     def getProof(input_text=''):
       lexer = Lexer().get_lexer()
```

### Comparing `logic4py-0.0.5/src/logic4py/parser_formula.py` & `logic4py-0.0.6/src/logic4py/parser_formula.py`

 * *Files identical despite different names*

### Comparing `logic4py-0.0.5/src/logic4py/parser_theorem.py` & `logic4py-0.0.6/src/logic4py/parser_theorem.py`

 * *Files identical despite different names*

### Comparing `logic4py-0.0.5/src/logic4py.egg-info/PKG-INFO` & `logic4py-0.0.6/src/logic4py.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logic4py
-Version: 0.0.5
+Version: 0.0.6
 Summary: logic4py is a libray for teaching logic to computer science students.
 Home-page: https://github.com/daviromero/logic4py
 Author: Davi Romero de Vasconcelos
 Author-email: daviromero@ufc.br
 License: MIT
 Keywords: Propositional Logic,First-Order Logia,Teaching Logic,Educational Software
 Platform: UNKNOWN
```

