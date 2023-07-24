# Comparing `tmp/yargy-0.8.0-py2.py3-none-any.whl.zip` & `tmp/yargy-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,47 @@
-Zip file size: 22020 bytes, number of entries: 17
--rw-rw-r--  2.0 unx    35106 b- defN 17-Apr-16 08:24 yargy/tests.py
--rw-rw-r--  2.0 unx     2524 b- defN 17-Apr-16 08:24 yargy/normalization.py
--rw-rw-r--  2.0 unx    10011 b- defN 17-Apr-16 08:24 yargy/labels.py
--rw-rw-r--  2.0 unx    11407 b- defN 17-Apr-16 08:24 yargy/parser.py
--rw-rw-r--  2.0 unx     9947 b- defN 17-Apr-16 08:24 yargy/tokenizer.py
--rw-rw-r--  2.0 unx      160 b- defN 17-Apr-16 08:24 yargy/morph.py
--rw-rw-r--  2.0 unx     4224 b- defN 17-Apr-16 08:24 yargy/interpretation.py
--rw-rw-r--  2.0 unx      133 b- defN 17-Apr-16 09:13 yargy/__init__.py
--rw-rw-r--  2.0 unx      403 b- defN 17-Apr-16 08:24 yargy/compat.py
--rw-rw-r--  2.0 unx     1239 b- defN 17-Apr-16 08:24 yargy/utils.py
--rw-rw-r--  2.0 unx     7257 b- defN 17-Apr-16 08:24 yargy/pipeline.py
--rw-rw-r--  2.0 unx       10 b- defN 17-Apr-16 11:52 yargy-0.8.0.dist-info/DESCRIPTION.rst
--rw-rw-r--  2.0 unx      981 b- defN 17-Apr-16 11:52 yargy-0.8.0.dist-info/metadata.json
--rw-rw-r--  2.0 unx        6 b- defN 17-Apr-16 11:52 yargy-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      113 b- defN 17-Apr-16 11:52 yargy-0.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx      841 b- defN 17-Apr-16 11:52 yargy-0.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx     1300 b- defN 17-Apr-16 11:52 yargy-0.8.0.dist-info/RECORD
-17 files, 85662 bytes uncompressed, 19954 bytes compressed:  76.7%
+Zip file size: 33754 bytes, number of entries: 45
+-rw-rw-r--  2.0 unx     2348 b- defN 17-Aug-25 11:16 yargy/token.py
+-rw-rw-r--  2.0 unx       30 b- defN 17-Aug-25 11:16 yargy/relations.py
+-rw-rw-r--  2.0 unx      931 b- defN 17-Aug-25 11:16 yargy/coreference.py
+-rw-rw-r--  2.0 unx     7084 b- defN 17-Aug-25 11:16 yargy/pipelines.py
+-rw-rw-r--  2.0 unx     8266 b- defN 17-Aug-29 19:35 yargy/parser.py
+-rw-rw-r--  2.0 unx       72 b- defN 17-Sep-12 15:18 yargy/__init__.py
+-rw-rw-r--  2.0 unx     3979 b- defN 17-Sep-29 18:17 yargy/tokenizer.py
+-rw-rw-r--  2.0 unx     2446 b- defN 17-Sep-21 15:31 yargy/morph.py
+-rw-rw-r--  2.0 unx      879 b- defN 17-Aug-25 11:16 yargy/visitor.py
+-rw-rw-r--  2.0 unx     1822 b- defN 17-Aug-25 11:16 yargy/api.py
+-rw-rw-r--  2.0 unx     2343 b- defN 17-Aug-29 19:35 yargy/utils.py
+-rw-rw-r--  2.0 unx       31 b- defN 17-Aug-25 11:16 yargy/predicates.py
+-rw-rw-r--  2.0 unx      433 b- defN 17-Sep-21 15:31 yargy/compat.py
+-rw-rw-r--  2.0 unx     3260 b- defN 17-Aug-25 11:16 yargy/dot.py
+-rw-rw-r--  2.0 unx     5187 b- defN 17-Sep-21 15:31 yargy/rule/constructors.py
+-rw-rw-r--  2.0 unx      237 b- defN 17-Aug-25 11:16 yargy/rule/__init__.py
+-rw-rw-r--  2.0 unx     6200 b- defN 17-Aug-29 19:35 yargy/rule/transformators.py
+-rw-rw-r--  2.0 unx     6517 b- defN 17-Aug-25 11:16 yargy/rule/bnf.py
+-rw-rw-r--  2.0 unx      436 b- defN 17-Aug-25 11:41 yargy/tests/test_tokenizer.py
+-rw-rw-r--  2.0 unx     1132 b- defN 17-Aug-25 12:33 yargy/tests/test_pipeline.py
+-rw-rw-r--  2.0 unx        0 b- defN 17-Aug-25 11:19 yargy/tests/__init__.py
+-rw-rw-r--  2.0 unx     1571 b- defN 17-Aug-25 11:16 yargy/tests/test_person.py
+-rw-rw-r--  2.0 unx     4882 b- defN 17-Sep-29 18:17 yargy/interpretation/interpretator.py
+-rw-rw-r--  2.0 unx      267 b- defN 17-Sep-21 15:31 yargy/interpretation/__init__.py
+-rw-rw-r--  2.0 unx     1149 b- defN 17-Sep-29 18:17 yargy/interpretation/normalizer.py
+-rw-rw-r--  2.0 unx     3212 b- defN 17-Sep-29 18:17 yargy/interpretation/attribute.py
+-rw-rw-r--  2.0 unx     5891 b- defN 17-Sep-29 18:17 yargy/interpretation/fact.py
+-rw-rw-r--  2.0 unx     2287 b- defN 17-Aug-25 11:16 yargy/relation/constructors.py
+-rw-rw-r--  2.0 unx      137 b- defN 17-Aug-25 11:16 yargy/relation/__init__.py
+-rw-rw-r--  2.0 unx     4069 b- defN 17-Aug-25 11:16 yargy/relation/graph.py
+-rw-rw-r--  2.0 unx     2038 b- defN 17-Aug-25 11:16 yargy/relation/bank.py
+-rw-rw-r--  2.0 unx     2230 b- defN 17-Aug-25 11:16 yargy/tree/constructors.py
+-rw-rw-r--  2.0 unx       85 b- defN 17-Aug-25 11:16 yargy/tree/__init__.py
+-rw-rw-r--  2.0 unx     2994 b- defN 17-Aug-25 11:16 yargy/tree/transformators.py
+-rw-rw-r--  2.0 unx     1618 b- defN 17-Aug-25 11:16 yargy/predicate/constructors.py
+-rw-rw-r--  2.0 unx      193 b- defN 17-Aug-25 11:16 yargy/predicate/__init__.py
+-rw-rw-r--  2.0 unx      704 b- defN 17-Aug-25 11:16 yargy/predicate/base.py
+-rw-rw-r--  2.0 unx      890 b- defN 17-Aug-25 11:16 yargy/predicate/relation.py
+-rw-rw-r--  2.0 unx     7369 b- defN 17-Sep-21 15:31 yargy/predicate/bank.py
+-rw-rw-r--  2.0 unx       10 b- defN 17-Sep-30 23:07 yargy-0.9.0.dist-info/DESCRIPTION.rst
+-rw-rw-r--  2.0 unx      993 b- defN 17-Sep-30 23:07 yargy-0.9.0.dist-info/metadata.json
+-rw-rw-r--  2.0 unx        6 b- defN 17-Sep-30 23:07 yargy-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      110 b- defN 17-Sep-30 23:07 yargy-0.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      853 b- defN 17-Sep-30 23:07 yargy-0.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx     3612 b- defN 17-Sep-30 23:07 yargy-0.9.0.dist-info/RECORD
+45 files, 100803 bytes uncompressed, 28142 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -1,52 +1,136 @@
-Filename: yargy/tests.py
+Filename: yargy/token.py
 Comment: 
 
