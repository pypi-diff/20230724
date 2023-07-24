# Comparing `tmp/pythainlp-4.0.2.tar.gz` & `tmp/pythainlp-4.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythainlp-4.0.2.tar", last modified: Tue May 30 17:13:13 2023, max compression
+gzip compressed data, was "pythainlp-4.1.0b1.tar", last modified: Mon Jul 24 05:02:55 2023, max compression
```

## Comparing `pythainlp-4.0.2.tar` & `pythainlp-4.1.0b1.tar`

### file list

```diff
@@ -1,209 +1,239 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.050603 pythainlp-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-05-30 17:13:02.000000 pythainlp-4.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-30 17:13:02.000000 pythainlp-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-30 17:13:02.000000 pythainlp-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-30 17:13:13.054603 pythainlp-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-05-30 17:13:02.000000 pythainlp-4.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-05-30 17:13:02.000000 pythainlp-4.0.2/README_TH.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/augment/
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/augment/lm/
--rw-r--r--   0 runner    (1001) docker     (122)      810 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/lm/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/lm/wangchanberta.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/augment/word2vec/
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/bpemb_wv.py
--rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/ltw2v.py
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/word2vec/thai2fit.py
--rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/augment/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/benchmarks/word_tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/cli/
--rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/tag.py
--rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/cli/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (122)     2799 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8281 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/conceptnet.py
--rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/oscar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/th_en_translit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/tnc.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/ttc.py
--rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/corpus/wordnet.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/generate/
--rw-r--r--   0 runner    (1001) docker     (122)      747 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/generate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/generate/thai2fit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.030602 pythainlp-4.0.2/pythainlp/khavee/
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/khavee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20881 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/khavee/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/khavee/example.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/parse/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      853 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/esupar_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/spacy_thai_engine.py
--rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/transformers_ud.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/parse/ud_goeswith.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/soundex/
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/lk82.py
--rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/metasound.py
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/prayut_and_somchaip.py
--rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/soundex/udom83.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/spell/
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      993 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/phunspell.py
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/pn.py
--rw-r--r--   0 runner    (1001) docker     (122)     2335 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/symspellpy.py
--rw-r--r--   0 runner    (1001) docker     (122)      952 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/spell/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.034602 pythainlp-4.0.2/pythainlp/summarize/
--rw-r--r--   0 runner    (1001) docker     (122)      902 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/freq.py
--rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/keybert.py
--rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/summarize/mt5.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.038602 pythainlp-4.0.2/pythainlp/tag/
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/_tag_perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/chunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/crfchunk.py
--rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/locations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5939 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/orchid.py
--rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/perceptron.py
--rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/pos_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/thai_nner.py
--rw-r--r--   0 runner    (1001) docker     (122)     8093 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/thainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/unigram.py
--rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tag/wangchanberta_onnx.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/tokenize/
--rw-r--r--   0 runner    (1001) docker     (122)     1579 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/attacut.py
--rw-r--r--   0 runner    (1001) docker     (122)    26351 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/crfcls.py
--rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/crfcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/deepcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/etcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/longest.py
--rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/multi_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/nercut.py
--rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/newmm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/nlpo3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/oskut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/sefr_cut.py
--rw-r--r--   0 runner    (1001) docker     (122)      861 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/ssg.py
--rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/tcc.py
--rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/tcc_p.py
--rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/thaisumcut.py
--rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tokenize/tltk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/tools/
--rw-r--r--   0 runner    (1001) docker     (122)      892 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tools/misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/tools/path.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/translate/
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3440 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     5193 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/en_th.py
--rw-r--r--   0 runner    (1001) docker     (122)     2345 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/th_fr.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/translate/zh_th.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.042602 pythainlp-4.0.2/pythainlp/transliterate/
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/core.py
--rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/ipa.py
--rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/iso_11940.py
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/lookup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/pyicu.py
--rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/royin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/spoonerism.py
--rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/thai2rom.py
--rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/thai2rom_onnx.py
--rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/thaig2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/tltk.py
--rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/w2p.py
--rw-r--r--   0 runner    (1001) docker     (122)     5847 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/transliterate/wunsen.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/ulmfit/
--rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/ulmfit/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/util/
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/collate.py
--rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/date.py
--rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/digitconv.py
--rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/emojiconv.py
--rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/keyboard.py
--rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/keywords.py
--rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/numtoword.py
--rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/phoneme.py
--rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/strftime.py
--rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/syllable.py
--rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/thai.py
--rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/thaiwordcheck.py
--rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/trie.py
--rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/util/wordtonum.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/wangchanberta/
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/wangchanberta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/wangchanberta/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.046602 pythainlp-4.0.2/pythainlp/word_vector/
--rw-r--r--   0 runner    (1001) docker     (122)      800 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/word_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-05-30 17:13:02.000000 pythainlp-4.0.2/pythainlp/word_vector/core.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.026602 pythainlp-4.0.2/pythainlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2721 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-30 17:13:12.000000 pythainlp-4.0.2/pythainlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-30 17:13:13.054603 pythainlp-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5914 2023-05-30 17:13:02.000000 pythainlp-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.050603 pythainlp-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      295 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 17:13:13.050603 pythainlp-4.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/eval-details-input.json
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/eval-input.yml
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/input.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/sentences.yml
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/data/test.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_khavee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_misspell.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (122)     3605 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_soundex.py
--rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_spell.py
--rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_summarize.py
--rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (122)    55078 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (122)     2259 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_translate.py
--rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_transliterate.py
--rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_ulmfit.py
--rw-r--r--   0 runner    (1001) docker     (122)    36563 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_wangchanberta.py
--rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-05-30 17:13:02.000000 pythainlp-4.0.2/tests/test_word_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (122)     7203 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10578 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)    15412 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/README_TH.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.692494 pythainlp-4.1.0b1/pythainlp/
+-rw-r--r--   0 runner    (1001) docker     (122)     2449 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1428 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.692494 pythainlp-4.1.0b1/pythainlp/augment/
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.692494 pythainlp-4.1.0b1/pythainlp/augment/lm/
+-rw-r--r--   0 runner    (1001) docker     (122)      810 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3003 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/lm/fasttext.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3415 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/lm/wangchanberta.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.696494 pythainlp-4.1.0b1/pythainlp/augment/word2vec/
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/word2vec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2444 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/word2vec/bpemb_wv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/word2vec/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2192 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/word2vec/ltw2v.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/word2vec/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/augment/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.696494 pythainlp-4.1.0b1/pythainlp/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8187 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/benchmarks/word_tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.696494 pythainlp-4.1.0b1/pythainlp/chat/
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3306 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/chat/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.700494 pythainlp-4.1.0b1/pythainlp/cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     1158 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5723 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cli/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4521 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cli/soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2761 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cli/tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5275 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cli/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.700494 pythainlp-4.1.0b1/pythainlp/cls/
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3500 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/cls/param_free.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.700494 pythainlp-4.1.0b1/pythainlp/coref/
+-rw-r--r--   0 runner    (1001) docker     (122)      748 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/coref/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1418 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/coref/_fastcoref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/coref/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      930 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/coref/han_coref.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.704494 pythainlp-4.1.0b1/pythainlp/corpus/
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11287 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4549 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/conceptnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17555 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/oscar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3119 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/th_en_translit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2755 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/tnc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/ttc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5102 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14410 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/corpus/wordnet.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.704494 pythainlp-4.1.0b1/pythainlp/el/
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/el/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1237 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/el/_multiel.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2480 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/el/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.704494 pythainlp-4.1.0b1/pythainlp/generate/
+-rw-r--r--   0 runner    (1001) docker     (122)      747 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9354 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/generate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3136 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/generate/thai2fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7627 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/generate/wangchanglm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.704494 pythainlp-4.1.0b1/pythainlp/khavee/
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/khavee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20883 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/khavee/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6599 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/khavee/example.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.708494 pythainlp-4.1.0b1/pythainlp/parse/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5878 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/parse/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/parse/esupar_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/parse/spacy_thai_engine.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4903 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/parse/transformers_ud.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/parse/ud_goeswith.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.708494 pythainlp-4.1.0b1/pythainlp/soundex/
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3560 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4562 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/lk82.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3501 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/metasound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/prayut_and_somchaip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2835 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/sound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3323 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/soundex/udom83.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.708494 pythainlp-4.1.0b1/pythainlp/spell/
+-rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/spell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6523 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/spell/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)      993 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/spell/phunspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11880 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/spell/pn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2290 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/spell/symspellpy.py
+-rw-r--r--   0 runner    (1001) docker     (122)      952 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/spell/tltk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.712494 pythainlp-4.1.0b1/pythainlp/summarize/
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/summarize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12359 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/summarize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/summarize/freq.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9478 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/summarize/keybert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3006 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/summarize/mt5.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.712494 pythainlp-4.1.0b1/pythainlp/tag/
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10480 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/_tag_perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1501 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2769 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/crfchunk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1505 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/locations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5974 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/orchid.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2617 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/perceptron.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7618 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/pos_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/thai_nner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8068 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/thainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3000 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/unigram.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4312 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tag/wangchanberta_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.712494 pythainlp-4.1.0b1/pythainlp/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3626 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/attacut.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29817 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2650 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/crfcls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5904 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/crfcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1432 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/deepcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/etcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/longest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5032 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/multi_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2731 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/nercut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7383 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/newmm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2614 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/nlpo3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1299 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/oskut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1231 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/sefr_cut.py
+-rw-r--r--   0 runner    (1001) docker     (122)      861 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/ssg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2929 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/tcc.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2941 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/tcc_p.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/thaisumcut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1624 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tokenize/wtsplit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.716494 pythainlp-4.1.0b1/pythainlp/tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      892 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4531 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tools/misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2479 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/tools/path.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.716494 pythainlp-4.1.0b1/pythainlp/translate/
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3667 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5207 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/en_th.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1960 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/small100.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2363 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/th_fr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15964 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/tokenization_small100.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3725 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/translate/zh_th.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.716494 pythainlp-4.1.0b1/pythainlp/transliterate/
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7349 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1092 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/ipa.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3168 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/iso_11940.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1236 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/pyicu.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6246 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/royin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/spoonerism.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11993 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/thai2rom.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6477 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/thai2rom_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12039 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/thaig2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1370 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/tltk.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7168 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/w2p.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5848 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/transliterate/wunsen.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.716494 pythainlp-4.1.0b1/pythainlp/ulmfit/
+-rw-r--r--   0 runner    (1001) docker     (122)     2060 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/ulmfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8987 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/ulmfit/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10463 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/ulmfit/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/ulmfit/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/pythainlp/util/
+-rw-r--r--   0 runner    (1001) docker     (122)     3545 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1955 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/abbreviation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/collate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12287 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5783 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/digitconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93944 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/emojiconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7189 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/keyboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4180 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3737 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/numtoword.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5284 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/phoneme.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4105 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/spell_words.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13782 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10169 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/syllable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7284 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/thai.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3826 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/thaiwordcheck.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10186 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/trie.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7102 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/util/wordtonum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/pythainlp/wangchanberta/
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/wangchanberta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8662 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/wangchanberta/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/pythainlp/word_vector/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/word_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14056 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/word_vector/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/pythainlp/wsd/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/wsd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5449 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/pythainlp/wsd/core.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.692494 pythainlp-4.1.0b1/pythainlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2900 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5717 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1901 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-24 05:02:55.000000 pythainlp-4.1.0b1/pythainlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      702 2023-07-24 05:02:55.724494 pythainlp-4.1.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     6572 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      295 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-24 05:02:55.720494 pythainlp-4.1.0b1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/data/eval-details-input.json
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/data/eval-input.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/data/input.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/data/sentences.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/data/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1771 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2931 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6083 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_cls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_coref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7255 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (122)      338 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_el.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2171 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_khavee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2151 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_misspell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3890 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_soundex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_spell.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5810 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17423 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (122)    56445 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2712 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_translate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11136 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_transliterate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9017 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_ulmfit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37455 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_wangchanberta.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2329 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_word_vector.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-07-24 05:02:45.000000 pythainlp-4.1.0b1/tests/test_wsd.py
```

### Comparing `pythainlp-4.0.2/CONTRIBUTING.md` & `pythainlp-4.1.0b1/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 <a href="https://github.com/PyThaiNLP/pythainlp/graphs/contributors">
   <img src="https://contributors-img.firebaseapp.com/image?repo=PyThaiNLP/pythainlp" />
 </a>
 
 Thanks all the [contributors](https://github.com/PyThaiNLP/pythainlp/graphs/contributors). (Image made with [contributors-img](https://contributors-img.firebaseapp.com))
 
 ### Development Lead
-- Wannaphong Phatthiyaphaibun <email@wannaphong.com> - founder, distribution and maintainance
+- Wannaphong Phatthiyaphaibun <wannaphong@yahoo.com> - founder, distribution and maintainance
 - Korakot Chaovavanich - initial tokenization and soundex code
 - Charin Polpanumas - classification and benchmarking
 - Peeradej Tanruangporn - documentation
 - Arthit Suriyawongkul - refactoring, packaging, distribution, and maintainance
 - Chakri Lowphansirikul - documentation
 - Pattarawat Chormai - benchmarking
 - Thanathip Suntorntip - nlpO3 maintainance, Rust Developer
```

### Comparing `pythainlp-4.0.2/LICENSE` & `pythainlp-4.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/README.md` & `pythainlp-4.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/README_TH.md` & `pythainlp-4.1.0b1/README_TH.md`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/__init__.py` & `pythainlp-4.1.0b1/pythainlp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # URL: <https://pythainlp.github.io/>
 # For license information, see LICENSE
-__version__ = "4.0.2"
+__version__ = "4.1.0beta1"
 
 thai_consonants = "กขฃคฅฆงจฉชซฌญฎฏฐฑฒณดตถทธนบปผฝพฟภมยรลวศษสหฬอฮ"  # 44 chars
 
 thai_vowels = (
     "\u0e24\u0e26\u0e30\u0e31\u0e32\u0e33\u0e34\u0e35\u0e36\u0e37"
     + "\u0e38\u0e39\u0e40\u0e41\u0e42\u0e43\u0e44\u0e45\u0e4d\u0e47"
 )  # 20
```

### Comparing `pythainlp-4.0.2/pythainlp/__main__.py` & `pythainlp-4.1.0b1/pythainlp/__main__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/__init__.py` & `pythainlp-4.1.0b1/pythainlp/augment/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/lm/__init__.py` & `pythainlp-4.1.0b1/pythainlp/augment/lm/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/lm/fasttext.py` & `pythainlp-4.1.0b1/pythainlp/augment/lm/fasttext.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/lm/wangchanberta.py` & `pythainlp-4.1.0b1/pythainlp/augment/lm/wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/word2vec/__init__.py` & `pythainlp-4.1.0b1/pythainlp/augment/word2vec/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/word2vec/bpemb_wv.py` & `pythainlp-4.1.0b1/pythainlp/augment/word2vec/bpemb_wv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/word2vec/core.py` & `pythainlp-4.1.0b1/pythainlp/augment/word2vec/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/word2vec/ltw2v.py` & `pythainlp-4.1.0b1/pythainlp/augment/word2vec/ltw2v.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/word2vec/thai2fit.py` & `pythainlp-4.1.0b1/pythainlp/augment/word2vec/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/augment/wordnet.py` & `pythainlp-4.1.0b1/pythainlp/augment/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/benchmarks/__init__.py` & `pythainlp-4.1.0b1/pythainlp/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/benchmarks/word_tokenization.py` & `pythainlp-4.1.0b1/pythainlp/benchmarks/word_tokenization.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/cli/__init__.py` & `pythainlp-4.1.0b1/pythainlp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/cli/benchmark.py` & `pythainlp-4.1.0b1/pythainlp/cli/benchmark.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/cli/data.py` & `pythainlp-4.1.0b1/pythainlp/cli/data.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/cli/soundex.py` & `pythainlp-4.1.0b1/pythainlp/cli/soundex.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/cli/tag.py` & `pythainlp-4.1.0b1/pythainlp/cli/tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/cli/tokenize.py` & `pythainlp-4.1.0b1/pythainlp/cli/tokenize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/__init__.py` & `pythainlp-4.1.0b1/pythainlp/corpus/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,21 +28,25 @@
     "get_corpus",
     "get_corpus_db",
     "get_corpus_db_detail",
     "get_corpus_default_db",
     "get_corpus_path",
     "provinces",
     "remove",
+    "thai_dict",
     "thai_family_names",
     "thai_female_names",
     "thai_male_names",
     "thai_negations",
+    "thai_synonym",
     "thai_stopwords",
     "thai_syllables",
     "thai_words",
+    "thai_wsd_dict",
+    "thai_orst_words",
     "path_pythainlp_corpus",
     "get_path_folder_corpus",
 ]
 
 import os
 
 from pythainlp.tools import get_full_data_path, get_pythainlp_path
