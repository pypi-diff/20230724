# Comparing `tmp/ekonlpy-1.2.0.tar.gz` & `tmp/ekonlpy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekonlpy-1.2.0.tar", max compression
+gzip compressed data, was "ekonlpy-2.0.0.tar", max compression
```

## Comparing `ekonlpy-1.2.0.tar` & `ekonlpy-2.0.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1071 2023-07-24 04:02:40.128115 ekonlpy-1.2.0/LICENSE
--rw-r--r--   0        0        0     8760 2023-07-24 04:02:40.128115 ekonlpy-1.2.0/README.md
--rw-r--r--   0        0        0     3576 2023-07-24 04:03:16.398296 ekonlpy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1060 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/__cli__.py
--rw-r--r--   0        0        0      388 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/__init__.py
--rw-r--r--   0        0        0       22 2023-07-24 04:03:16.326292 ekonlpy-1.2.0/src/ekonlpy/_version.py
--rw-r--r--   0        0        0       53 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/base/__init__.py
--rw-r--r--   0        0        0     1079 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/base/base.py
--rw-r--r--   0        0        0       31 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/__init__.py
--rw-r--r--   0        0        0      514 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ADJECTIVES.txt
--rw-r--r--   0        0        0      108 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ADVERBS.txt
--rw-r--r--   0        0        0     2583 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/COUNTRY.txt
--rw-r--r--   0        0        0       17 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/CURRENCY.txt
--rw-r--r--   0        0        0    47727 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
--rw-r--r--   0        0        0   475773 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_TERMS.txt
--rwxr-xr-x   0        0        0    77542 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ENTITY.txt
--rw-r--r--   0        0        0     9629 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
--rw-r--r--   0        0        0     2077 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/GENERIC.txt
--rw-r--r--   0        0        0    35442 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
--rw-r--r--   0        0        0    69192 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INSTITUTION.txt
--rw-r--r--   0        0        0    20594 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/LEMMA.txt
--rw-r--r--   0        0        0     2072 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NAMES.txt
--rw-r--r--   0        0        0      687 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NOUNS.txt
--rw-r--r--   0        0        0    10396 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
--rw-r--r--   0        0        0    12378 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
--rw-r--r--   0        0        0    14928 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SECTOR.txt
--rw-r--r--   0        0        0     6456 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS.txt
--rwxr-xr-x   0        0        0      260 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
--rw-r--r--   0        0        0     5788 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
--rwxr-xr-x   0        0        0      598 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
--rw-r--r--   0        0        0    33685 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM.txt
--rw-r--r--   0        0        0      300 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
--rw-r--r--   0        0        0     5329 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
--rw-r--r--   0        0        0    27207 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
--rw-r--r--   0        0        0       87 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
--rw-r--r--   0        0        0       69 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/UNIT.txt
--rw-r--r--   0        0        0       40 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/VERBS.txt
--rwxr-xr-x   0        0        0     1677 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Currencies.txt
--rwxr-xr-x   0        0        0      724 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/DatesandNumbers.txt
--rwxr-xr-x   0        0        0     1798 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Generic.txt
--rwxr-xr-x   0        0        0     1622 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Geographic.txt
--rwxr-xr-x   0        0        0  2903900 2023-07-24 04:02:40.248116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/HIV-4.csv
--rwxr-xr-x   0        0        0  8373373 2023-07-24 04:02:40.296116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/LM.csv
--rwxr-xr-x   0        0        0    93474 2023-07-24 04:02:40.300116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Names.txt
--rw-r--r--   0        0        0  3047832 2023-07-24 04:02:40.316116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
--rw-r--r--   0        0        0  2362210 2023-07-24 04:02:40.328116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
--rwxr-xr-x   0        0        0   778128 2023-07-24 04:02:40.332116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
--rwxr-xr-x   0        0        0   661841 2023-07-24 04:02:40.336116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/intensity.csv
--rwxr-xr-x   0        0        0   659879 2023-07-24 04:02:40.340116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/polarity.csv
--rw-r--r--   0        0        0  3226022 2023-07-24 04:02:40.360116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
--rw-r--r--   0        0        0  3832440 2023-07-24 04:02:40.380117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
--rw-r--r--   0        0        0  2735025 2023-07-24 04:02:40.396117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
--rw-r--r--   0        0        0  3749409 2023-07-24 04:02:40.416117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
--rw-r--r--   0        0        0  2835691 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
--rw-r--r--   0        0        0    36419 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
--rw-r--r--   0        0        0   281858 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/model/MPKC.nbc
--rw-r--r--   0        0        0    15644 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/tagset.py
--rw-r--r--   0        0        0       58 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/etag/__init__.py
--rw-r--r--   0        0        0     4174 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/etag/_template.py
--rwxr-xr-x   0        0        0      102 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/mecab/__init__.py
--rw-r--r--   0        0        0     6113 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/mecab/_mecab.py
--rw-r--r--   0        0        0     5133 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/mecab/_userdic.py
--rw-r--r--   0        0        0        0 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/py.typed
--rwxr-xr-x   0        0        0      293 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/__init__.py
--rwxr-xr-x   0        0        0     4024 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/base.py
--rwxr-xr-x   0        0        0     1713 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/euko.py
--rwxr-xr-x   0        0        0      906 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/hiv4.py
--rw-r--r--   0        0        0     5665 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/kosac.py
--rwxr-xr-x   0        0        0      950 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/lm.py
--rw-r--r--   0        0        0    15729 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/mpck.py
--rwxr-xr-x   0        0        0     1812 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/mpko.py
--rwxr-xr-x   0        0        0     8992 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/utils.py
--rw-r--r--   0        0        0      104 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/tag/__init__.py
--rw-r--r--   0        0        0    12575 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/tag/_mecab.py
--rw-r--r--   0        0        0     2171 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/tag/_postprocess.py
--rwxr-xr-x   0        0        0        0 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/utils/__init__.py
--rw-r--r--   0        0        0     3481 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/utils/dictionary.py
--rw-r--r--   0        0        0     6426 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/utils/io.py
--rw-r--r--   0        0        0     9695 1970-01-01 00:00:00.000000 ekonlpy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 04:16:30.939303 ekonlpy-2.0.0/LICENSE
+-rw-r--r--   0        0        0     9198 2023-07-24 04:16:30.939303 ekonlpy-2.0.0/README.md
+-rw-r--r--   0        0        0     3576 2023-07-24 04:17:05.931410 ekonlpy-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1060 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/__cli__.py
+-rw-r--r--   0        0        0      388 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 04:17:05.863410 ekonlpy-2.0.0/src/ekonlpy/_version.py
+-rw-r--r--   0        0        0       53 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/base/__init__.py
+-rw-r--r--   0        0        0     1079 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/base/base.py
+-rw-r--r--   0        0        0       31 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/data/__init__.py
+-rw-r--r--   0        0        0      514 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ADJECTIVES.txt
+-rw-r--r--   0        0        0      108 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ADVERBS.txt
+-rw-r--r--   0        0        0     2583 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/COUNTRY.txt
+-rw-r--r--   0        0        0       17 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/CURRENCY.txt
+-rw-r--r--   0        0        0    47727 2023-07-24 04:16:31.031304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
+-rw-r--r--   0        0        0   475773 2023-07-24 04:16:31.043304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ECON_TERMS.txt
+-rwxr-xr-x   0        0        0    77542 2023-07-24 04:16:31.043304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ENTITY.txt
+-rw-r--r--   0        0        0     9629 2023-07-24 04:16:31.043304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
+-rw-r--r--   0        0        0     2077 2023-07-24 04:16:31.043304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/GENERIC.txt
+-rw-r--r--   0        0        0    35442 2023-07-24 04:16:31.043304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
+-rw-r--r--   0        0        0    69192 2023-07-24 04:16:31.043304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/INSTITUTION.txt
+-rw-r--r--   0        0        0    20594 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/LEMMA.txt
+-rw-r--r--   0        0        0     2072 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/NAMES.txt
+-rw-r--r--   0        0        0      687 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/NOUNS.txt
+-rw-r--r--   0        0        0    10396 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
+-rw-r--r--   0        0        0    12378 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
+-rw-r--r--   0        0        0    14928 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SECTOR.txt
+-rw-r--r--   0        0        0     6456 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS.txt
+-rwxr-xr-x   0        0        0      260 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
+-rw-r--r--   0        0        0     5788 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
+-rwxr-xr-x   0        0        0      598 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
+-rw-r--r--   0        0        0    33685 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM.txt
+-rw-r--r--   0        0        0      300 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
+-rw-r--r--   0        0        0     5329 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
+-rw-r--r--   0        0        0    27207 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
+-rw-r--r--   0        0        0       87 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
+-rw-r--r--   0        0        0       69 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/UNIT.txt
+-rw-r--r--   0        0        0       40 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/dictionary/VERBS.txt
+-rwxr-xr-x   0        0        0     1677 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Currencies.txt
+-rwxr-xr-x   0        0        0      724 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/DatesandNumbers.txt
+-rwxr-xr-x   0        0        0     1798 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Generic.txt
+-rwxr-xr-x   0        0        0     1622 2023-07-24 04:16:31.047304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Geographic.txt
+-rwxr-xr-x   0        0        0  2903900 2023-07-24 04:16:31.059304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/HIV-4.csv
+-rwxr-xr-x   0        0        0  8373373 2023-07-24 04:16:31.099304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/LM.csv
+-rwxr-xr-x   0        0        0    93474 2023-07-24 04:16:31.103304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Names.txt
+-rw-r--r--   0        0        0  3047832 2023-07-24 04:16:31.119304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
+-rw-r--r--   0        0        0  2362210 2023-07-24 04:16:31.131304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
+-rwxr-xr-x   0        0        0   778128 2023-07-24 04:16:31.131304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
+-rwxr-xr-x   0        0        0   661841 2023-07-24 04:16:31.135304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/kosac/intensity.csv
+-rwxr-xr-x   0        0        0   659879 2023-07-24 04:16:31.139304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/kosac/polarity.csv
+-rw-r--r--   0        0        0  3226022 2023-07-24 04:16:31.155304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
+-rw-r--r--   0        0        0  3832440 2023-07-24 04:16:31.171304 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
+-rw-r--r--   0        0        0  2735025 2023-07-24 04:16:31.187305 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
+-rw-r--r--   0        0        0  3749409 2023-07-24 04:16:31.207305 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
+-rw-r--r--   0        0        0  2835691 2023-07-24 04:16:31.215305 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
+-rw-r--r--   0        0        0    36419 2023-07-24 04:16:31.215305 ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
+-rw-r--r--   0        0        0   281858 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/data/model/MPKC.nbc
+-rw-r--r--   0        0        0    15644 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/data/tagset.py
+-rw-r--r--   0        0        0       58 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/etag/__init__.py
+-rw-r--r--   0        0        0     4174 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/etag/_template.py
+-rwxr-xr-x   0        0        0      102 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/mecab/__init__.py
+-rw-r--r--   0        0        0     6113 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/mecab/_mecab.py
+-rw-r--r--   0        0        0     5133 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/mecab/_userdic.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/py.typed
+-rwxr-xr-x   0        0        0      293 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/__init__.py
+-rwxr-xr-x   0        0        0     4024 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/base.py
+-rwxr-xr-x   0        0        0     1713 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/euko.py
+-rwxr-xr-x   0        0        0      906 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/hiv4.py
+-rw-r--r--   0        0        0     5665 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/kosac.py
+-rwxr-xr-x   0        0        0      950 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/lm.py
+-rw-r--r--   0        0        0    15729 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/mpck.py
+-rwxr-xr-x   0        0        0     1812 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/mpko.py
+-rwxr-xr-x   0        0        0     8992 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/sentiment/utils.py
+-rw-r--r--   0        0        0      104 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/tag/__init__.py
+-rw-r--r--   0        0        0    12575 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/tag/_mecab.py
+-rw-r--r--   0        0        0     2171 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/tag/_postprocess.py
+-rwxr-xr-x   0        0        0        0 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/utils/__init__.py
+-rw-r--r--   0        0        0     3481 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/utils/dictionary.py
+-rw-r--r--   0        0        0     6426 2023-07-24 04:16:31.219305 ekonlpy-2.0.0/src/ekonlpy/utils/io.py
+-rw-r--r--   0        0        0    10133 1970-01-01 00:00:00.000000 ekonlpy-2.0.0/PKG-INFO
```

### Comparing `ekonlpy-1.2.0/LICENSE` & `ekonlpy-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/README.md` & `ekonlpy-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
 
 <!-- Links: -->
 
 `eKoNLPy` is a Korean Natural Language Processing (NLP) Python library specifically designed for economic analysis. It extends the functionality of the `MeCab` tagger from KoNLPy to improve the handling of economic terms, financial institutions, and company names, classifying them as single nouns. Additionally, it incorporates sentiment analysis features to determine the tone of monetary policy statements, such as Hawkish or Dovish.
 
 > **Note**
 >