-Filename: yargy/normalization.py
+Filename: yargy/relations.py
 Comment: 
 
-Filename: yargy/labels.py
+Filename: yargy/coreference.py
+Comment: 
+
+Filename: yargy/pipelines.py
 Comment: 
 
 Filename: yargy/parser.py
 Comment: 
 
+Filename: yargy/__init__.py
+Comment: 
+
 Filename: yargy/tokenizer.py
 Comment: 
 
 Filename: yargy/morph.py
 Comment: 
 
-Filename: yargy/interpretation.py
+Filename: yargy/visitor.py
 Comment: 
 
-Filename: yargy/__init__.py
+Filename: yargy/api.py
+Comment: 
+
+Filename: yargy/utils.py
+Comment: 
+
+Filename: yargy/predicates.py
 Comment: 
 
 Filename: yargy/compat.py
 Comment: 
 
-Filename: yargy/utils.py
+Filename: yargy/dot.py
+Comment: 
+
+Filename: yargy/rule/constructors.py
+Comment: 
+
+Filename: yargy/rule/__init__.py
+Comment: 
+
+Filename: yargy/rule/transformators.py
+Comment: 
+
+Filename: yargy/rule/bnf.py
+Comment: 
+
+Filename: yargy/tests/test_tokenizer.py
+Comment: 
+
+Filename: yargy/tests/test_pipeline.py
+Comment: 
+
+Filename: yargy/tests/__init__.py
+Comment: 
+
+Filename: yargy/tests/test_person.py
+Comment: 
+
+Filename: yargy/interpretation/interpretator.py
+Comment: 
+
+Filename: yargy/interpretation/__init__.py
+Comment: 
+
+Filename: yargy/interpretation/normalizer.py
+Comment: 
+
+Filename: yargy/interpretation/attribute.py
+Comment: 
+
+Filename: yargy/interpretation/fact.py
+Comment: 
+
+Filename: yargy/relation/constructors.py
+Comment: 
+
+Filename: yargy/relation/__init__.py
+Comment: 
+
+Filename: yargy/relation/graph.py
+Comment: 
+
+Filename: yargy/relation/bank.py
+Comment: 
+
+Filename: yargy/tree/constructors.py
+Comment: 
+
+Filename: yargy/tree/__init__.py
+Comment: 
+
+Filename: yargy/tree/transformators.py
+Comment: 
+
+Filename: yargy/predicate/constructors.py
+Comment: 
+
+Filename: yargy/predicate/__init__.py
+Comment: 
+
+Filename: yargy/predicate/base.py
+Comment: 
+
+Filename: yargy/predicate/relation.py
 Comment: 
 
-Filename: yargy/pipeline.py
+Filename: yargy/predicate/bank.py
 Comment: 
 
-Filename: yargy-0.8.0.dist-info/DESCRIPTION.rst
+Filename: yargy-0.9.0.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: yargy-0.8.0.dist-info/metadata.json
+Filename: yargy-0.9.0.dist-info/metadata.json
 Comment: 
 
-Filename: yargy-0.8.0.dist-info/top_level.txt
+Filename: yargy-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: yargy-0.8.0.dist-info/WHEEL
+Filename: yargy-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: yargy-0.8.0.dist-info/METADATA
+Filename: yargy-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: yargy-0.8.0.dist-info/RECORD
+Filename: yargy-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yargy/parser.py