@@ -103,11 +107,15 @@
 from pythainlp.corpus.common import (
     countries,
     provinces,
     thai_family_names,
     thai_female_names,
     thai_male_names,
     thai_negations,
+    thai_synonym,
     thai_stopwords,
     thai_syllables,
     thai_words,
+    thai_orst_words,
+    thai_dict,
+    thai_wsd_dict
 )
```

### Comparing `pythainlp-4.0.2/pythainlp/corpus/common.py` & `pythainlp-4.1.0b1/pythainlp/corpus/common.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,19 +22,22 @@
     "thai_family_names",
     "thai_female_names",
     "thai_male_names",
     "thai_negations",
     "thai_stopwords",
     "thai_syllables",
     "thai_words",
+    "thai_dict",
+    "thai_wsd_dict",
+    "thai_synonym",
 ]
 
 from typing import FrozenSet, List, Union
 
-from pythainlp.corpus import get_corpus
+from pythainlp.corpus import get_corpus, get_corpus_path
 
 _THAI_COUNTRIES = set()
 _THAI_COUNTRIES_FILENAME = "countries_th.txt"
 
 _THAI_THAILAND_PROVINCES = set()
 _THAI_THAILAND_PROVINCES_DETAILS = list()
 _THAI_THAILAND_PROVINCES_FILENAME = "thailand_provinces_th.csv"