+> From the version 2.0.0, eKoNLPy intergrate the extended tagger with the original tagger. If you want to use the original tagger, please set `use_original_tagger=True` when you create the instance of `Mecab` class. Additionally, the `Mecab` class can be directly imported from `ekonlpy` module. The default input text parameter of `Mecab.pos()` is changed from `phrase` to `text` to be consistent with the original tagger.
+
+> **Note**
+>
 > eKoNLPy is built on the [fugashi](https://github.com/polm/fugashi) and [mecab-ko-dic](https://github.com/LuminosoInsight/mecab-ko-dic) libraries. For more information on using the `Mecab` tagger, please refer to the [fugashi documentation](https://github.com/polm/fugashi). As eKoNLPy no longer relies on the [KoNLPy](https://konlpy.org) library, Java is not required for its use. This makes eKoNLPy compatible with Windows, Linux, and Mac OS, without the need for Java installation. You can also use eKoNLPy on Google Colab.
 
 If you wish to tokenize general Korean text with eKoNLPy, you do not need to install the `KoNLPy` library. Instead, utilize `ekonlpy.mecab.MeCab` as a replacement for `ekonlpy.tag.Mecab`.
 
 However, if you plan to use the [Korean Sentiment Analyzer (KSA)](#korean-sentiment-analyzer-ksa), which employs the `Kkma` morpheme analyzer, you will need to install the [KoNLPy](https://konlpy.org) library.
 
 ## Installation
```

### Comparing `ekonlpy-1.2.0/pyproject.toml` & `ekonlpy-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eKoNLPy"
-version = "1.2.0"
+version = "2.0.0"
 description = "A Korean natural language processing toolkit for economic analysis"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ekonlpy", from = "src" }]
 homepage = "https://ekonlpy.entelecheia.ai/"
 repository = "https://github.com/entelecheia/eKoNLPy"
```

### Comparing `ekonlpy-1.2.0/src/ekonlpy/__cli__.py` & `ekonlpy-2.0.0/src/ekonlpy/__cli__.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/base/base.py` & `ekonlpy-2.0.0/src/ekonlpy/base/base.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ADJECTIVES.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ADJECTIVES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/COUNTRY.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/COUNTRY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_PHRASES.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ECON_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_TERMS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ECON_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ENTITY.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/ENTITY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/GENERIC.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/GENERIC.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INSTITUTION.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/INSTITUTION.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/LEMMA.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/LEMMA.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NAMES.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/NAMES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NOUNS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SECTOR.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SECTOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Currencies.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Currencies.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/DatesandNumbers.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/DatesandNumbers.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Generic.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Generic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Geographic.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Geographic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/HIV-4.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/HIV-4.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/LM.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/LM.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Names.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/Names.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/expressive-type.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/kosac/expressive-type.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/intensity.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/kosac/intensity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/polarity.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/kosac/polarity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt` & `ekonlpy-2.0.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/model/MPKC.nbc` & `ekonlpy-2.0.0/src/ekonlpy/data/model/MPKC.nbc`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/data/tagset.py` & `ekonlpy-2.0.0/src/ekonlpy/data/tagset.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/etag/_template.py` & `ekonlpy-2.0.0/src/ekonlpy/etag/_template.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/mecab/_mecab.py` & `ekonlpy-2.0.0/src/ekonlpy/mecab/_mecab.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/mecab/_userdic.py` & `ekonlpy-2.0.0/src/ekonlpy/mecab/_userdic.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/base.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/base.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/euko.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/euko.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/hiv4.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/hiv4.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/kosac.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/kosac.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/lm.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/lm.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/mpck.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/mpck.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/mpko.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/mpko.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/sentiment/utils.py` & `ekonlpy-2.0.0/src/ekonlpy/sentiment/utils.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/tag/_mecab.py` & `ekonlpy-2.0.0/src/ekonlpy/tag/_mecab.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/tag/_postprocess.py` & `ekonlpy-2.0.0/src/ekonlpy/tag/_postprocess.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/utils/dictionary.py` & `ekonlpy-2.0.0/src/ekonlpy/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/src/ekonlpy/utils/io.py` & `ekonlpy-2.0.0/src/ekonlpy/utils/io.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.2.0/PKG-INFO` & `ekonlpy-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ekonlpy
-Version: 1.2.0
+Version: 2.0.0
 Summary: A Korean natural language processing toolkit for economic analysis
 Home-page: https://ekonlpy.entelecheia.ai/
 License: MIT
 Keywords: KoNLPy,Tokenization,Sentiment analysis,Monetary policy
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
@@ -54,14 +54,18 @@
 
 <!-- Links: -->
 
 `eKoNLPy` is a Korean Natural Language Processing (NLP) Python library specifically designed for economic analysis. It extends the functionality of the `MeCab` tagger from KoNLPy to improve the handling of economic terms, financial institutions, and company names, classifying them as single nouns. Additionally, it incorporates sentiment analysis features to determine the tone of monetary policy statements, such as Hawkish or Dovish.
 
 > **Note**
 >
+> From the version 2.0.0, eKoNLPy intergrate the extended tagger with the original tagger. If you want to use the original tagger, please set `use_original_tagger=True` when you create the instance of `Mecab` class. Additionally, the `Mecab` class can be directly imported from `ekonlpy` module. The default input text parameter of `Mecab.pos()` is changed from `phrase` to `text` to be consistent with the original tagger.
+
+> **Note**
+>
 > eKoNLPy is built on the [fugashi](https://github.com/polm/fugashi) and [mecab-ko-dic](https://github.com/LuminosoInsight/mecab-ko-dic) libraries. For more information on using the `Mecab` tagger, please refer to the [fugashi documentation](https://github.com/polm/fugashi). As eKoNLPy no longer relies on the [KoNLPy](https://konlpy.org) library, Java is not required for its use. This makes eKoNLPy compatible with Windows, Linux, and Mac OS, without the need for Java installation. You can also use eKoNLPy on Google Colab.
 
 If you wish to tokenize general Korean text with eKoNLPy, you do not need to install the `KoNLPy` library. Instead, utilize `ekonlpy.mecab.MeCab` as a replacement for `ekonlpy.tag.Mecab`.
 
 However, if you plan to use the [Korean Sentiment Analyzer (KSA)](#korean-sentiment-analyzer-ksa), which employs the `Kkma` morpheme analyzer, you will need to install the [KoNLPy](https://konlpy.org) library.
 
 ## Installation
```