```diff
@@ -1,349 +1,275 @@
 # coding: utf-8
 from __future__ import unicode_literals
 
-from copy import deepcopy, copy
 from threading import Lock
+from collections import defaultdict
+
 from intervaltree import IntervalTree
 
-from yargy.tokenizer import Token, Tokenizer
-from yargy.pipeline import PipelineStatus
-from yargy.normalization import NormalizationType
-from yargy.utils import get_tokens_position
+from yargy.compat import str
+from .utils import Record
+from .token import get_tokens_span
+from .tree import (
+    Node,
+    InterpretationNode,
+    Leaf,
+    Tree
+)
+from .tokenizer import Tokenizer
+from .predicate import is_relation_predicate
+from .relation import Graph as Relations
+from .rule.bnf import is_rule
+
+
+class Chart(object):
+    def __init__(self, tokens):
+        self.tokens = list(tokens)
+
+        self.columns = [Column(0, None)]
+        for index, token in enumerate(self.tokens, 1):
+            self.columns.append(Column(index, token))
+
+    def matches(self, rule):
+        for column in self.columns:
+            for state in column:
+                if state.completed and id(state.rule) == id(rule):
+                    yield state
 
+    def __iter__(self):
+        return iter(self.columns)
 
-def create_or_copy_grammar(grammar, name=None):
-    if isinstance(grammar, list):
-        grammar = Grammar(name, deepcopy(grammar))
-    elif isinstance(grammar, (Operation, Grammar)):
-        grammar = deepcopy(grammar)
-    else:
-        raise ValueError('Not supported grammar type: {}'.format(grammar))
-    return grammar
+    def __getitem__(self, index):
+        return self.columns[index]
 
+    def __len__(self):
+        return len(self.columns)
 
-def build_grammars_from_multiple_classes(classes):
-    for _class in classes:
-        _class_name = _class.__name__
-        for rule in _class.__members__.values():
-            name = '{0}__{1}'.format(_class_name, rule.name)
-            yield rule, name, create_or_copy_grammar(rule.value, name)
-
-
-class Stack(list):
-
-    '''
-    Special list for grammar, which holds matches with rule index
-    (by which token was captured)
-    '''
-
-    def have_matches_by_rule_index(self, rule_index):
-        '''
-        Checks that stack contains matches by rule index
-        '''
-        return any(
-            (rule == rule_index for (rule, _) in reversed(self))
+    def __repr__(self):
+        return 'Chart({columns!r}, ...)'.format(
+            columns=self.columns
         )
 
-    def flatten(self):
-        '''
-        Returns matched tokens without rule indexes
-        '''
-        return [value for (_, value) in self]
-
-
-class Operation(object):
-
-    def __init__(self, *grammars):
-        self.matches = []
-        self.grammars = [
-            create_or_copy_grammar(grammar) 
-            for grammar in grammars
-        ]
-        self.working = self.grammars
- 
-    def reset(self):
-        self.matches = []
-        self.working = self.grammars
-        for grammar in self.working:
-            if grammar.stack:
-                grammar.reset()
-
-    def shift(self, token):
-        recheck = any([
-            grammar.shift(token)
-            for grammar in self.working
-        ])
-        self.update_working()
-        return recheck or bool(self.matches and not self.working)
-
-    def reduce(self, end_of_stream=False):
-        for grammar in self.working:
-            match = grammar.reduce(end_of_stream=end_of_stream)
-            if match:
-                self.matches.append(match)
-        self.update_working()
-        if self.matches and (not self.working or end_of_stream):
-            match = max(self.matches, key=len)
-            self.reset()
-            return match
-
-    def update_working(self):
-        self.working = [
-            grammar for grammar in self.working
-            if grammar.active
-        ]
+    @property
+    def source(self):
+        for column in self.columns:
+            for line in column.source:
+                yield line
+            yield ''
+
+    def _repr_pretty_(self, printer, cycle):
+        for line in self.source:
+            printer.text(line)
+            printer.break_()
+
+
+class Column(object):
+    def __init__(self, index, token):
+        self.index = index
+        self.token = token
+        self.states = []
+        self.hashes = set()
+        self.states_index = defaultdict(list)
+
+    def __iter__(self):
+        return iter(self.states)
+
+    def append(self, state):
+        value = hash(state)
+        if value not in self.hashes:
+            self.hashes.add(value)
+            self.states.append(state)
+            self.update_index(state)
+
+    def update_index(self, state):
+        if not state.completed:
+            next_term = state.next_term
+            if is_rule(next_term):
+                self.states_index[id(next_term)].append(state)
+
+    def __repr__(self):
+        return 'Column({index!r}, {token!r}, ...)'.format(
+            index=self.index,
+            token=self.token
+        )
 
     @property
-    def active(self):
-        return bool(self.matches) or any(
-            grammar.active for grammar in self.working
+    def source(self):
+        yield '{index!r} {token!r}'.format(
+            index=self.index,
+            token=self.token
         )
+        yield '----------------'
+        for state in self.states:
+            yield str(state)
+
+    def _repr_pretty_(self, printer, cycle):
+        for line in self.source:
+            printer.text(line)
+            printer.break_()
+
+
+class State(object):
+    def __init__(self, rule, production, dot_index,
+                 start_column, stop_column, children,
+                 relations):
+        self.rule = rule
+        self.production = production
+        self.dot_index = dot_index
+        self.start_column = start_column
+        self.stop_column = stop_column
+        self.children = children
+        self.relations = relations
+
+    def __hash__(self):
+        return hash((
+            id(self.rule), id(self.production), self.dot_index,
+            self.start_column.index, self.stop_column.index
+        ))
 
+    @property
+    def completed(self):
+        return self.dot_index >= len(self.production.terms)
 
-class OR(Operation):
+    @property
+    def next_term(self):
+        return self.production.terms[self.dot_index]
 
-    pass
+    def __str__(self):
+        terms = self.production.terms
+        production = ' '.join(
+            [_.label for _ in terms[:self.dot_index]]
+            + ['$']
+            + [_.label for _ in terms[self.dot_index:]]
+        )
+        return '[{start}:{stop}] {name} -> {production}'.format(
+            start=self.start_column.index,
+            stop=self.stop_column.index,
+            name=self.rule.label,
+            production=production,
+        )
 
 
-class Grammar(object):
+class Match(Record):
+    __attributes__ = ['tokens', 'span']
 
-    '''
-    Grammar contains stack and list of rules.
-    When GLR-parser iterates over tokens it calls
-    `shift` & `reduce` methods on each grammar which checks
-    current grammar stack & provided token on current rule
-    when stack contents matches all rules - grammar returns stack,
-    which contains actual text match
-    '''
-
-    def __init__(self, name, rules):
-        self.name = name
-        self.rules = rules + [
-            {
-                'terminal': True,
-            },
-        ]
-        self.reset()
-
-    def shift(self, token, recheck=False):
-        '''
-        Parser <- [grammar_1, grammar_2]
-                   |
-                   V
-                shift(token_1)
-        Grammar_1 -> []
-        Grammar_2 -> [token_1]
-                   |
-                   V
-                shift(token_2)
-        Grammar_1 -> []
-        Grammar_2 -> [token_1, token_2]
-                   |
-                   V
-                reduce()
-        Grammar_1 -> []
-        Grammar_2 -> [] <-> returns stack [token_1, token_2]
-        '''
-        rule = self.rules[self.index]
-
-        # need to clone tokens, because labels can modify
-        # its forms or other attributes
-        token = copy(token)
-
-        if isinstance(rule, (Operation, Grammar)):
-            recheck = rule.shift(token)
-            if not rule.active:
-                rule.reset()
-                self.reset()
-            return recheck
-        else:
-            repeatable = rule.get('repeatable', False)
-            optional = rule.get('optional', False)
-            terminal = rule.get('terminal', False)
-            skip = rule.get('skip', False)
-            labels = rule.get('labels', [])
-
-            if terminal:
-                return True
-
-            if not all(self.match(token, labels)) and not terminal:
-                last_index = self.index
-                recheck = False
-                if optional or (repeatable and self.stack.have_matches_by_rule_index(self.index)):
-                    self.index += 1
-                else:
-                    recheck = True
-                    self.reset()
-
-                if (self.index != last_index) and (not recheck or (optional or repeatable)):
-                    # recheck current token on next rule
-                    return self.shift(token, recheck=recheck)
-                else:
-                    self.reset()
-            else:
-                # token matches current rule
-                if not terminal:
-                    # append token to stack if it's not a terminal rule and current rule
-                    # doesn't have 'skip' option
-                    if not skip:
-                        # add additional fields to tokens, like normalization
-                        # and interpretation rules
-                        token.normalization_type = rule.get(
-                            'normalization', NormalizationType.Normalized)
-                        token.interpretation = rule.get('interpretation', None)
-                        # finally append match to stack
-                        self.stack.append((self.index, token))
-                    if not repeatable:
-                        self.index += 1
-
-    def reduce(self, end_of_stream=False):
-        '''
-        Reduce method returns grammar stack if
-        current grammar index equals to last (terminal) rule
-        '''
-        current_rule = self.rules[self.index]
-        terminal_rule = self.rules[-1]
-
-        is_grammar_object = isinstance(current_rule, (Operation, Grammar))
-
-        if is_grammar_object and current_rule.active:
-            match = current_rule.reduce(end_of_stream=end_of_stream)
-            if match:
-                self.index += 1
-                current_rule = self.rules[self.index]
-                is_grammar_object = isinstance(current_rule, (Operation, Grammar))
-                for token in match.flatten():
-                    self.stack.append((self.index, token))
-
-        if (current_rule == terminal_rule) and self.stack:
-            match = self.stack
-            self.reset()
-            return match
-
-        if end_of_stream and not is_grammar_object:
-            is_repeatable_and_have_matches = (
-                current_rule.get('repeatable', False)
-                and
-                self.stack.have_matches_by_rule_index(self.index)
-            )
-            is_optional = current_rule.get('optional', False)
-            next_rule_is_terminal = (
-                self.rules[self.index + 1] == terminal_rule)
-            if (is_repeatable_and_have_matches or is_optional) and next_rule_is_terminal:
-                match = self.stack
-                self.reset()
-                return match
+    def __init__(self, rule, tree):
+        self.rule = rule
+        self.tree = tree
+        self.tokens = [_.token for _ in tree.walk(types=Leaf)]
+        self.span = get_tokens_span(self.tokens)
 
     @property
-    def active(self):
-        return bool(self.stack) or any(
-            rule.active for rule in self.rules
-            if isinstance(rule, (Operation, Grammar))
-        )
-
-    def reset(self):
-        self.stack = Stack()
-        self.index = 0
-        for rule in self.rules:
-            if isinstance(rule, (Operation, Grammar)):
-                rule.reset()
-
-    def match(self, token, labels):
-        stack = self.stack.flatten()
-        for label in labels:
-            yield label(token, stack)
+    def fact(self):
+        fact = self.tree.interpret()
+        return fact.normalized
 
-    def __copy__(self):
-        return Grammar(self.name, self.rules[:-1])
 
-    def __repr__(self):
-        return 'Grammar(name=\'{name}\', stack={stack})'.format(
-            name=self.name,
-            stack=self.stack,
-        )
+def prepare_node(rule, children):
+    if rule.interpretator:
+        return InterpretationNode(rule, children)
+    else:
+        return Node(rule, children)
 
 
 class Parser(object):
-
-    '''
-    Yet another GLR-parser.
-    '''
-
-    def __init__(self, grammars, tokenizer=None, pipelines=None, cache_size=0):
-        self.grammars = grammars
-        self.tokenizer = tokenizer or Tokenizer(cache_size=cache_size)
+    def __init__(self, rule, tokenizer=None, pipelines=None):
+        self.rule = rule.normalized.as_bnf.start
+        self.tokenizer = tokenizer or Tokenizer()
         self.pipelines = pipelines or []
         self.lock = Lock()
 
-    def extract(self, text, return_flatten_stack=True):
+    def chart(self, text):
         with self.lock:
-            stream = self.tokenizer.transform(text)
-            
+            stream = self.tokenizer(text)
+
             for pipeline in self.pipelines:
                 stream = pipeline(stream)
 
-            for token in stream:
-                for grammar in self.grammars:
-                    recheck = grammar.shift(token)
-                    match = grammar.reduce()
-
-                    if match:
-                        if return_flatten_stack:
-                            match = match.flatten()
-                        yield (grammar, match)
-
-                    if recheck:
-                        grammar.shift(token)
-                        match = grammar.reduce()
-
-                        if match:
-                            if return_flatten_stack:
-                                match = match.flatten()
-                            yield (grammar, match)
-
-            for grammar in self.grammars:
-                match = grammar.reduce(end_of_stream=True)
-                if match:
-                    if return_flatten_stack:
-                        match = match.flatten()
-                    yield (grammar, match)
-                grammar.reset()
-
-
-class Combinator(object):
-
-    '''
-    Combinator merges multiple grammars (in multiple enums) into one parser
-    '''
-
-    def __init__(self, classes, *args, **kwargs):
-        self.classes = {}
-        self.grammars = []
-        for rule, name, grammar in build_grammars_from_multiple_classes(classes):
-            self.classes[name] = rule
-            self.grammars.append(grammar)
-        self.parser = Parser(self.grammars, *args, **kwargs)
+            chart = Chart(stream)
+            for column in chart:
+                self.predict(column, self.rule)
+                for state in column:
+                    if state.completed:
+                        self.complete(column, state)
+                    else:
+                        next_term = state.next_term
+                        if is_rule(next_term):
+                            self.predict(column, next_term)
+                        elif column.index + 1 < len(chart):
+                            next_column = chart[column.index + 1]
+                            self.scan(next_column, next_term, state)
+            return chart
 
     def extract(self, text):
-        for (rule, match) in self.parser.extract(text):
-            yield self.classes[rule.name], match
+        chart = self.chart(text)
+        for state in chart.matches(self.rule):
+            root = prepare_node(self.rule, state.children)
+            tree = Tree(root).replace_token_forms(state.relations.nodes)
+            yield Match(self.rule, tree)
 
-    def resolve_matches(self, matches, strict=True):
-        # sort matches by tokens count in decreasing order
-        matches = sorted(matches, key=lambda m: len(m[1]), reverse=True)
+    def resolve(self, matches):
+        matches = sorted(matches, key=lambda _: len(_.tokens), reverse=True)
         tree = IntervalTree()
-        for (grammar, match) in matches:
-            start, stop = get_tokens_position(match)
-            exists = tree[start:stop]
-            if exists and not strict:
-                for interval in exists:
-                    exists_grammar, _ = interval.data
-                    exists_contains_current_grammar = (
-                        interval.begin < start and interval.end > stop)
-                    exists_grammar_with_same_type = isinstance(
-                        exists_grammar, grammar.__class__)
-                    if not exists_grammar_with_same_type and exists_contains_current_grammar:
-                        exists = False
-            if not exists:
-                tree[start:stop] = (grammar, match)
-                yield (grammar, match)
+        for match in matches:
+            start, stop = match.span
+            if not tree[start:stop]:
+                tree[start:stop] = match
+                yield match
+
+    def findall(self, text):
+        matches = self.extract(text)
+        return self.resolve(matches)
+
+    def match(self, text):
+        # NOTE Not an optimal implementation. Assume `match` is used
+        # not very often
+        for match in self.extract(text):
+            if match.span == (0, len(text)):
+                yield match
+
+    def predict(self, column, rule):
+        for production in rule.productions:
+            state = State(
+                rule, production,
+                dot_index=0,
+                start_column=column,
+                stop_column=column,
+                children=[],
+                relations=Relations()
+            )
+            column.append(state)
+
+    def scan(self, column, predicate, state):
+        token = column.token
+        if predicate(token):
+            relations = state.relations
+            if is_relation_predicate(predicate):
+                relations = relations.copy().add(token, predicate)
+                if not relations:
+                    return
+            node = Leaf(predicate, token)
+            state = State(
+                state.rule, state.production,
+                dot_index=state.dot_index + 1,
+                start_column=state.start_column,
+                stop_column=column,
+                children=state.children + [node],
+                relations=relations
+            )
+            column.append(state)
+
+    def complete(self, column, completed):
+        node = prepare_node(completed.rule, completed.children)
+        states = completed.start_column.states_index[id(completed.rule)]
+        for state in states:
+            relations = state.relations.copy().merge(completed.relations)
+            if relations:
+                state = State(
+                    state.rule, state.production,
+                    dot_index=state.dot_index + 1,
+                    start_column=state.start_column,
+                    stop_column=column,
+                    children=state.children + [node],
+                    relations=relations
+                )
+                column.append(state)
```