@@ -54,14 +57,20 @@
 _THAI_FAMLIY_NAMES = set()
 _THAI_FAMLIY_NAMES_FILENAME = "family_names_th.txt"
 _THAI_FEMALE_NAMES = set()
 _THAI_FEMALE_NAMES_FILENAME = "person_names_female_th.txt"
 _THAI_MALE_NAMES = set()
 _THAI_MALE_NAMES_FILENAME = "person_names_male_th.txt"
 
+_THAI_ORST_WORDS = set()
+
+_THAI_DICT = {}
+_THAI_WSD_DICT = {}
+_THAI_SYNONYM = None
+
 
 def countries() -> FrozenSet[str]:
     """
     Return a frozenset of country names in Thai such as "แคนาดา", "โรมาเนีย",
     "แอลจีเรีย", and "ลาว".
     \n(See: `dev/pythainlp/corpus/countries_th.txt\
     <https://github.com/PyThaiNLP/pythainlp/blob/dev/pythainlp/corpus/countries_th.txt>`_)
@@ -149,14 +158,30 @@
     global _THAI_WORDS
     if not _THAI_WORDS:
         _THAI_WORDS = get_corpus(_THAI_WORDS_FILENAME)
 
     return _THAI_WORDS
 
 
+def thai_orst_words() -> FrozenSet[str]:
+    """
+    Return a frozenset of Thai words from Royal Society of Thailand
+    \n(See: `dev/pythainlp/corpus/thai_orst_words.txt\
+    <https://github.com/PyThaiNLP/pythainlp/blob/dev/pythainlp/corpus/thai_orst_words>`_)
+
+    :return: :class:`frozenset` containing words in Thai language.
+    :rtype: :class:`frozenset`
+    """
+    global _THAI_ORST_WORDS
+    if not _THAI_ORST_WORDS:
+        _THAI_ORST_WORDS = get_corpus("thai_orst_words.txt")
+
+    return _THAI_ORST_WORDS
+
+
 def thai_stopwords() -> FrozenSet[str]:
     """
     Return a frozenset of Thai stopwords such as "มี", "ไป", "ไง", "ขณะ",
     "การ", and "ประการหนึ่ง". \n(See: `dev/pythainlp/corpus/stopwords_th.txt\
     <https://github.com/PyThaiNLP/pythainlp/blob/dev/pythainlp/corpus/stopwords_th.txt>`_)
     We using stopword lists by thesis's เพ็ญศิริ ลี้ตระกูล.
 
@@ -234,7 +259,78 @@
     :rtype: :class:`frozenset`
     """
     global _THAI_MALE_NAMES
     if not _THAI_MALE_NAMES:
         _THAI_MALE_NAMES = get_corpus(_THAI_MALE_NAMES_FILENAME)
 
     return _THAI_MALE_NAMES
+
+
+def thai_dict() -> dict:
+    """
+    Return Thai dictionary with definition from wiktionary.
+    \n(See: `thai_dict\
+    <https://pythainlp.github.io/pythainlp-corpus/thai_dict.html>`_)
+
+    :return: Thai word with part-of-speech type and definition
+    :rtype: dict
+    """
+    global _THAI_DICT
+    if _THAI_DICT == {}:
+        import csv
+        _THAI_DICT = {"word":[], "meaning":[]}
+        with open(get_corpus_path("thai_dict"), newline="\n", encoding="utf-8") as csvfile:
+            reader = csv.DictReader(csvfile, delimiter=",")
+            for row in reader:
+                _THAI_DICT["word"].append(row["word"])
+                _THAI_DICT["meaning"].append(row["meaning"])
+
+    return _THAI_DICT
+
+
+def thai_wsd_dict() -> dict:
+    """
+    Return Thai Word Sense Disambiguation dictionary with definition from wiktionary.
+    \n(See: `thai_dict\
+    <https://pythainlp.github.io/pythainlp-corpus/thai_dict.html>`_)
+
+    :return: Thai word with part-of-speech type and definition
+    :rtype: dict
+    """
+    global _THAI_WSD_DICT
+    if _THAI_WSD_DICT == {}:
+        _thai_wsd = thai_dict()
+        _THAI_WSD_DICT = {"word":[],"meaning":[]}
+        for i,j in zip(_thai_wsd["word"],_thai_wsd["meaning"]):
+            _all_value = list(eval(j).values())
+            _use = []
+            for k in _all_value:
+                _use.extend(k)
+            _use=list(set(_use))
+            if len(_use)>1:
+                _THAI_WSD_DICT["word"].append(i)
+                _THAI_WSD_DICT["meaning"].append(_use)
+
+    return _THAI_WSD_DICT
+
+
+def thai_synonym() -> dict:
+    """
+    Return Thai synonym.
+    \n(See: `thai_synonym\
+    <https://pythainlp.github.io/pythainlp-corpus/thai_synonym.html>`_)
+
+    :return: Thai word with part-of-speech type and synonym
+    :rtype: dict
+    """
+    global _THAI_SYNONYM
+    if _THAI_SYNONYM == None:
+        import csv
+        _THAI_SYNONYM = {"word":[], "pos":[], "synonym":[]}
+        with open(get_corpus_path("thai_synonym"), newline="\n", encoding="utf-8") as csvfile:
+            reader = csv.DictReader(csvfile, delimiter=",")
+            for row in reader:
+                _THAI_SYNONYM["word"].append(row["word"])
+                _THAI_SYNONYM["pos"].append(row["pos"])
+                _THAI_SYNONYM["synonym"].append(row["synonym"].split("|"))
+
+    return _THAI_SYNONYM
```

### Comparing `pythainlp-4.0.2/pythainlp/corpus/conceptnet.py` & `pythainlp-4.1.0b1/pythainlp/corpus/conceptnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/core.py` & `pythainlp-4.1.0b1/pythainlp/corpus/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/oscar.py` & `pythainlp-4.1.0b1/pythainlp/corpus/oscar.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/th_en_translit.py` & `pythainlp-4.1.0b1/pythainlp/corpus/th_en_translit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/tnc.py` & `pythainlp-4.1.0b1/pythainlp/corpus/tnc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/ttc.py` & `pythainlp-4.1.0b1/pythainlp/corpus/ttc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/util.py` & `pythainlp-4.1.0b1/pythainlp/corpus/util.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/corpus/wordnet.py` & `pythainlp-4.1.0b1/pythainlp/corpus/wordnet.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/generate/__init__.py` & `pythainlp-4.1.0b1/pythainlp/generate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/generate/core.py` & `pythainlp-4.1.0b1/pythainlp/generate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/generate/thai2fit.py` & `pythainlp-4.1.0b1/pythainlp/generate/thai2fit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/khavee/__init__.py` & `pythainlp-4.1.0b1/pythainlp/khavee/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/khavee/core.py` & `pythainlp-4.1.0b1/pythainlp/khavee/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,14 +414,15 @@
             
         else:
             return 'Something went wrong Make sure you enter it in correct form.'
         
     def check_aek_too(self, text: Union[List[str], str], dead_syllable_as_aek:bool = False) -> Union[List[bool], List[str], bool, str]:
         """
         Thai tonal word checker
+
         :param Union[List[str], str] text: Thai word or list of Thai words
         :param bool dead_syllable_as_aek: if True, dead syllable will be considered as aek
         :return: the check if the word is aek or too or False(not both) or list of the check if input is list
         :rtype: Union[List[bool], List[str], bool, str]
 
         :Example:
         ::
```

### Comparing `pythainlp-4.0.2/pythainlp/khavee/example.py` & `pythainlp-4.1.0b1/pythainlp/khavee/example.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/parse/__init__.py` & `pythainlp-4.1.0b1/pythainlp/parse/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/parse/core.py` & `pythainlp-4.1.0b1/pythainlp/parse/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/parse/esupar_engine.py` & `pythainlp-4.1.0b1/pythainlp/parse/esupar_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/parse/spacy_thai_engine.py` & `pythainlp-4.1.0b1/pythainlp/parse/spacy_thai_engine.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/parse/transformers_ud.py` & `pythainlp-4.1.0b1/pythainlp/parse/transformers_ud.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/parse/ud_goeswith.py` & `pythainlp-4.1.0b1/pythainlp/parse/ud_goeswith.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/soundex/__init__.py` & `pythainlp-4.1.0b1/pythainlp/soundex/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/soundex/core.py` & `pythainlp-4.1.0b1/pythainlp/soundex/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/soundex/lk82.py` & `pythainlp-4.1.0b1/pythainlp/soundex/lk82.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/soundex/metasound.py` & `pythainlp-4.1.0b1/pythainlp/soundex/metasound.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/soundex/prayut_and_somchaip.py` & `pythainlp-4.1.0b1/pythainlp/soundex/prayut_and_somchaip.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/soundex/udom83.py` & `pythainlp-4.1.0b1/pythainlp/soundex/udom83.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/spell/__init__.py` & `pythainlp-4.1.0b1/pythainlp/spell/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/spell/core.py` & `pythainlp-4.1.0b1/pythainlp/spell/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/spell/phunspell.py` & `pythainlp-4.1.0b1/pythainlp/spell/phunspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/spell/pn.py` & `pythainlp-4.1.0b1/pythainlp/spell/pn.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,16 @@
                             (default = 40)
         :param func dict_filter: A function to filter the dictionary.
                                  Default filter removes any word
                                  with number or non-Thai characters.
                                  If no filter is required, use None.
         """
         if not custom_dict:  # default, use Thai National Corpus
-            custom_dict = tnc.word_freqs()
+            # TODO: #680 change the dict
+            custom_dict = [(i,j) for i,j in tnc.word_freqs()]
 
         if not dict_filter:
             dict_filter = _no_filter
 
         custom_dict = _convert_custom_dict(
             custom_dict, min_freq, min_len, max_len, dict_filter
         )
```

### Comparing `pythainlp-4.0.2/pythainlp/spell/symspellpy.py` & `pythainlp-4.1.0b1/pythainlp/spell/symspellpy.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     * \
         https://github.com/mammothb/symspellpy
 """
 from typing import List
 from symspellpy import SymSpell, Verbosity
 from pythainlp.corpus import get_corpus_path
 from pythainlp.corpus import path_pythainlp_corpus