## yargy/tokenizer.py

```diff
@@ -1,292 +1,168 @@
 # coding: utf-8
 from __future__ import unicode_literals
 
 import re
-import sys
-import string
-import collections
-
-from pymorphy2.shapes import is_roman_number
-
-from yargy.morph import Analyzer
-from yargy.utils import frange, decode_roman_number
-from yargy.compat import range, lru_cache, RUNNING_ON_PYTHON_2_VERSION
-
-
-russian_token_regex = r'(?P<russian>[а-яё][а-яё\-]*)'
-latin_token_regex = r'(?P<latin>[a-z]\-?[a-z\']*)'
-int_separated_token_regex = r'(?P<int_separated>[1-9]\d*(\s\d{3})+)'
-int_range_token_regex = r'(?P<int_range>\d+\s*?[\-\—]\s*?\d+)'
-int_token_regex = r'(?P<int>[+-]?\d+)'
-float_range_token_regex = r'(?P<float_range>[\d]+[\.\,][\d]+\s*?[\-\—]\s*?[\d]+[\.\,][\d]+)'
-float_token_regex = r'(?P<float>[+-]?[\d]+[\.\,][\d]+)'
-quote_token_regex = r'(?P<quote>[\"\'\«\»\„\“])'
-punctuation_token_regex = string.punctuation.join(['(?P<punct>[\—', r'])'])
-email_token_regex = r'(?P<email>[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+)'
-phone_number_token_regex = r'(?P<phone>(\+)?([-\s_()]?\d[-\s_()]?){10,14})' # found at https://toster.ru/answer?answer_id=852265#answers_list_answer
-end_of_line_token_regex = r'(?P<end_of_line>[\n\r]+)'
-complete_token_regex = r'|'.join((
-    phone_number_token_regex,
-    email_token_regex,
-    float_range_token_regex,
-    float_token_regex,
-    int_separated_token_regex,
-    int_range_token_regex,
-    int_token_regex,
-    russian_token_regex,
-    latin_token_regex,
-    quote_token_regex,
-    punctuation_token_regex,
-    end_of_line_token_regex,
-))
-
-token_regex = re.compile(complete_token_regex, re.UNICODE | re.IGNORECASE)
-
-class Token(object):
-
-    __slots__ = (
-        'value',
-        'position',
-        'forms',
-        'normalization_type',
-        'interpretation',
-    )
-
-    def __init__(self, value, position, forms, normalization_type=None, interpretation=None):
-        self.value = value
-        self.position = position
-        self.forms = forms
-        self.normalization_type = normalization_type
-        self.interpretation = interpretation
-
-    def __hash__(self):
-        return hash(
-            self.value
-        )
-
-    def __eq__(self, other):
-        if not isinstance(other, Token):
-            return False
-        else:
-            return (
-                (self.value == other.value) &
-                (self.position == other.position) &
-                (self.forms == other.forms)
-            )
 
-    def __copy__(self):
-        return Token(
-            self.value,
-            self.position,
-            self.forms[:],
-            self.normalization_type,
-        )
+from .utils import Record, assert_type
+from .compat import string_type, long
+from .token import Token
+from .morph import Form, MORPH
+
+
+class TokenRule(Record):
+    __attributes__ = ['pattern', 'grammemes']
+
+    pattern = None
+    grammemes = set()
+
+    def construct(self, value):
+        return value
+
+    def normalize(self, value):
+        return value
+
+    def forms(self, value):
+        yield Form(self.normalize(value), self.grammemes)
+
+    def __call__(self, value, span):
+        value = self.construct(value)
+        forms = list(self.forms(value))
+        return Token(value, span, forms)
+
+
+class RussianRule(TokenRule):
+    # TODO Why does it differ from LatinRule pattern?
+    pattern = r'[а-яё]+'
+
+    def __init__(self, morph=MORPH):
+        self.morph = morph
+
+    def forms(self, value):
+        return self.morph.parse(value)
+
+
+class LatinRule(TokenRule):
+    pattern = r'[a-z]+'
+    grammemes = {'LATN'}
+
+    def normalize(self, value):
+        return value.lower()
+
+
+class StrInt(long):
+    def __new__(cls, string):
+        assert_type(string, string_type)
+        self = super(StrInt, cls).__new__(cls, string)
+        self.raw = string
+        return self
+
+    def __str__(self):
+        return self.raw
 
     def __repr__(self):
-        return '{0.__class__.__name__}({0.value!r}, {0.position!r}, {0.forms!r})'.format(self)
+        return self.raw
 
-class Tokenizer(object):
 
-    def __init__(self, pattern=token_regex, morph_analyzer=Analyzer, cache_size=0, frange_step=0.1):
-        self.pattern = pattern
-        self.morph = morph_analyzer
-        self.cache = lru_cache(maxsize=cache_size)(self.get_word_forms)
-        self.frange_step = frange_step
-
-    def get_word_forms(self, word):
-        forms = []
-        for form in self.morph.parse(word):
-            token = {}
-            token['grammemes'] = set(form.tag.grammemes)
-            token['normal_form'] = form.normal_form
-            token['score'] = form.score
-            token['methods_stack'] = form.methods_stack
-            forms.append(token)
-        return forms
-
-    def transform(self, text):
-        for match in re.finditer(self.pattern, text):
-            group = match.lastgroup
-            value = match.group(0)
-            position = match.span()
-            transform_method = getattr(self, 'transform_{}'.format(group), None)
-            if transform_method:
-                token = transform_method(value, position)
-                yield token
-            else:
-                raise NotImplementedError('Unknown token type: {}'.format(group))
-
-    def transform_russian(self, value, position):
-        '''
-        Transforms russian word into token
-        :returns: Token with word morphology info
-        :rtype: Token instance
-        '''
-        return Token(value, position, self.cache(value))
-
-    def transform_latin(self, value, position):
-        '''
-        Transforms latin word into token, note that no morph info is added to token
-        :returns: Token with 'LATN' or 'ROMN' grammeme
-        :rtype: Token instance
-        '''
-        grammemes = {
-            'LATN',
-        }
-        normal_form = value.lower()
-        is_number = is_roman_number(value)
-        if is_number:
-            grammemes = {
-                'NUMBER',
-                'ROMN',
-            }
-            normal_form = value
-            value = decode_roman_number(value)
-        return Token(value, position, [
-            {
-                'grammemes': grammemes,
-                'normal_form': normal_form,
-            }
-        ])
-
-    def transform_quote(self, value, position):
-        '''
-        Transforms different types of quotes to tokens, sets different grammemes
-        to its, based on type of quote (e.g. '«' - gets L-QUOTE grammeme)
-        :returns: Token with 'QUOTE' grammeme and (optional) L/R-QUOTE grammeme
-        '''
+class IntRule(TokenRule):
+    pattern = r'\d+'
+    construct = StrInt
+    grammemes = {'NUMBER', 'INT'}
+
+
+class QuoteRule(TokenRule):
+    # TODO Are ʼʻ” generic? Need to include ˈ and ´
+    pattern = r'["\'«»„“ʼʻ”]'
+
+    def forms(self, value):
         grammemes = {'QUOTE', }
         if value in {'«', '„'}:
-            grammemes |= {'L-QUOTE'} # left quote
+            grammemes |= {'L-QUOTE'}  # left quote
         elif value in {'»', '“'}:
-            grammemes |= {'R-QUOTE'} # right quote
-        else:
-            grammemes |= {'G-QUOTE'} # generic quote like <">
-        return Token(value, position, [
-            {
-                'grammemes': grammemes,
-                'normal_form': value
-            }
-        ])
-
-    def transform_int(self, value, position):
-        '''
-        Transforms integer to token
-        :returns: Token with 'NUMBER' and 'INT' grammemes
-        :rtype: Token instance
-        '''
-        return Token(int(value), position, [
-            {'grammemes': {'NUMBER', 'INT'}, 'normal_form': value}
-        ])
-
-    def transform_int_range(self, value, position):
-        '''
-        Transforms integer range (two numbers separated by dash or minus) to token with 'RANGE' grammeme
-        :returns: Token with 'RANGE' and 'INT-RANGE' grammemes
-        :rtype: Token instance
-        '''
-        start, stop = map(int, re.split(r'[\-\—]', value))
-        if RUNNING_ON_PYTHON_2_VERSION:
-            # do as suggested in official docs: https://docs.python.org/2.7/library/functions.html#xrange
-            if start > sys.maxsize or stop > sys.maxsize:
-                value = frange(start, stop, 1)
-            else:
-                value = xrange(start, stop)
+            grammemes |= {'R-QUOTE'}  # right quote
         else:
-            value = range(start, stop)
-        return Token(value, position, [
-            {'grammemes': {'RANGE', 'INT-RANGE'}, 'normal_form': value}
-        ])
-
-    def transform_int_separated(self, value, position):
-        '''
-        Transforms integer separated by spaces (like 1 000 000) to token with 'INT' grammeme
-        :returns: Token with 'NUMBER' and 'INT' gramemes
-        :rtype: Token instance
-        '''
-        value = int(re.sub('\D', '', value))
-        return Token(value, position, [
-            {'grammemes': {'NUMBER', 'INT', 'INT-SEPARATED'}, 'normal_form': value}
-        ])
-
-    def transform_float(self, value, position):
-        '''
-        Transforms float (with '.' or ',' as delimiter) to token with 'FLOAT' grammeme
-        :returns: Token with 'NUMBER' and 'FLOAT' grammeme
-        :rtype: Token instance
-        '''
-        value = float(value.replace(',', '.'))
-        return Token(value, position, [
-            {'grammemes': {'NUMBER', 'FLOAT'}, 'normal_form': value}
-        ])
-
-    def transform_float_range(self, value, position):
-        '''
-        Transforms floats separated by dash or minus to token with special type - float range
-        Because python built-in `range` type doesnt supports float ranges we use custom type
-        for that purposes, which can be found at `yargy.utils.frange` function
-        :returns: Token with 'RANGE' and 'FLOAT-RANGE' gremmemes
-        :rtype: Token instance
-        '''
-
-        values = map(float, (x.replace(',', '.') for x in re.split(r'[\-\—]', value)))
-        range_value = frange(*values, step=self.frange_step)
-        return Token(range_value, position, [
-            {
-                'grammemes': {'RANGE', 'FLOAT-RANGE'},
-                'normal_form': value,
-            },
-        ])
-
-    def transform_punct(self, value, position):
-        '''
-        Transforms punctuation characters to token with 'PUNCT' grammeme
-        :returns: Token with 'PUNCT' grammeme
-        :rtype: Token instance
-        '''
-        return Token(value, position, [
-            {
-                'grammemes': {'PUNCT'},
-                'normal_form': value
-            }
-        ])
-
-    def transform_email(self, value, position):
-        '''
-        Transforms email address to token with 'EMAIL' grammeme
-        :returns: Token with 'EMAIL' grammeme
-        :rtype: Token instance
-        '''
-        return Token(value, position, [
-            {
-                'grammemes': {'EMAIL'},
-                'normal_form': value,
-            }
-        ])
-
-    def transform_phone(self, value, position):
-        '''
-        Transforms phone number to token with 'PHONE' gremmeme
-        :returns: Token with 'PHONE' grammeme
-        :rtype: Token instance
-        '''
-        value = value.strip()
-        return Token(value, position, [
-            {
-                'grammemes': {'PHONE'},
-                'normal_form': value,
-            }
-        ])
-
-    def transform_end_of_line(self, value, position):
-        '''
-        Transforms end-of-line and caret returns characters to token with 'END-OF-LINE' grammeme
-        :returns: Token with 'END-OF-LINE' grammeme
-        :rtype: Token instance
-        '''
-        return Token(value, position, [
-            {
-                'grammemes': {'END-OF-LINE'},
-                'normal_form': '\n',
-            },
-        ])
+            grammemes |= {'G-QUOTE'}  # generic quote like <">
+
+        yield Form(value, grammemes)
+
+
+class PunctuationRule(TokenRule):
+    pattern = r'[-\\/!#$%&()\[\]\*\+,\.:;<=>?@^_`{|}~№…]'
+    grammemes = {'PUNCT'}
+
+
+class EOLRule(TokenRule):
+    pattern = r'[\n\r]+'
+    grammemes = {'END-OF-LINE'}
+
+    def normalize(self, value):
+        return '\n'
+
+
+class OtherRule(TokenRule):
+    pattern = r'\S'
+    grammemes = {'OTHER'}
+
+
+class EmailRule(TokenRule):
+    pattern = r'[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+'
+    grammemes = {'EMAIL'}
+
+
+class PhoneRule(TokenRule):
+    # found at https://toster.ru/answer?answer_id=852265#answers_list_answer
+    pattern = r'(\+)?([-\s_()]?\d[-\s_()]?){10,14}'
+    grammemes = {'PHONE'}
+
+
+DEFAULT_RULES = [
+    RussianRule(),
+    LatinRule(),
+    IntRule(),
+    QuoteRule(),
+    PunctuationRule(),
+    EOLRule(),
+    OtherRule(),
+    # EmailRule(),
+    # PhoneRule()
+]
+
+
+class Tokenizer(object):
+    def __init__(self, rules=DEFAULT_RULES):
+        for rule in rules:
+            assert_type(rule, TokenRule)
+        self.rules = rules
+        self.regexp, self.mapping = self.compile(rules)
+
+    def add_rules(self, *rules):
+        self.__init__(list(rules) + self.rules)
+        return self
+
+    def remove_rules(self, *rules):
+        self.__init__([_ for _ in self.rules if _ not in rules])
+        return self
+
+    def compile(self, rules):
+        mapping = {}
+        patterns = []
+        for rule in rules:
+            name = 'rule_{id}'.format(id=id(rule))
+            pattern = r'(?P<{name}>{pattern})'.format(
+                name=name,
+                pattern=rule.pattern
+            )
+            mapping[name] = rule
+            patterns.append(pattern)
+
+        pattern = '|'.join(patterns)
+        regexp = re.compile(pattern, re.UNICODE | re.IGNORECASE)
+        return regexp, mapping
+
+    def __call__(self, text):
+        for match in re.finditer(self.regexp, text):
+            name = match.lastgroup
+            value = match.group(0)
+            span = match.span()
+            rule = self.mapping[name]
+            token = rule(value, span)
+            yield token
```

## yargy/morph.py

```diff
@@ -1,5 +1,96 @@
-from pymorphy2 import MorphAnalyzer
+# coding: utf-8
+from __future__ import unicode_literals
 
-# global instance of pymorphy2 morph analyzer
-# which used in tokenization & normalizing methods
-Analyzer = MorphAnalyzer()
+from pymorphy2 import MorphAnalyzer as PymorphyAnalyzer
+
+from .compat import lru_cache
+from .utils import Record
+
+
+class Gender(Record):
+    __attributes__ = ['male', 'female', 'neutral', 'bi', 'general']
+
+    def __init__(self, grammemes):
+        self.male = 'masc' in grammemes
+        self.female = 'femn' in grammemes
+        self.neutral = 'neut' in grammemes
+        self.bi = 'Ms-f' in grammemes or 'ms-f' in grammemes
+        self.general = 'GNdr' in grammemes
+
+
+class Number(Record):
+    __attributes__ = ['single', 'plural', 'only_single', 'only_plural']
+
+    def __init__(self, grammemes):
+        self.single = 'sing' in grammemes
+        self.plural = 'plur' in grammemes
+        self.only_single = 'Sgtm' in grammemes
+        self.only_plural = 'Pltm' in grammemes
+
+
+class Case(Record):
+    __attributes__ = ['mask', 'fixed']
+
+    def __init__(self, grammemes):
+        self.mask = [
+            (_ in grammemes)
+            for _ in ['nomn', 'gent', 'datv', 'accs', 'ablt', 'loct', 'voct']
+        ]
+        self.fixed = 'Fixd' in grammemes
+
+
+class Form(Record):
+    __attributes__ = ['normalized', 'grammemes']
+
+    def __init__(self, normalized, grammemes, raw=None):
+        self.normalized = normalized
+        self.grammemes = grammemes
+        self.raw = raw
+
+    @property
+    def gender(self):
+        return Gender(self.grammemes)
+
+    @property
+    def number(self):
+        return Number(self.grammemes)
+
+    @property
+    def case(self):
+        return Case(self.grammemes)
+
+    def inflect(self, grammemes=None):
+        if self.raw:
+            if grammemes is None:
+                grammemes = {'nomn', 'sing'}
+            form = self.raw.inflect(grammemes)
+            if form:
+                return form.word
+        raise ValueError
+
+
+def prepare_form(record):
+    normalized = record.normal_form
+    grammemes = set(record.tag.grammemes)
+    return Form(normalized, grammemes, raw=record)
+
+
+class MorphAnalyzer(object):
+    def __init__(self):
+        self.analyzer = PymorphyAnalyzer()
+
+    def parse(self, word):
+        records = self.analyzer.parse(word)
+        return [prepare_form(_) for _ in records]
+
+
+DEFAULT_SIZE = 100000
+
+
+class CachedMorphAnalyzer(MorphAnalyzer):
+    def __init__(self, size=DEFAULT_SIZE):
+        super(CachedMorphAnalyzer, self).__init__()
+        self.parse = lru_cache(size)(self.parse)
+
+
+MORPH = CachedMorphAnalyzer()
```

## yargy/__init__.py

```diff
@@ -1,6 +1,7 @@
-# coding: utf-8
-from __future__ import unicode_literals
 