-from pythainlp.tokenize import word_tokenize
 
 _UNIGRAM = "tnc_freq.txt"
 _BIGRAM = "tnc_bigram_word_freqs"
 
 sym_spell = SymSpell()
 sym_spell.load_dictionary(
     path_pythainlp_corpus(_UNIGRAM), 0, 1, separator="\t", encoding="utf-8-sig"
```

### Comparing `pythainlp-4.0.2/pythainlp/spell/tltk.py` & `pythainlp-4.1.0b1/pythainlp/spell/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/summarize/__init__.py` & `pythainlp-4.1.0b1/pythainlp/summarize/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/summarize/core.py` & `pythainlp-4.1.0b1/pythainlp/summarize/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/summarize/freq.py` & `pythainlp-4.1.0b1/pythainlp/summarize/freq.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/summarize/keybert.py` & `pythainlp-4.1.0b1/pythainlp/summarize/keybert.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/summarize/mt5.py` & `pythainlp-4.1.0b1/pythainlp/summarize/mt5.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/__init__.py` & `pythainlp-4.1.0b1/pythainlp/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/_tag_perceptron.py` & `pythainlp-4.1.0b1/pythainlp/tag/_tag_perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/blackboard.py` & `pythainlp-4.1.0b1/pythainlp/tag/blackboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/chunk.py` & `pythainlp-4.1.0b1/pythainlp/tag/chunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/crfchunk.py` & `pythainlp-4.1.0b1/pythainlp/tag/crfchunk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/locations.py` & `pythainlp-4.1.0b1/pythainlp/tag/locations.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/named_entity.py` & `pythainlp-4.1.0b1/pythainlp/tag/named_entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,25 +23,25 @@
     """
     Named-entity recognizer class
 
     :param str engine: Named-entity recognizer engine
     :param str corpus: corpus
 
     **Options for engine**
+        * *thainer-v2* - Thai NER engine v2.0 for Thai NER 2.0 (default)
         * *thainer* - Thai NER engine
         * *tltk* - wrapper for `TLTK <https://pypi.org/project/tltk/>`_.
-        * *thainer-v2* - Thai NER engine v2.0 for Thai NER 2.0
 
     **Options for corpus**
-        * *thainer* - Thai NER corpus
+        * *thainer* - Thai NER corpus (default)
 
     **Note**: for tltk engine, It's support ner model from tltk only.
     """
 
-    def __init__(self, engine: str, corpus: str = "thainer") -> None:
+    def __init__(self, engine: str = "thainer-v2", corpus: str = "thainer") -> None:
         self.load_engine(engine=engine, corpus=corpus)
 
     def load_engine(self, engine: str, corpus: str) -> None:
         self.name_engine = engine
         self.engine = None
         if engine == "thainer" and corpus == "thainer":
             from pythainlp.tag.thainer import ThaiNameTagger
```

### Comparing `pythainlp-4.0.2/pythainlp/tag/orchid.py` & `pythainlp-4.1.0b1/pythainlp/tag/orchid.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/perceptron.py` & `pythainlp-4.1.0b1/pythainlp/tag/perceptron.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/pos_tag.py` & `pythainlp-4.1.0b1/pythainlp/tag/pos_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/thai_nner.py` & `pythainlp-4.1.0b1/pythainlp/tag/thai_nner.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/thainer.py` & `pythainlp-4.1.0b1/pythainlp/tag/thainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from typing import Dict, List, Tuple, Union
 
 from pythainlp.corpus import get_corpus_path, thai_stopwords
 from pythainlp.tag import pos_tag
 from pythainlp.tokenize import word_tokenize
 from pythainlp.util import isthai
 
-_CORPUS_NAME = "thainer"
 _TOKENIZER_ENGINE = "newmm"  # should be the same as one used in training data
 
 
 def _is_stopword(word: str) -> bool:  # เช็คว่าเป็นคำฟุ่มเฟือย
     return word in thai_stopwords()
```

### Comparing `pythainlp-4.0.2/pythainlp/tag/tltk.py` & `pythainlp-4.1.0b1/pythainlp/tag/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/unigram.py` & `pythainlp-4.1.0b1/pythainlp/tag/unigram.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tag/wangchanberta_onnx.py` & `pythainlp-4.1.0b1/pythainlp/tag/wangchanberta_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/__init__.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "Tokenizer",
     "Trie",
     "clause_tokenize",
     "sent_tokenize",
     "subword_tokenize",
     "word_tokenize",
     "word_detokenize",
+    "paragraph_tokenize",
 ]
 
 from pythainlp.corpus import thai_syllables, thai_words
 from pythainlp.util.trie import Trie
 
 DEFAULT_WORD_TOKENIZE_ENGINE = "newmm"
 DEFAULT_SENT_TOKENIZE_ENGINE = "crfcut"
@@ -42,14 +43,15 @@
 from pythainlp.tokenize.core import (
     Tokenizer,
     clause_tokenize,
     sent_tokenize,
     subword_tokenize,
     word_tokenize,
     word_detokenize,
+    paragraph_tokenize,
 )
 
 from pythainlp.corpus import get_corpus as _get_corpus
 
 THAI2FIT_TOKENIZER = Tokenizer(
     custom_dict=_get_corpus("words_th_thai2fit_201810.txt"), engine="newmm"
 )
```

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/_utils.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/_utils.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/attacut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/attacut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/core.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     Tokenizes running word list into list of clauses (list of strings).
     split by CRF trained on Blackboard Treebank.
 
     :param str doc: word list to be clause
     :return: list of claues
     :rtype: list[list[str]]
     :Example:
-    Clause tokenizer::
+    ::
+
         from pythainlp.tokenize import clause_tokenize
         clause_tokenize(["ฉัน","นอน","และ","คุณ","เล่น","มือถือ","ส่วน","น้อง","เขียน","โปรแกรม"])
         # [['ฉัน', 'นอน'],
         # ['และ', 'คุณ', 'เล่น', 'มือถือ'],
         # ['ส่วน', 'น้อง', 'เขียน', 'โปรแกรม']]
     """
     from pythainlp.tokenize.crfcls import segment
@@ -64,14 +65,20 @@
 
     This function will detokenize the list word in each sentence to text.
 
     :param str segments: List sentences with list words.
     :param str output: the output type (str or list)
     :return: the thai text
     :rtype: Union[str,List[str]]
+    :Example:
+    ::
+
+        from pythainlp.tokenize import word_detokenize
+        print(word_detokenize(["เรา", "เล่น"]))
+        # output: เราเล่น
     """
     _list_all = []
     if isinstance(segments[0], str):
         segments = [segments]
     from pythainlp import thai_characters
 
     for i, s in enumerate(segments):
@@ -340,14 +347,20 @@
     :return: list of splited sentences
     :rtype: list[str]
     **Options for engine**
         * *crfcut* - (default) split by CRF trained on TED dataset
         * *thaisum* - The implementation of sentence segmentator from \
             Nakhun Chumpolsathien, 2020
         * *tltk* - split by `TLTK <https://pypi.org/project/tltk/>`_.,
+        * *wtp* - split by `wtpsplitaxe <https://github.com/bminixhofer/wtpsplit>`_., \
+            It support many size of models. You can use ``wtp`` to use mini model, \
+            ``wtp-tiny`` to use ``wtp-bert-tiny`` model (default), \
+            ``wtp-mini`` to use ``wtp-bert-mini`` model, \
+            ``wtp-base`` to use ``wtp-canine-s-1l`` model, \
+            and ``wtp-large`` to use ``wtp-canine-s-12l`` model.
         * *whitespace+newline* - split by whitespaces and newline.
         * *whitespace* - split by whitespaces. Specifiaclly, with \
                          :class:`regex` pattern  ``r" +"``
     :Example:
 
     Split the text based on *whitespace*::
 