-from yargy.parser import Grammar, Parser, Combinator
 
-__version__ = '0.8.0'
+from .parser import Parser
+from .api import *
+
+
+__version__ = '0.9.1'
```

## yargy/compat.py

```diff
@@ -1,19 +1,20 @@
 try:
     # Python 2
     str = unicode
+    long = long
     string_type = basestring
     range = xrange
     RUNNING_ON_PYTHON_2_VERSION = True
 except NameError:
     # Python 3
     str = str
+    long = int
     string_type = str
     range = range
     RUNNING_ON_PYTHON_2_VERSION = False
-
 try:
     # Python 3.4+
     from functools import lru_cache
 except ImportError:
     # Backport
     from backports.functools_lru_cache import lru_cache
```

## yargy/utils.py

```diff
@@ -1,56 +1,88 @@
 # coding: utf-8
-
 from __future__ import unicode_literals
-from itertools import count, takewhile
-
 
-def frange(start, stop, step):
-    return takewhile(lambda x: x <= stop, (start + i * step for i in count()))
 
-def get_tokens_position(tokens):
-    if not tokens:
-        return None
-    head, tail = tokens[0], tokens[-1]
-    return head.position[0], tail.position[1]
-
-def get_original_text(text, tokens):
-    '''
-    Returns original text captured by parser grammars
-    '''
-    position = get_tokens_position(tokens)
-    if not position:
-        return None
-    else:
-        start, end = position
-    return text[start:end]
-
-def get_desired_index_matches(matches, *indexes):
-    for (n, tokens) in matches:
-        if n in indexes:
-            yield (n, tokens)
-
-
-# stealed from rosettacode
-ROMAN_VALUES = (
-    ('I', 1),
-    ('IV', 4),
-    ('V', 5),
-    ('IX', 9),
-    ('X', 10),
-    ('XL', 40),
-    ('L', 50),
-    ('XC', 90),
-    ('C', 100),
-    ('CD', 400),
-    ('D', 500),
-    ('CM', 900),
-    ('M', 1000),
-)
- 
-def decode_roman_number(number):
-    total = 0
-    for symbol, value in reversed(ROMAN_VALUES):
-        while number.startswith(symbol):
-            total += value
-            number = number[len(symbol):]
-    return total
+def assert_type(item, types):
+    if not isinstance(item, types):
+        if not isinstance(types, tuple):
+            types = [types]
+        raise TypeError('expected {types}, got {type}'.format(
+            types=' or '.join(_.__name__ for _ in types),
+            type=type(item).__name__
+        ))
+
+
+def assert_subclass(item, Class):
+    if not issubclass(item, Class):
+        raise TypeError('expected {expected}, got {got}'.format(
+            expected=Class.__name__,
+            got=item.__name__
+        ))
+
+
+def assert_equals(item, value):
+    if item != value:
+        raise ValueError('expected {value!r}, got {item!r}'.format(
+            item=item,
+            value=value
+        ))
+
+
+def assert_not_empty(item):
+    if len(item) == 0:
+        raise ValueError('expected not empty')
+
+
+class Record(object):
+    __attributes__ = []
+
+    def __eq__(self, other):
+        return (
+            type(self) == type(other)
+            and all(
+                (getattr(self, _) == getattr(other, _))
+                for _ in self.__attributes__
+            )
+        )
+
+    def __ne__(self, other):
+        return not self == other
+
+    def __iter__(self):
+        return (getattr(self, _) for _ in self.__attributes__)
+
+    def __hash__(self):
+        return hash(tuple(self))
+
+    def __repr__(self):
+        name = self.__class__.__name__
+        args = ', '.join(
+            repr(getattr(self, _))
+            for _ in self.__attributes__
+        )
+        return '{name}({args})'.format(
+            name=name,
+            args=args
+        )
+
+    def _repr_pretty_(self, printer, cycle):
+        name = self.__class__.__name__
+        if cycle:
+            printer.text('{name}(...)'.format(name=name))
+        else:
+            with printer.group(len(name) + 1, '{name}('.format(name=name), ')'):
+                for index, key in enumerate(self.__attributes__):
+                    if index > 0:
+                        printer.text(',')
+                        printer.breakable()
+                    value = getattr(self, key)
+                    printer.pretty(value)
+
+
+def flatten(items, list=list):
+    for item in items:
+        if isinstance(item, list):
+            for item in flatten(item):
+                yield item
+        else:
+            yield item
```

## Comparing `yargy-0.8.0.dist-info/metadata.json` & `yargy-0.9.0.dist-info/metadata.json`

 * *Files 8% similar despite different names*

### Pretty-printed

 * *Similarity: 0.8963383838383838%*

 * *Differences: {"'classifiers'": "{insert: [(7, 'Programming Language :: Python :: 3.6')]}",*

 * * "'extensions'": "{'python.details': {'contacts': {0: {'name': 'Yargy contributors'}}, "*

 * *                 "'project_urls': {'Home': 'https://github.com/natasha/yargy'}}}",*

 * * "'generator'": "'bdist_wheel (0.29.0)'",*

 * * "'run_requires'": "{0: {'requires': {delete: [1]}}}",*

 * * "'version'": "'0.9.0'"}*

```diff
@@ -2,52 +2,52 @@
     "classifiers": [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5"
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6"
     ],
     "extensions": {
         "python.details": {
             "contacts": [
                 {
                     "email": "d.a.veselov@yandex.ru",
-                    "name": "Dmitry Veselov",
+                    "name": "Yargy contributors",
                     "role": "author"
                 }
             ],
             "document_names": {
                 "description": "DESCRIPTION.rst"
             },
             "project_urls": {
-                "Home": "https://github.com/bureaucratic-labs/yargy"
+                "Home": "https://github.com/natasha/yargy"
             }
         }
     },
     "extras": [],