@@ -410,26 +423,89 @@
     elif engine == "thaisum":
         from pythainlp.tokenize.thaisumcut import (
             ThaiSentenceSegmentor as segmentor,
         )
 
         segment = segmentor()
         segments = segment.split_into_sentences(text)
+    elif engine.startswith("wtp"):
+        if "-" not in engine:
+            _size="mini"
+        else:
+            _size = engine.split("-")[-1]
+        from pythainlp.tokenize.wtsplit import tokenize as segment
+        segments = segment(text,size=_size,tokenize="sentence")
     else:
         raise ValueError(
             f"""Tokenizer \"{engine}\" not found.
             It might be a typo; if not, please consult our document."""
         )
 
     if not keep_whitespace:
         segments = strip_whitespace(segments)
 
     return segments
 
 
+def paragraph_tokenize(text: str, engine: str = "wtp-mini", paragraph_threshold:float=0.5) -> List[List[str]]:
+    """
+    Paragraph tokenizer.
+
+    Tokenizes text into paragraph.
+
+    :param str text: text to be tokenized
+    :param str engine: the name paragraph tokenizer
+    :return: list of paragraph
+    :rtype: List[List[str]]
+    **Options for engine**
+        * *wtp* - split by `wtpsplitaxe <https://github.com/bminixhofer/wtpsplit>`_., \
+            It support many size of models. You can use ``wtp`` to use mini model, \
+            ``wtp-tiny`` to use ``wtp-bert-tiny`` model (default), \
+            ``wtp-mini`` to use ``wtp-bert-mini`` model, \
+            ``wtp-base`` to use ``wtp-canine-s-1l`` model, \
+            and ``wtp-large`` to use ``wtp-canine-s-12l`` model.
+
+    :Example:
+
+    Split the text based on *wtp*::
+
+        from pythainlp.tokenize import paragraph_tokenize
+
+        sent = (
+            "(1) บทความนี้ผู้เขียนสังเคราะห์ขึ้นมาจากผลงานวิจัยที่เคยทำมาในอดีต"
+            +"  มิได้ทำการศึกษาค้นคว้าใหม่อย่างกว้างขวางแต่อย่างใด"
+            +" จึงใคร่ขออภัยในความบกพร่องทั้งปวงมา ณ ที่นี้"
+        )
+
+        paragraph_tokenize(sent)
+        # output: [
+        # ['(1) '], 
+        # [
+        #   'บทความนี้ผู้เขียนสังเคราะห์ขึ้นมาจากผลงานวิจัยที่เคยทำมาในอดีต  ',
+        #   'มิได้ทำการศึกษาค้นคว้าใหม่อย่างกว้างขวางแต่อย่างใด ',
+        #   'จึงใคร่ขออภัยในความบกพร่องทั้งปวงมา ',
+        #   'ณ ที่นี้'
+        # ]]
+    """
+    if engine.startswith("wtp"):
+        if "-" not in engine:
+            _size="mini"
+        else:
+            _size = engine.split("-")[-1]
+        from pythainlp.tokenize.wtsplit import tokenize as segment
+        segments = segment(text,size=_size,tokenize="paragraph",paragraph_threshold=paragraph_threshold)
+        
+    else:
+        raise ValueError(
+            f"""Tokenizer \"{engine}\" not found.
+            It might be a typo; if not, please consult our document."""
+        )
+    return segments
+
+
 def subword_tokenize(
     text: str,
     engine: str = DEFAULT_SUBWORD_TOKENIZE_ENGINE,
     keep_whitespace: bool = True,
 ) -> List[str]:
     """
     Subword tokenizer. Can be smaller than syllable.
```

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/crfcls.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/crfcls.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/crfcut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/crfcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/deepcut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/deepcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/etcc.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/etcc.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,14 @@
     Sarayut Paludkong, Supot Nitsuwat, and Para Limmaneepraserth.
     "Thai word segmentation using combination of forward and backward
     longest matching techniques." In International Symposium on Communications
     and Information Technology (ISCIT), pp. 37-40. 2001.
 
     :param str text: text to be tokenized to character clusters
     :return: list of clusters, tokenized from the text
-    :return: list[str]
+    :return: List[str]
     """
 
     if not text or not isinstance(text, str):
         return []
 
     return _cut_subword(_cut_etcc.word_tokenize(text))
```

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/longest.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/longest.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/multi_cut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/multi_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/nercut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/nercut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/newmm.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/newmm.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/nlpo3.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/nlpo3.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/oskut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/oskut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/pyicu.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/sefr_cut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/sefr_cut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/ssg.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/ssg.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/tcc.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/tcc.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/tcc_p.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/tcc_p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/thaisumcut.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/thaisumcut.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tokenize/tltk.py` & `pythainlp-4.1.0b1/pythainlp/tokenize/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tools/__init__.py` & `pythainlp-4.1.0b1/pythainlp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tools/misspell.py` & `pythainlp-4.1.0b1/pythainlp/tools/misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/tools/path.py` & `pythainlp-4.1.0b1/pythainlp/tools/path.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/translate/__init__.py` & `pythainlp-4.1.0b1/pythainlp/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/translate/core.py` & `pythainlp-4.1.0b1/pythainlp/translate/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,67 +13,64 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 class Translate:
     """
     Machine Translation
-
-    :param str src_lang: source language
-    :param str target_lang: target language
-    :param bool use_gpu: load model to gpu (Default is False)
-
-    **Options for source & target language**
-        * *th* - *en* - Thai to English
-        * *en* - *th* - English to Thai
-        * *th* - *zh* - Thai to Chinese
-        * *zh* - *th* - Chinese to Thai
-        * *th* - *fr* - Thai to French
-
-    :Example:
-
-    Translate text from Thai to English::
-
-        from pythainlp.translate import Translate
-        th2en = Translate('th', 'en')
-
-        th2en.translate("ฉันรักแมว")
-        # output: I love cat.
     """
 
     def __init__(
-        self, src_lang: str, target_lang: str, use_gpu: bool = False
+        self, src_lang: str, target_lang: str, engine: str="default", use_gpu: bool = False
     ) -> None:
         """
         :param str src_lang: source language
         :param str target_lang: target language
+        :param str engine: Machine Translation engine
         :param bool use_gpu: load model to gpu (Default is False)
 
+        **Options for engine*
+            * *default* - The engine default by each a language.
+            * *small100* - A multilingual machine translation model (covering 100 languages)
+
         **Options for source & target language**
             * *th* - *en* - Thai to English
             * *en* - *th* - English to Thai
             * *th* - *zh* - Thai to Chinese
             * *zh* - *th* - Chinese to Thai
             * *th* - *fr* - Thai to French
+            * *th* - *xx* - Thai to xx (xx is language code). It uses small100 model.
+            * *xx* - *th* - xx to Thai (xx is language code). It uses small100 model.
 
         :Example:
 
         Translate text from Thai to English::
 
             from pythainlp.translate import Translate
             th2en = Translate('th', 'en')
 
             th2en.translate("ฉันรักแมว")
             # output: I love cat.
         """
         self.model = None
-        self.load_model(src_lang, target_lang, use_gpu)
+        self.engine = engine
+        self.src_lang = src_lang
+        self.use_gpu = use_gpu
+        self.target_lang = target_lang
+        self.load_model()
+
+    def load_model(self):
+        src_lang = self.src_lang
+        target_lang = self.target_lang
+        use_gpu = self.use_gpu
+        if self.engine == "small100":
+            from .small100 import Small100Translator
 
-    def load_model(self, src_lang: str, target_lang: str, use_gpu: bool):
-        if src_lang == "th" and target_lang == "en":
+            self.model = Small100Translator(use_gpu)
+        elif src_lang == "th" and target_lang == "en":
             from pythainlp.translate.en_th import ThEnTranslator
 
             self.model = ThEnTranslator(use_gpu)
         elif src_lang == "en" and target_lang == "th":
             from pythainlp.translate.en_th import EnThTranslator
 
             self.model = EnThTranslator(use_gpu)
@@ -96,8 +93,10 @@
         """
         Translate text
 
         :param str text: input text in source language
         :return: translated text in target language
         :rtype: str
         """
+        if self.engine == "small100":
+            return self.model.translate(text, tgt_lang=self.target_lang)
         return self.model.translate(text)
```

### Comparing `pythainlp-4.0.2/pythainlp/translate/en_th.py` & `pythainlp-4.1.0b1/pythainlp/translate/en_th.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             data_name_or_path=_get_translate_path(
                 self._model_name,
                 _EN_TH_FILE_NAME,
                 "vocab",
             ),
         )
         if use_gpu:
-            self._model.cuda()
+            self._model = self._model.cuda()
 
     def translate(self, text: str) -> str:
         """
         Translate text from English to Thai
 
         :param str text: input text in source language
         :return: translated text in target language
```

### Comparing `pythainlp-4.0.2/pythainlp/translate/th_fr.py` & `pythainlp-4.1.0b1/pythainlp/translate/th_fr.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self,
         use_gpu: bool = False,
         pretrained: str = "Helsinki-NLP/opus-mt-th-fr",
     ) -> None:
         self.tokenizer_thzh = AutoTokenizer.from_pretrained(pretrained)
         self.model_thzh = AutoModelForSeq2SeqLM.from_pretrained(pretrained)
         if use_gpu:
-            self.model_thzh.cuda()
+            self.model_thzh = self.model_thzh.cuda()
 
     def translate(self, text: str) -> str:
         """
         Translate text from Thai to French
 
         :param str text: input text in source language
         :return: translated text in target language