-    "generator": "bdist_wheel (0.30.0.a0)",
+    "generator": "bdist_wheel (0.29.0)",
     "keywords": [
         "natural",
         "language",
         "processing",
         "russian",
         "morphology"
     ],
     "license": "MIT",
     "metadata_version": "2.0",
     "name": "yargy",
     "run_requires": [
         {
             "requires": [
                 "backports.functools-lru-cache (==1.3)",
-                "enum34 (==1.1.6)",
                 "intervaltree (==2.1.0)",
                 "jellyfish (==0.5.6)",
                 "pymorphy2 (==0.8)"
             ]
         }
     ],
     "summary": "Tiny rule-based facts extraction package",
-    "version": "0.8.0"
+    "version": "0.9.0"
 }
```

## Comparing `yargy-0.8.0.dist-info/METADATA` & `yargy-0.9.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.0
 Name: yargy
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tiny rule-based facts extraction package
-Home-page: https://github.com/bureaucratic-labs/yargy
-Author: Dmitry Veselov
+Home-page: https://github.com/natasha/yargy
+Author: Yargy contributors
 Author-email: d.a.veselov@yandex.ru
 License: MIT
 Keywords: natural language processing,russian morphology
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
-Requires-Dist: pymorphy2 (==0.8)
-Requires-Dist: enum34 (==1.1.6)
+Classifier: Programming Language :: Python :: 3.6
 Requires-Dist: backports.functools-lru-cache (==1.3)
 Requires-Dist: intervaltree (==2.1.0)
 Requires-Dist: jellyfish (==0.5.6)
+Requires-Dist: pymorphy2 (==0.8)
 
 UNKNOWN
```