```

### Comparing `pythainlp-4.0.2/pythainlp/translate/zh_th.py` & `pythainlp-4.1.0b1/pythainlp/translate/zh_th.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self,
         use_gpu: bool = False,
         pretrained: str = "Lalita/marianmt-th-zh_cn",
     ) -> None:
         self.tokenizer_thzh = AutoTokenizer.from_pretrained(pretrained)
         self.model_thzh = AutoModelForSeq2SeqLM.from_pretrained(pretrained)
         if use_gpu:
-            self.model_thzh.cuda()
+            self.model_thzh = self.model_thzh.cuda()
 
     def translate(self, text: str) -> str:
         """
         Translate text from Thai to Chinese
 
         :param str text: input text in source language
         :return: translated text in target language
```

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/__init__.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/core.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/ipa.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/ipa.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/iso_11940.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/iso_11940.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/lookup.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/lookup.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/pyicu.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/pyicu.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/royin.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/royin.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/spoonerism.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/spoonerism.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/thai2rom.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/thai2rom.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/thai2rom_onnx.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/thai2rom_onnx.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/thaig2p.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/thaig2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/tltk.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/tltk.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/w2p.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/w2p.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/transliterate/wunsen.py` & `pythainlp-4.1.0b1/pythainlp/transliterate/wunsen.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
                 (ราชบัณฑิตยสถาน พ.ศ. 2549)
             * *THC43* - for Mandarin เกณฑ์การถ่ายทอดเสียงภาษาจีนแมนดาริน
                 ด้วยอักขรวิธีไทย (คณะกรรมการสืบค้นประวัติศาสตร์ไทยในเอกสาร
                 ภาษาจีน พ.ศ. 2543)
 
         :Example:
         ::
+
             from pythainlp.transliterate.wunsen import WunsenTransliterate
 
             wt = WunsenTransliterate()
 
             wt.transliterate("ohayō", lang="jp")
             # output: 'โอฮาโย'
```

### Comparing `pythainlp-4.0.2/pythainlp/ulmfit/__init__.py` & `pythainlp-4.1.0b1/pythainlp/ulmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/ulmfit/core.py` & `pythainlp-4.1.0b1/pythainlp/ulmfit/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/ulmfit/preprocess.py` & `pythainlp-4.1.0b1/pythainlp/ulmfit/preprocess.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/ulmfit/tokenizer.py` & `pythainlp-4.1.0b1/pythainlp/ulmfit/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/__init__.py` & `pythainlp-4.1.0b1/pythainlp/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 """
 Utility functions, like date conversion and digit conversion
 """
 
 __all__ = [
     "Trie",
+    "abbreviation_to_full_text",
     "arabic_digit_to_thai_digit",
     "bahttext",
     "convert_years",
     "collate",
     "countthai",
     "count_thai_chars",
     "dict_trie",
@@ -61,14 +62,16 @@
     "words_to_num",
     "sound_syllable",
     "syllable_length",
     "syllable_open_close_detector",
     "nectec_to_ipa",
     "ipa_to_rtgs",
     "remove_tone_ipa",
+    "tis620_to_utf8",
+    "spell_words",
 ]
 
 from pythainlp.util.collate import collate
 from pythainlp.util.date import (
     now_reign_year,
     reign_year_to_ad,
     thaiword_to_date,
@@ -117,7 +120,10 @@
 from pythainlp.util.syllable import (
     sound_syllable,
     tone_detector,
     syllable_length,
     syllable_open_close_detector,
 )
 from pythainlp.util.phoneme import nectec_to_ipa, ipa_to_rtgs, remove_tone_ipa
+from pythainlp.util.encoding import tis620_to_utf8
+import pythainlp.util.spell_words as spell_words
+from pythainlp.util.abbreviation import abbreviation_to_full_text
```

### Comparing `pythainlp-4.0.2/pythainlp/util/collate.py` & `pythainlp-4.1.0b1/pythainlp/util/collate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/date.py` & `pythainlp-4.1.0b1/pythainlp/util/date.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/digitconv.py` & `pythainlp-4.1.0b1/pythainlp/util/digitconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/emojiconv.py` & `pythainlp-4.1.0b1/pythainlp/util/emojiconv.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/keyboard.py` & `pythainlp-4.1.0b1/pythainlp/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/keywords.py` & `pythainlp-4.1.0b1/pythainlp/util/keywords.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/normalize.py` & `pythainlp-4.1.0b1/pythainlp/util/normalize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/numtoword.py` & `pythainlp-4.1.0b1/pythainlp/util/numtoword.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/phoneme.py` & `pythainlp-4.1.0b1/pythainlp/util/phoneme.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/strftime.py` & `pythainlp-4.1.0b1/pythainlp/util/strftime.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/syllable.py` & `pythainlp-4.1.0b1/pythainlp/util/syllable.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/thai.py` & `pythainlp-4.1.0b1/pythainlp/util/thai.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/thaiwordcheck.py` & `pythainlp-4.1.0b1/pythainlp/util/thaiwordcheck.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/time.py` & `pythainlp-4.1.0b1/pythainlp/util/time.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/trie.py` & `pythainlp-4.1.0b1/pythainlp/util/trie.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/util/wordtonum.py` & `pythainlp-4.1.0b1/pythainlp/util/wordtonum.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/wangchanberta/__init__.py` & `pythainlp-4.1.0b1/pythainlp/wangchanberta/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/wangchanberta/core.py` & `pythainlp-4.1.0b1/pythainlp/wangchanberta/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/word_vector/__init__.py` & `pythainlp-4.1.0b1/pythainlp/word_vector/__init__.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp/word_vector/core.py` & `pythainlp-4.1.0b1/pythainlp/word_vector/core.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/pythainlp.egg-info/SOURCES.txt` & `pythainlp-4.1.0b1/pythainlp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,47 +22,60 @@
 pythainlp/augment/word2vec/__init__.py
 pythainlp/augment/word2vec/bpemb_wv.py
 pythainlp/augment/word2vec/core.py
 pythainlp/augment/word2vec/ltw2v.py
 pythainlp/augment/word2vec/thai2fit.py
 pythainlp/benchmarks/__init__.py
 pythainlp/benchmarks/word_tokenization.py
+pythainlp/chat/__init__.py
+pythainlp/chat/core.py
 pythainlp/cli/__init__.py
 pythainlp/cli/benchmark.py
 pythainlp/cli/data.py
 pythainlp/cli/soundex.py
 pythainlp/cli/tag.py
 pythainlp/cli/tokenize.py
+pythainlp/cls/__init__.py
+pythainlp/cls/param_free.py
+pythainlp/coref/__init__.py
+pythainlp/coref/_fastcoref.py
+pythainlp/coref/core.py
+pythainlp/coref/han_coref.py
 pythainlp/corpus/__init__.py
 pythainlp/corpus/common.py
 pythainlp/corpus/conceptnet.py
 pythainlp/corpus/core.py
 pythainlp/corpus/oscar.py
 pythainlp/corpus/th_en_translit.py
 pythainlp/corpus/tnc.py
 pythainlp/corpus/ttc.py
 pythainlp/corpus/util.py
 pythainlp/corpus/wordnet.py
+pythainlp/el/__init__.py
+pythainlp/el/_multiel.py
+pythainlp/el/core.py
 pythainlp/generate/__init__.py
 pythainlp/generate/core.py
 pythainlp/generate/thai2fit.py
+pythainlp/generate/wangchanglm.py
 pythainlp/khavee/__init__.py
 pythainlp/khavee/core.py
 pythainlp/khavee/example.py
 pythainlp/parse/__init__.py
 pythainlp/parse/core.py
 pythainlp/parse/esupar_engine.py
 pythainlp/parse/spacy_thai_engine.py
 pythainlp/parse/transformers_ud.py
 pythainlp/parse/ud_goeswith.py
 pythainlp/soundex/__init__.py
 pythainlp/soundex/core.py
 pythainlp/soundex/lk82.py
 pythainlp/soundex/metasound.py
 pythainlp/soundex/prayut_and_somchaip.py
+pythainlp/soundex/sound.py
 pythainlp/soundex/udom83.py
 pythainlp/spell/__init__.py
 pythainlp/spell/core.py
 pythainlp/spell/phunspell.py
 pythainlp/spell/pn.py
 pythainlp/spell/symspellpy.py
 pythainlp/spell/tltk.py
@@ -103,21 +116,24 @@
 pythainlp/tokenize/pyicu.py
 pythainlp/tokenize/sefr_cut.py
 pythainlp/tokenize/ssg.py
 pythainlp/tokenize/tcc.py
 pythainlp/tokenize/tcc_p.py
 pythainlp/tokenize/thaisumcut.py
 pythainlp/tokenize/tltk.py
+pythainlp/tokenize/wtsplit.py
 pythainlp/tools/__init__.py
 pythainlp/tools/misspell.py
 pythainlp/tools/path.py
 pythainlp/translate/__init__.py
 pythainlp/translate/core.py
 pythainlp/translate/en_th.py
+pythainlp/translate/small100.py
 pythainlp/translate/th_fr.py
+pythainlp/translate/tokenization_small100.py
 pythainlp/translate/zh_th.py
 pythainlp/transliterate/__init__.py
 pythainlp/transliterate/core.py
 pythainlp/transliterate/ipa.py
 pythainlp/transliterate/iso_11940.py
 pythainlp/transliterate/lookup.py
 pythainlp/transliterate/pyicu.py
@@ -130,39 +146,47 @@
 pythainlp/transliterate/w2p.py
 pythainlp/transliterate/wunsen.py
 pythainlp/ulmfit/__init__.py
 pythainlp/ulmfit/core.py
 pythainlp/ulmfit/preprocess.py
 pythainlp/ulmfit/tokenizer.py
 pythainlp/util/__init__.py
+pythainlp/util/abbreviation.py
 pythainlp/util/collate.py
 pythainlp/util/date.py
 pythainlp/util/digitconv.py
 pythainlp/util/emojiconv.py
+pythainlp/util/encoding.py
 pythainlp/util/keyboard.py
 pythainlp/util/keywords.py
 pythainlp/util/normalize.py
 pythainlp/util/numtoword.py
 pythainlp/util/phoneme.py
+pythainlp/util/spell_words.py
 pythainlp/util/strftime.py
 pythainlp/util/syllable.py
 pythainlp/util/thai.py
 pythainlp/util/thaiwordcheck.py
 pythainlp/util/time.py
 pythainlp/util/trie.py
 pythainlp/util/wordtonum.py
 pythainlp/wangchanberta/__init__.py
 pythainlp/wangchanberta/core.py
 pythainlp/word_vector/__init__.py
 pythainlp/word_vector/core.py
+pythainlp/wsd/__init__.py
+pythainlp/wsd/core.py
 tests/__init__.py
 tests/test_augment.py
 tests/test_benchmarks.py
 tests/test_cli.py
+tests/test_cls.py
+tests/test_coref.py
 tests/test_corpus.py
+tests/test_el.py
 tests/test_generate.py
 tests/test_khavee.py
 tests/test_misspell.py
 tests/test_parse.py
 tests/test_soundex.py
 tests/test_spell.py
 tests/test_summarize.py
@@ -171,12 +195,13 @@
 tests/test_tools.py
 tests/test_translate.py
 tests/test_transliterate.py
 tests/test_ulmfit.py
 tests/test_util.py
 tests/test_wangchanberta.py
 tests/test_word_vector.py
+tests/test_wsd.py
 tests/data/eval-details-input.json
 tests/data/eval-input.yml
 tests/data/input.txt
 tests/data/sentences.yml
 tests/data/test.txt
```

### Comparing `pythainlp-4.0.2/pythainlp.egg-info/requires.txt` & `pythainlp-4.1.0b1/pythainlp.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 requests>=2.22.0
 
 [:python_version < "3.9"]
 backports.zoneinfo
 
+[abbreviation]
+khamyo>=0.2.0
+
 [attacut]
 attacut>=1.0.6
 
 [benchmarks]
 PyYAML>=5.3.1
 numpy>=1.22
 pandas>=0.24
 
+[coreference_resolution]
+spacy>=3.0
+fastcoref>=2.1.5
+
 [dependency_parsing]
 spacy_thai>=0.7.1
 ufal.chu-liu-edmonds>=1.0.2
 transformers>=4.22.1
 
+[el]
+multiel>=0.5
+
 [esupar]
 esupar>=1.3.8
 numpy
 transformers>=4.22.1
 
 [full]
 PyYAML>=5.3.1
@@ -44,16 +54,22 @@
 spylls>=0.1.5
 symspellpy>=6.7.6
 oskut>=1.3
 nlpo3>=1.2.2
 onnxruntime>=1.10.0
 thai_nner
 wunsen>=0.0.3
+wtpsplit>=1.0.1
 spacy_thai>=0.7.1
+spacy>=3.0
+fastcoref>=2.1.5
 ufal.chu-liu-edmonds>=1.0.2
+panphon>=0.20.0
+sentence-transformers>=2.2.2
+khamyo>=0.2.0
 
 [generate]
 fastai<2.0
 
 [icu]
 pyicu>=2.3
 
@@ -120,12 +136,27 @@
 torch>=1.0.0
 transformers>=4.6.0
 
 [wangchanberta]
 transformers>=4.6.0
 sentencepiece>=0.1.91
 
+[wangchanglm]
+transformers>=4.6.0
+sentencepiece>=0.1.91
+pandas>=0.24
+
+[word_approximation]
+panphon>=0.20.0
+
 [wordnet]
 nltk>=3.3
 
+[wsd]
+sentence-transformers>=2.2.2
+
+[wtp]
+transformers>=4.6.0
+wtpsplit>=1.0.1
+
 [wunsen]
 wunsen>=0.0.1
```

### Comparing `pythainlp-4.0.2/setup.cfg` & `pythainlp-4.1.0b1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.0.1
+current_version = 4.1.0beta1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `pythainlp-4.0.2/setup.py` & `pythainlp-4.1.0b1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         "gensim>=4.0.0"
     ],
     "wangchanberta": [
         "transformers>=4.6.0",
         "sentencepiece>=0.1.91"
     ],
     "mt5": ["transformers>=4.6.0", "sentencepiece>=0.1.91"],
+    "wtp": ["transformers>=4.6.0", "wtpsplit>=1.0.1"],
     "wordnet": ["nltk>=3.3"],
     "generate": ["fastai<2.0"],
     "sefr_cut": ["sefr_cut>=1.1"],
     "spell": [
         "phunspell>=0.1.6",
         "spylls>=0.1.5",
         "symspellpy>=6.7.6"
@@ -105,14 +106,35 @@
         "transformers>=4.22.1",
     ],
     "dependency_parsing": [
         "spacy_thai>=0.7.1",
         "ufal.chu-liu-edmonds>=1.0.2",
         "transformers>=4.22.1",
     ],
+    "coreference_resolution":{
+        "spacy>=3.0",
+        "fastcoref>=2.1.5",
+    },
+    "word_approximation":{
+        "panphon>=0.20.0"
+    },
+    "wangchanglm": [
+        "transformers>=4.6.0",
+        "sentencepiece>=0.1.91",
+        "pandas>=0.24"
+    ],
+    "wsd":{
+        "sentence-transformers>=2.2.2"
+    },
+    "el":{
+        "multiel>=0.5"
+    },
+    "abbreviation":{
+        "khamyo>=0.2.0"
+    },
     "full": [
         "PyYAML>=5.3.1",
         "attacut>=1.0.4",
         "emoji>=0.5.1",
         "epitran>=1.1",
         "fairseq>=0.10.0",
         "gensim>=4.0.0",
@@ -132,22 +154,28 @@
         "spylls>=0.1.5",
         "symspellpy>=6.7.6",
         "oskut>=1.3",
         "nlpo3>=1.2.2",
         "onnxruntime>=1.10.0",
         "thai_nner",
         "wunsen>=0.0.3",
+        "wtpsplit>=1.0.1",
         "spacy_thai>=0.7.1",
+        "spacy>=3.0",
+        "fastcoref>=2.1.5",
         "ufal.chu-liu-edmonds>=1.0.2",
+        "panphon>=0.20.0",
+        "sentence-transformers>=2.2.2",
+        "khamyo>=0.2.0",
     ],
 }
 
 setup(
     name="pythainlp",
-    version="4.0.2",
+    version="4.1.0beta1",
     description="Thai Natural Language Processing library",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="PyThaiNLP",
     author_email="email@wannaphong.com",
     url="https://github.com/PyThaiNLP/pythainlp",
     packages=find_packages(exclude=["tests", "tests.*"]),
@@ -172,15 +200,15 @@
         "localization",
         "computational linguistics",
         "ThaiNLP",
         "Thai NLP",
         "Thai language",
     ],
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: Thai",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Text Processing",
         "Topic :: Text Processing :: General",
```

### Comparing `pythainlp-4.0.2/tests/data/eval-details-input.json` & `pythainlp-4.1.0b1/tests/data/eval-details-input.json`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/data/sentences.yml` & `pythainlp-4.1.0b1/tests/data/sentences.yml`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_augment.py` & `pythainlp-4.1.0b1/tests/test_augment.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_benchmarks.py` & `pythainlp-4.1.0b1/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_cli.py` & `pythainlp-4.1.0b1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_corpus.py` & `pythainlp-4.1.0b1/tests/test_corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     remove,
     thai_family_names,
     thai_female_names,
     thai_male_names,
     thai_negations,
     thai_stopwords,
     thai_syllables,
+    thai_synonym,
     thai_words,
     tnc,
     ttc,
     wordnet,
 )
 from pythainlp.corpus.util import revise_newmm_default_wordset
 from requests import Response
@@ -40,14 +41,15 @@
         self.assertIsInstance(thai_stopwords(), frozenset)
         self.assertIsInstance(thai_syllables(), frozenset)
         self.assertIsInstance(thai_words(), frozenset)
 
         self.assertIsInstance(countries(), frozenset)
         self.assertIsInstance(provinces(), frozenset)
         self.assertIsInstance(provinces(details=True), list)
+        self.assertIsInstance(thai_synonym(), dict)
         self.assertEqual(
             len(provinces(details=False)), len(provinces(details=True))
         )
         self.assertIsInstance(thai_family_names(), frozenset)
         self.assertIsInstance(list(thai_family_names())[0], str)
         self.assertIsInstance(thai_female_names(), frozenset)
         self.assertIsInstance(thai_male_names(), frozenset)
```

### Comparing `pythainlp-4.0.2/tests/test_generate.py` & `pythainlp-4.1.0b1/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_khavee.py` & `pythainlp-4.1.0b1/tests/test_khavee.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_misspell.py` & `pythainlp-4.1.0b1/tests/test_misspell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_parse.py` & `pythainlp-4.1.0b1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_soundex.py` & `pythainlp-4.1.0b1/tests/test_soundex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import unittest
 
 from pythainlp.soundex import lk82, metasound, soundex, udom83, prayut_and_somchaip
+from pythainlp.soundex.sound import word_approximation, audio_vector
 
 
 class TestSoundexPackage(unittest.TestCase):
     def test_soundex(self):
         self.assertIsNotNone(soundex("a", engine="lk82"))
         self.assertIsNotNone(soundex("a", engine="udom83"))
         self.assertIsNotNone(soundex("a", engine="metasound"))
@@ -69,7 +70,13 @@
         self.assertIsNotNone(prayut_and_somchaip("มอ"))
         self.assertIsNotNone(prayut_and_somchaip("รอ"))
         self.assertIsNotNone(prayut_and_somchaip("ขอ"))
         self.assertIsNotNone(prayut_and_somchaip("บน"))
         self.assertIsNotNone(prayut_and_somchaip("ณาญ"))
         self.assertIsNotNone(prayut_and_somchaip("กาง"))
         self.assertIsNotNone(prayut_and_somchaip("ว้าว"))
+
+    def test_word_approximation(self):
+        self.assertIsNotNone(word_approximation("รถ", ["รส","รด","คน"]))
+
+    def test_audio_vector(self):
+        self.assertIsNotNone(audio_vector("คน"))
```

### Comparing `pythainlp-4.0.2/tests/test_spell.py` & `pythainlp-4.1.0b1/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_summarize.py` & `pythainlp-4.1.0b1/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_tag.py` & `pythainlp-4.1.0b1/tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_tokenize.py` & `pythainlp-4.1.0b1/tests/test_tokenize.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     tcc,
     tcc_p,
     word_tokenize,
     sefr_cut,
     tltk,
     oskut,
     word_detokenize,
+    paragraph_tokenize,
 )
 from pythainlp.tokenize import clause_tokenize as sent_clause_tokenize
 from pythainlp.util import dict_trie
 
 
 class TestTokenizePackage(unittest.TestCase):
     def setUp(self):
@@ -302,25 +303,60 @@
         )
         self.assertIsNotNone(
             sent_tokenize(
                 sent_3,
                 engine="thaisum",
             ),
         )
+        self.assertIsNotNone(
+            sent_tokenize(
+                sent_3,
+                engine="wtp",
+            ),
+        )
+        self.assertIsNotNone(
+            sent_tokenize(
+                sent_3,
+                engine="wtp-tiny",
+            ),
+        )
+        # self.assertIsNotNone(
+        #     sent_tokenize(
+        #         sent_3,
+        #         engine="wtp-base",
+        #     ),
+        # )
+        # self.assertIsNotNone(
+        #     sent_tokenize(
+        #         sent_3,
+        #         engine="wtp-large",
+        #     ),
+        # )
         self.assertFalse(
             " "
             in sent_tokenize(
                 sent_1,
                 engine="whitespace",
                 keep_whitespace=False,
             )
         )
         with self.assertRaises(ValueError):
             sent_tokenize("ฉันไป กิน", engine="XX")  # engine does not exist
 
+    def test_paragraph_tokenize(self):
+        sent = (
+            "(1) บทความนี้ผู้เขียนสังเคราะห์ขึ้นมา"
+            + "จากผลงานวิจัยที่เคยทำมาในอดีต"
+            + " มิได้ทำการศึกษาค้นคว้าใหม่อย่างกว้างขวางแต่อย่างใด"
+            + " จึงใคร่ขออภัยในความบกพร่องทั้งปวงมา ณ ที่นี้"
+        )
+        self.assertIsNotNone(paragraph_tokenize(sent))
+        with self.assertRaises(ValueError):
+            paragraph_tokenize(sent, engine="ai2+2thai")
+
     def test_subword_tokenize(self):
         self.assertEqual(subword_tokenize(None), [])
         self.assertEqual(subword_tokenize(""), [])
         self.assertIsInstance(
             subword_tokenize("สวัสดีดาวอังคาร", engine="tcc"), list
         )
         self.assertFalse(
```

### Comparing `pythainlp-4.0.2/tests/test_translate.py` & `pythainlp-4.1.0b1/tests/test_translate.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,9 +69,21 @@
         )
         self.th_fr_translator = Translate('th', 'fr')
         self.assertIsNotNone(
             self.th_fr_translator.translate(
                 "ทดสอบระบบ",
             )
         )
+        self.th_fr_translator = Translate('th', 'fr', engine="small100")
+        self.assertIsNotNone(
+            self.th_fr_translator.translate(
+                "ทดสอบระบบ",
+            )
+        )
+        self.th_ja_translator = Translate('th', 'ja', engine="small100")
+        self.assertIsNotNone(
+            self.th_fr_translator.translate(
+                "ทดสอบระบบ",
+            )
+        )
         with self.assertRaises(ValueError):
-            self.th_cat_translator = Translate('th', 'cat')
+            self.th_cat_translator = Translate('th', 'cat', engine="fkfj")
```

### Comparing `pythainlp-4.0.2/tests/test_transliterate.py` & `pythainlp-4.1.0b1/tests/test_transliterate.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_ulmfit.py` & `pythainlp-4.1.0b1/tests/test_ulmfit.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_util.py` & `pythainlp-4.1.0b1/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections import Counter
 from datetime import datetime, time, timedelta, timezone
 
 from pythainlp.corpus import _CORPUS_PATH, thai_words
 from pythainlp.corpus.common import _THAI_WORDS_FILENAME
 from pythainlp.util import (
     Trie,
+    abbreviation_to_full_text,
     arabic_digit_to_thai_digit,
     bahttext,
     collate,
     countthai,
     count_thai_chars,
     dict_trie,
     display_thai_char,
@@ -53,15 +54,17 @@
     tone_detector,
     thai_word_tone_detector,
     convert_years,
     thai_strptime,
     nectec_to_ipa,
     ipa_to_rtgs,
     remove_tone_ipa,
+    tis620_to_utf8,
 )
+from pythainlp.util.spell_words import spell_word
 
 
 class TestUtilPackage(unittest.TestCase):
 
     # ### pythainlp.util.collate
 
     def test_collate(self):
@@ -836,7 +839,19 @@
     def test_ipa_to_rtgs(self):
         self.assertEqual(ipa_to_rtgs("kluaj"), "kluai")
         self.assertEqual(ipa_to_rtgs("waːw"), "wao")
         self.assertEqual(ipa_to_rtgs("/naː˥˩/"), "/na/")
 
     def test_remove_tone_ipa(self):
         self.assertEqual(remove_tone_ipa("laː˦˥.sa˨˩.maj˩˩˦"), "laː.sa.maj")
+
+    def test_tis620_to_utf8(self):
+        self.assertEqual(tis620_to_utf8("¡ÃÐ·ÃÇ§ÍØµÊÒË¡ÃÃÁ"), "กระทรวงอุตสาหกรรม")
+
+    def test_spell_word(self):
+        self.assertEqual(spell_word("เสือ"),['สอ', 'เอือ', 'เสือ'])
+        self.assertEqual(spell_word("เสื้อ"),['สอ', 'เอือ', 'ไม้โท', 'เสื้อ'])
+        self.assertEqual(spell_word("คน"),['คอ', 'นอ', 'คน'])
+        self.assertEqual(spell_word("คนดี"),['คอ', 'นอ', 'คน', 'ดอ', 'อี', 'ดี', 'คนดี'])
+    
+    def test_abbreviation_to_full_text(self):
+        self.assertIsInstance(abbreviation_to_full_text("รร.ของเราน่าอยู่", list))
```

### Comparing `pythainlp-4.0.2/tests/test_wangchanberta.py` & `pythainlp-4.1.0b1/tests/test_wangchanberta.py`

 * *Files identical despite different names*

### Comparing `pythainlp-4.0.2/tests/test_word_vector.py` & `pythainlp-4.1.0b1/tests/test_word_vector.py`

 * *Files identical despite different names*

