# Comparing `tmp/ekonlpy-1.1.7.tar.gz` & `tmp/ekonlpy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ekonlpy-1.1.7.tar", max compression
+gzip compressed data, was "ekonlpy-1.2.0.tar", max compression
```

## Comparing `ekonlpy-1.1.7.tar` & `ekonlpy-1.2.0.tar`

### file list

```diff
@@ -1,76 +1,79 @@
--rw-r--r--   0        0        0     1071 2023-04-26 19:28:57.344443 ekonlpy-1.1.7/LICENSE
--rw-r--r--   0        0        0     8562 2023-04-26 19:28:57.348444 ekonlpy-1.1.7/README.md
--rw-r--r--   0        0        0     3469 2023-04-26 19:29:37.960735 ekonlpy-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/__init__.py
--rw-r--r--   0        0        0       22 2023-04-26 19:29:37.888735 ekonlpy-1.1.7/src/ekonlpy/_version.py
--rw-r--r--   0        0        0       31 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/__init__.py
--rw-r--r--   0        0        0      514 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ADJECTIVES.txt
--rw-r--r--   0        0        0      108 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ADVERBS.txt
--rw-r--r--   0        0        0     2583 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/COUNTRY.txt
--rw-r--r--   0        0        0       17 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/CURRENCY.txt
--rw-r--r--   0        0        0    47727 2023-04-26 19:28:57.444444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
--rw-r--r--   0        0        0   475773 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_TERMS.txt
--rwxr-xr-x   0        0        0    77542 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ENTITY.txt
--rw-r--r--   0        0        0     9629 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
--rw-r--r--   0        0        0     2077 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/GENERIC.txt
--rw-r--r--   0        0        0    35442 2023-04-26 19:28:57.452444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
--rw-r--r--   0        0        0    69192 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INSTITUTION.txt
--rw-r--r--   0        0        0    20594 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/LEMMA.txt
--rw-r--r--   0        0        0     2072 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NAMES.txt
--rw-r--r--   0        0        0      687 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NOUNS.txt
--rw-r--r--   0        0        0    10396 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
--rw-r--r--   0        0        0    12378 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
--rw-r--r--   0        0        0    14928 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SECTOR.txt
--rw-r--r--   0        0        0     6456 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS.txt
--rwxr-xr-x   0        0        0      260 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
--rw-r--r--   0        0        0     5788 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
--rwxr-xr-x   0        0        0      598 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
--rw-r--r--   0        0        0    33685 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM.txt
--rw-r--r--   0        0        0      300 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
--rw-r--r--   0        0        0     5329 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
--rw-r--r--   0        0        0    27207 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
--rw-r--r--   0        0        0       87 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
--rw-r--r--   0        0        0       69 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/UNIT.txt
--rw-r--r--   0        0        0       40 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/dictionary/VERBS.txt
--rwxr-xr-x   0        0        0     1677 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Currencies.txt
--rwxr-xr-x   0        0        0      724 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/DatesandNumbers.txt
--rwxr-xr-x   0        0        0     1798 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Generic.txt
--rwxr-xr-x   0        0        0     1622 2023-04-26 19:28:57.456444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Geographic.txt
--rwxr-xr-x   0        0        0  2903900 2023-04-26 19:28:57.468444 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/HIV-4.csv
--rwxr-xr-x   0        0        0  8373373 2023-04-26 19:28:57.516445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/LM.csv
--rwxr-xr-x   0        0        0    93474 2023-04-26 19:28:57.516445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Names.txt
--rw-r--r--   0        0        0  3047832 2023-04-26 19:28:57.532445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
--rw-r--r--   0        0        0  2362210 2023-04-26 19:28:57.544445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
--rwxr-xr-x   0        0        0   778128 2023-04-26 19:28:57.548445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
--rwxr-xr-x   0        0        0   661841 2023-04-26 19:28:57.552445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/intensity.csv
--rwxr-xr-x   0        0        0   659879 2023-04-26 19:28:57.556445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/polarity.csv
--rw-r--r--   0        0        0  3226022 2023-04-26 19:28:57.572445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
--rw-r--r--   0        0        0  3832440 2023-04-26 19:28:57.592445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
--rw-r--r--   0        0        0  2735025 2023-04-26 19:28:57.608445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
--rw-r--r--   0        0        0  3749409 2023-04-26 19:28:57.628445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
--rw-r--r--   0        0        0  2835691 2023-04-26 19:28:57.640445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
--rw-r--r--   0        0        0    36419 2023-04-26 19:28:57.640445 ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
--rw-r--r--   0        0        0   281858 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/data/model/MPKC.nbc
--rw-r--r--   0        0        0    15644 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/data/tagset.py
--rw-r--r--   0        0        0       33 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/etag/__init__.py
--rw-r--r--   0        0        0     4210 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/etag/_template.py
--rwxr-xr-x   0        0        0       63 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/mecab/__init__.py
--rw-r--r--   0        0        0     5687 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/mecab/_mecab.py
--rw-r--r--   0        0        0     4529 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/mecab/_userdic.py
--rw-r--r--   0        0        0        0 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/py.typed
--rwxr-xr-x   0        0        0      236 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/__init__.py
--rwxr-xr-x   0        0        0     4149 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/base.py
--rwxr-xr-x   0        0        0     1741 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/euko.py
--rwxr-xr-x   0        0        0     1010 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/hiv4.py
--rw-r--r--   0        0        0     5936 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/kosac.py
--rwxr-xr-x   0        0        0     1054 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/lm.py
--rw-r--r--   0        0        0    16112 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/mpck.py
--rwxr-xr-x   0        0        0     1840 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/mpko.py
--rwxr-xr-x   0        0        0     9268 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/sentiment/utils.py
--rw-r--r--   0        0        0       66 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/tag/__init__.py
--rw-r--r--   0        0        0    10630 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/tag/_mecab.py
--rw-r--r--   0        0        0     2172 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/tag/_postprocess.py
--rwxr-xr-x   0        0        0        0 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/utils/__init__.py
--rw-r--r--   0        0        0     3520 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/utils/dictionary.py
--rw-r--r--   0        0        0     6668 2023-04-26 19:28:57.644445 ekonlpy-1.1.7/src/ekonlpy/utils/io.py
--rw-r--r--   0        0        0     9459 1970-01-01 00:00:00.000000 ekonlpy-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-24 04:02:40.128115 ekonlpy-1.2.0/LICENSE
+-rw-r--r--   0        0        0     8760 2023-07-24 04:02:40.128115 ekonlpy-1.2.0/README.md
+-rw-r--r--   0        0        0     3576 2023-07-24 04:03:16.398296 ekonlpy-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1060 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/__cli__.py
+-rw-r--r--   0        0        0      388 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-24 04:03:16.326292 ekonlpy-1.2.0/src/ekonlpy/_version.py
+-rw-r--r--   0        0        0       53 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/base/__init__.py
+-rw-r--r--   0        0        0     1079 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/base/base.py
+-rw-r--r--   0        0        0       31 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/__init__.py
+-rw-r--r--   0        0        0      514 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ADJECTIVES.txt
+-rw-r--r--   0        0        0      108 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ADVERBS.txt
+-rw-r--r--   0        0        0     2583 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/COUNTRY.txt
+-rw-r--r--   0        0        0       17 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/CURRENCY.txt
+-rw-r--r--   0        0        0    47727 2023-07-24 04:02:40.224115 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_PHRASES.txt
+-rw-r--r--   0        0        0   475773 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_TERMS.txt
+-rwxr-xr-x   0        0        0    77542 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ENTITY.txt
+-rw-r--r--   0        0        0     9629 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt
+-rw-r--r--   0        0        0     2077 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/GENERIC.txt
+-rw-r--r--   0        0        0    35442 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt
+-rw-r--r--   0        0        0    69192 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INSTITUTION.txt
+-rw-r--r--   0        0        0    20594 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/LEMMA.txt
+-rw-r--r--   0        0        0     2072 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NAMES.txt
+-rw-r--r--   0        0        0      687 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NOUNS.txt
+-rw-r--r--   0        0        0    10396 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt
+-rw-r--r--   0        0        0    12378 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt
+-rw-r--r--   0        0        0    14928 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SECTOR.txt
+-rw-r--r--   0        0        0     6456 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS.txt
+-rwxr-xr-x   0        0        0      260 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_CUST.txt
+-rw-r--r--   0        0        0     5788 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt
+-rwxr-xr-x   0        0        0      598 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt
+-rw-r--r--   0        0        0    33685 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM.txt
+-rw-r--r--   0        0        0      300 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_MAG.txt
+-rw-r--r--   0        0        0     5329 2023-07-24 04:02:40.236116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt
+-rw-r--r--   0        0        0    27207 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt
+-rw-r--r--   0        0        0       87 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_VA.txt
+-rw-r--r--   0        0        0       69 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/UNIT.txt
+-rw-r--r--   0        0        0       40 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/dictionary/VERBS.txt
+-rwxr-xr-x   0        0        0     1677 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Currencies.txt
+-rwxr-xr-x   0        0        0      724 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/DatesandNumbers.txt
+-rwxr-xr-x   0        0        0     1798 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Generic.txt
+-rwxr-xr-x   0        0        0     1622 2023-07-24 04:02:40.240116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Geographic.txt
+-rwxr-xr-x   0        0        0  2903900 2023-07-24 04:02:40.248116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/HIV-4.csv
+-rwxr-xr-x   0        0        0  8373373 2023-07-24 04:02:40.296116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/LM.csv
+-rwxr-xr-x   0        0        0    93474 2023-07-24 04:02:40.300116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Names.txt
+-rw-r--r--   0        0        0  3047832 2023-07-24 04:02:40.316116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv
+-rw-r--r--   0        0        0  2362210 2023-07-24 04:02:40.328116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv
+-rwxr-xr-x   0        0        0   778128 2023-07-24 04:02:40.332116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/expressive-type.csv
+-rwxr-xr-x   0        0        0   661841 2023-07-24 04:02:40.336116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/intensity.csv
+-rwxr-xr-x   0        0        0   659879 2023-07-24 04:02:40.340116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/polarity.csv
+-rw-r--r--   0        0        0  3226022 2023-07-24 04:02:40.360116 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv
+-rw-r--r--   0        0        0  3832440 2023-07-24 04:02:40.380117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv
+-rw-r--r--   0        0        0  2735025 2023-07-24 04:02:40.396117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv
+-rw-r--r--   0        0        0  3749409 2023-07-24 04:02:40.416117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv
+-rw-r--r--   0        0        0  2835691 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt
+-rw-r--r--   0        0        0    36419 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt
+-rw-r--r--   0        0        0   281858 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/model/MPKC.nbc
+-rw-r--r--   0        0        0    15644 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/data/tagset.py
+-rw-r--r--   0        0        0       58 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/etag/__init__.py
+-rw-r--r--   0        0        0     4174 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/etag/_template.py
+-rwxr-xr-x   0        0        0      102 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/mecab/__init__.py
+-rw-r--r--   0        0        0     6113 2023-07-24 04:02:40.428117 ekonlpy-1.2.0/src/ekonlpy/mecab/_mecab.py
+-rw-r--r--   0        0        0     5133 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/mecab/_userdic.py
+-rw-r--r--   0        0        0        0 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/py.typed
+-rwxr-xr-x   0        0        0      293 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/__init__.py
+-rwxr-xr-x   0        0        0     4024 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/base.py
+-rwxr-xr-x   0        0        0     1713 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/euko.py
+-rwxr-xr-x   0        0        0      906 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/hiv4.py
+-rw-r--r--   0        0        0     5665 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/kosac.py
+-rwxr-xr-x   0        0        0      950 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/lm.py
+-rw-r--r--   0        0        0    15729 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/mpck.py
+-rwxr-xr-x   0        0        0     1812 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/mpko.py
+-rwxr-xr-x   0        0        0     8992 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/sentiment/utils.py
+-rw-r--r--   0        0        0      104 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/tag/__init__.py
+-rw-r--r--   0        0        0    12575 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/tag/_mecab.py
+-rw-r--r--   0        0        0     2171 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/tag/_postprocess.py
+-rwxr-xr-x   0        0        0        0 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/utils/__init__.py
+-rw-r--r--   0        0        0     3481 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/utils/dictionary.py
+-rw-r--r--   0        0        0     6426 2023-07-24 04:02:40.432117 ekonlpy-1.2.0/src/ekonlpy/utils/io.py
+-rw-r--r--   0        0        0     9695 1970-01-01 00:00:00.000000 ekonlpy-1.2.0/PKG-INFO
```

### Comparing `ekonlpy-1.1.7/LICENSE` & `ekonlpy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/README.md` & `ekonlpy-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,27 @@
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/eKoNLPy
 [release-url]: https://github.com/entelecheia/eKoNLPy/releases
 [pypi-downloads-image]: https://img.shields.io/pypi/dm/ekonlpy
 [codecov-image]: https://codecov.io/gh/entelecheia/eKoNLPy/branch/master/graph/badge.svg?token=8I4ORHRREL
 [codecov-url]: https://codecov.io/gh/entelecheia/eKoNLPy
 [zenodo-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.7809447.svg
 [zenodo-url]: https://doi.org/10.5281/zenodo.7809447
-
 [repo-url]: https://github.com/entelecheia/eKoNLPy
 [pypi-url]: https://pypi.org/project/ekonlpy
 [docs-url]: https://ekonlpy.entelecheia.ai
 [changelog]: https://github.com/entelecheia/eKoNLPy/blob/master/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/eKoNLPy/blob/master/CONTRIBUTING.md
 
 <!-- Links: -->
 
 `eKoNLPy` is a Korean Natural Language Processing (NLP) Python library specifically designed for economic analysis. It extends the functionality of the `MeCab` tagger from KoNLPy to improve the handling of economic terms, financial institutions, and company names, classifying them as single nouns. Additionally, it incorporates sentiment analysis features to determine the tone of monetary policy statements, such as Hawkish or Dovish.
 
-**Important Note:**
-
-eKoNLPy is built on the [fugashi](https://github.com/polm/fugashi) and [mecab-ko-dic](https://github.com/LuminosoInsight/mecab-ko-dic) libraries. For more information on using the `Mecab` tagger, please refer to the [fugashi documentation](https://github.com/polm/fugashi). As eKoNLPy no longer relies on the [KoNLPy](https://konlpy.org) library, Java is not required for its use. This makes eKoNLPy compatible with Windows, Linux, and Mac OS, without the need for Java installation. You can also use eKoNLPy on Google Colab.
+> **Note**
+>
+> eKoNLPy is built on the [fugashi](https://github.com/polm/fugashi) and [mecab-ko-dic](https://github.com/LuminosoInsight/mecab-ko-dic) libraries. For more information on using the `Mecab` tagger, please refer to the [fugashi documentation](https://github.com/polm/fugashi). As eKoNLPy no longer relies on the [KoNLPy](https://konlpy.org) library, Java is not required for its use. This makes eKoNLPy compatible with Windows, Linux, and Mac OS, without the need for Java installation. You can also use eKoNLPy on Google Colab.
 
 If you wish to tokenize general Korean text with eKoNLPy, you do not need to install the `KoNLPy` library. Instead, utilize `ekonlpy.mecab.MeCab` as a replacement for `ekonlpy.tag.Mecab`.
 
 However, if you plan to use the [Korean Sentiment Analyzer (KSA)](#korean-sentiment-analyzer-ksa), which employs the `Kkma` morpheme analyzer, you will need to install the [KoNLPy](https://konlpy.org) library.
 
 ## Installation
 
@@ -52,28 +51,36 @@
 ## Usage
 
 ### Part of Speech Tagging
 
 To use the part of speech tagging feature, input `Mecab.pos(phrase)` just like KoNLPy. First, the input is processed using KoNLPy's Mecab morpheme analyzer. Then, if a combination of consecutive tokens matches a term in the user dictionary, the phrase is separated into compound nouns.
 
 ```python
-from ekonlpy.tag import Mecab
+from ekonlpy import Mecab
 
 mecab = Mecab()
 mecab.pos('금통위는 따라서 물가안정과 병행, 경기상황에 유의하는 금리정책을 펼쳐나가기로 했다고 밝혔다.')
 ```
 
 > [('금', 'MAJ'), ('통', 'MAG'), ('위', 'NNG'), ('는', 'JX'), ('따라서', 'MAJ'), ('물가', 'NNG'), ('안정', 'NNG'), ('과', 'JC'), ('병행', 'NNG'), (',', 'SC'), ('경기', 'NNG'), ('상황', 'NNG'), ('에', 'JKB'), ('유의', 'NNG'), ('하', 'XSV'), ('는', 'ETM'), ('금리', 'NNG'), ('정책', 'NNG'), ('을', 'JKO'), ('펼쳐', 'VV+EC'), ('나가', 'VX'), ('기', 'ETN'), ('로', 'JKB'), ('했', 'VV+EP'), ('다고', 'EC'), ('밝혔', 'VV+EP'), ('다', 'EF'), ('.', 'SF')]
 
+You can also use the Command Line Interface (CLI) to perform part of speech tagging:
+
+```bash
+ekonlpy --input "안녕하세요"
+```
+
+> [('안녕', 'NNG'), ('하', 'XSV'), ('세요', 'EP')]
+
 ### cf. MeCab POS Tagging (fugashi)
 
 ```python
-from ekonlpy.mecab import MeCab # Be careful! `C` is capital.
+from ekonlpy import Mecab
 
-mecab = MeCab()
+mecab = Mecab(use_original_tagger=True) # set use_original_tagger=True
 mecab.pos('금통위는 따라서 물가안정과 병행, 경기상황에 유의하는 금리정책을 펼쳐나가기로 했다고 밝혔다.')
 ```
 
 > [('금', 'MAJ'), ('통', 'MAG'), ('위', 'NNG'), ('는', 'JX'), ('따라서', 'MAJ'), ('물가', 'NNG'), ('안정', 'NNG'), ('과', 'JC'), ('병행', 'NNG'), (',', 'SC'), ('경기', 'NNG'), ('상황', 'NNG'), ('에', 'JKB'), ('유의', 'NNG'), ('하', 'XSV'), ('는', 'ETM'), ('금리', 'NNG'), ('정책', 'NNG'), ('을', 'JKO'), ('펼쳐', 'VV+EC'), ('나가', 'VX'), ('기', 'ETN'), ('로', 'JKB'), ('했', 'VV+EP'), ('다고', 'EC'), ('밝혔', 'VV+EP'), ('다', 'EF'), ('.', 'SF')]
 
 ### Lemmatization and Synonyms
```

### Comparing `ekonlpy-1.1.7/pyproject.toml` & `ekonlpy-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eKoNLPy"
-version = "1.1.7"
+version = "1.2.0"
 description = "A Korean natural language processing toolkit for economic analysis"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "ekonlpy", from = "src" }]
 homepage = "https://ekonlpy.entelecheia.ai/"
 repository = "https://github.com/entelecheia/eKoNLPy"
@@ -13,32 +13,38 @@
     "src/ekonlpy/data/*/*.txt",
     "src/ekonlpy/data/*/*.csv",
     "src/ekonlpy/data/*/*/*.txt",
     "src/ekonlpy/data/*/*/*.csv",
     "src/ekonlpy/data/model/*",
 ]
 
+[tool.poetry.scripts]
+ekonlpy = "ekonlpy.__cli__:main"
+
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
 fugashi = "^1.2.1"
 mecab-ko-dic = "^1.0.0"
 nltk = "^3.8.1"
 scipy = "^1.10.1"
 pandas = "^1.5.3"
+click = "^8.1.6"
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
-black = "^23.1.0"
+black = ">=23.0.0,<=23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-commitizen = "^2.42.1"
 
 [tool.black]
 exclude = [
     '_version.py',
     'node_modules',
     '_build',
     'docs',
@@ -128,21 +134,21 @@
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "master"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/ekonlpy/_version.py:__version__"
 version_source = "tag"
-commit_version_number = true                                          # required for version_source = "tag"
+commit_version_number = true                                    # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
-hvcs = "github"                                                       # hosting version control system, gitlab is also supported
+hvcs = "github"                                                 # hosting version control system, gitlab is also supported
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ADJECTIVES.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ADJECTIVES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/COUNTRY.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/COUNTRY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_PHRASES.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ECON_TERMS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ECON_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/ENTITY.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/ENTITY.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/FOREIGN_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/GENERIC.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/GENERIC.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INDUSTRY_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/INSTITUTION.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/INSTITUTION.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/LEMMA.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/LEMMA.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NAMES.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NAMES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/NOUNS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/POLARITY_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/PROPER_NOUNS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SECTOR.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SECTOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_EN.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/STOPWORDS_KOR.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_PHRASES.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/dictionary/SYNONYM_TERMS.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Currencies.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Currencies.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/DatesandNumbers.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/DatesandNumbers.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Generic.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Generic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Geographic.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Geographic.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/HIV-4.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/HIV-4.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/LM.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/LM.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/Names.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/Names.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/euko/mp_uncertainty_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/expressive-type.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/expressive-type.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/intensity.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/intensity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/kosac/polarity.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/kosac/polarity.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_lex.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n3.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_lexicon_mkt_n7.csv`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_vocab.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt` & `ekonlpy-1.2.0/src/ekonlpy/data/lexicon/mpko/mp_polarity_wordset.txt`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/model/MPKC.nbc` & `ekonlpy-1.2.0/src/ekonlpy/data/model/MPKC.nbc`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/data/tagset.py` & `ekonlpy-1.2.0/src/ekonlpy/data/tagset.py`

 * *Files identical despite different names*

### Comparing `ekonlpy-1.1.7/src/ekonlpy/etag/_template.py` & `ekonlpy-1.2.0/src/ekonlpy/etag/_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ..data.tagset import nouns_tags, pass_tags, skip_chk_tags, skip_tags
+from ekonlpy.data.tagset import nouns_tags, pass_tags, skip_chk_tags, skip_tags
 
 
 class ExtTagger:
     def __init__(self, dictionary, max_ngram=7):
         self.dictionary = dictionary
         self.max_ngram = max_ngram
         self.skip_chk_tags = skip_chk_tags
@@ -61,18 +61,17 @@
 
                     if not word_found and tmp_tags in cskip_chk_tags.keys():
                         new_word = ""
                         num_word = ""
                         for j in range(ngram):
                             if tmp_tags[j] not in cskip_tags:
                                 new_word += tokens_org[ipos + j][0]
-                            if tmp_tags[j] == "SN":
-                                num_word += "n"
-                            else:
-                                num_word += tokens_org[ipos + j][0]
+                            num_word += (
+                                "n" if tmp_tags[j] == "SN" else tokens_org[ipos + j][0]
+                            )
                         dict_tag = cdictionary.get_tags(num_word.lower())
                         if dict_tag:
                             new_word = num_word
                         else:
                             dict_tag = cdictionary.get_tags(new_word.lower())
                         if dict_tag:
                             new_tag = (
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/mecab/_mecab.py` & `ekonlpy-1.2.0/src/ekonlpy/mecab/_mecab.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 import logging
 import os
 from collections import namedtuple
+from typing import Any, List, Optional, Sequence, Tuple, Union
 
-log = logging.getLogger(__name__)
+import fugashi as _mecab
+
+from ekonlpy.base import BaseMecab
+
+logger = logging.getLogger(__name__)
 
 
 Feature = namedtuple(
     "Feature",
     [
         "pos",
         "semantic",
@@ -20,160 +25,169 @@
 )
 # ('합니다',
 #   Feature(pos='XSA+EF', semantic=None, has_jongseong=False, reading='합니다', type='Inflect',
 #           start_pos='XSA', end_pos='EF',
 #           expression='하/XSA/*+ᄇ니다/EF/*')),
 
 
-def _extract_feature(values):
+def _extract_feature(values: Sequence[Any]) -> Feature:
     # Reference:
     # - http://taku910.github.io/mecab/learn.html
     # - https://docs.google.com/spreadsheets/d/1-9blXKjtjeKZqsf4NzHeYJCrr49-nXeRF6D80udfcwY
     # - https://bitbucket.org/eunjeon/mecab-ko-dic/src/master/utils/dictionary/lexicon.py
 
     # feature = <pos>,<semantic>,<has_jongseong>,<reading>,<type>,<start_pos>,<end_pos>,<expression>
     assert len(values) == 8
 
-    values = [value if value != "*" else None for value in values]
-    feature = dict(zip(Feature._fields, values))
-    feature["has_jongseong"] = {"T": True, "F": False}.get(feature["has_jongseong"])
+    feature_values = [value if value != "*" else None for value in values]
+    feature = dict(zip(Feature._fields, feature_values))
+    has_jongseong = feature.get("has_jongseong")
+    feature["has_jongseong"] = has_jongseong == "T"
 
     return Feature(**feature)
 
 
 class MeCabError(Exception):
     pass
 
 
-class MeCab:  # APIs are inspried by KoNLPy
+class Mecab(BaseMecab):
+    backend = "fugashi"
+    verbose: bool = False
+
+    _tagger: _mecab.GenericTagger  # type: ignore
+
     def __init__(
         self,
-        dicdir=None,
-        userdic_path=None,
-        verbose=False,
+        dicdir: Optional[str] = None,
+        userdic_path: Optional[str] = None,
+        verbose: bool = False,
         **kwargs,
     ):
         import mecab_ko_dic
 
-        self.dicdir = None
-        self.userdic_path = None
         self.verbose = verbose
 
         DICDIR = mecab_ko_dic.DICDIR
         mecabrc = os.path.join(DICDIR, "mecabrc")
 
-        if self.verbose:
-            log.info(f"MeCab uses {self.backend} as backend.")
+        logger.debug("MeCab uses %s backend.", self.backend)
 
         if not dicdir:
             dicdir = DICDIR
-        self.dicdir = dicdir
-        MECAB_ARGS = '-r "{}" -d "{}" '.format(mecabrc, dicdir)
+        MECAB_ARGS = f'-r "{mecabrc}" -d "{dicdir}" '
         if userdic_path:
-            self.userdic_path = userdic_path
-            MECAB_ARGS += '-u "{}" '.format(userdic_path)
+            MECAB_ARGS += f'-u "{userdic_path}" '
         if self.verbose:
-            log.info(
-                f"Mecab uses system dictionary: {dicdir}, user dictionary: {userdic_path}"
+            logger.info(
+                "Mecab uses system dictionary: %s, user dictionary: %s",
+                dicdir,
+                userdic_path,
             )
         try:
-            try:
-                import fugashi as _mecab
-            except ImportError:
-                raise ImportError(
-                    "\n"
-                    "You must install `fugashi` to use MeCab backend.\n"
-                    "Please install it with `pip install fugashi`.\n"
-                )
-            self.tagger = _mecab.GenericTagger(MECAB_ARGS)
-            self.dictionary_info = self.tagger.dictionary_info
-            self.sysdic_path = self.dictionary_info[0]["filename"]
-        except RuntimeError:
-            raise Exception(
+            self._tagger = _mecab.GenericTagger(MECAB_ARGS)  # type: ignore
+            dictionary_info = self._tagger.dictionary_info
+            sysdic_path = dictionary_info[0]["filename"]
+            logger.debug("Mecab is loaded from %s", sysdic_path)
+        except RuntimeError as e:
+            raise MeCabError(
                 'The MeCab dictionary does not exist at "%s". Is the dictionary correctly installed?\nYou can also try entering the dictionary path when initializing the MeCab class: "MeCab(\'/some/dic/path\')"'
-                % self.dicdir
-            )
-        except NameError:
-            raise Exception("Check if MeCab is installed correctlly.")
+                % dicdir
+            ) from e
+        except NameError as e:
+            raise MeCabError(
+                "The fugashi package is not installed. Please install fugashi with: pip install fugashi"
+            ) from e
 
-    def parse(self, text):
+    def _parse(self, text: str) -> List[Tuple[str, Feature]]:
         return [
-            (node.surface, _extract_feature(node.feature)) for node in self.tagger(text)
+            (node.surface, _extract_feature(node.feature))
+            for node in self._tagger(text)
         ]
 
-    def pos(
+    def parse(
         self,
-        sentence,
-        flatten=True,
-        concat_surface_and_pos=False,
-        include_whitespace_token=False,
-    ):
-        sentence = sentence.strip()
+        text: str,
+        flatten: bool = True,
+        include_whitespace_token: bool = False,
+    ) -> List[Tuple[str, str]]:
+        if flatten:
+            res = [(surface, feature.pos) for surface, feature in self._parse(text)]
+        else:
+            res = []
+            for surface, feature in self._parse(text):
+                if feature.expression is None:
+                    res.append((surface, feature.pos))
+                else:
+                    for elem in feature.expression.split("+"):
+                        s = elem.split("/")
+                        res.append((s[0], s[1]))
         if include_whitespace_token:
             sent_ptr = 0
             res = []
 
-            for token, pos in self._pos(sentence, flatten=flatten):
-                if sentence[sent_ptr] == " ":
+            for token, pos in res:
+                if text[sent_ptr] == " ":
                     # Move pointer to whitespace token to reserve whitespace
                     # cf. to prevent double white-space, move pointer to next eojeol
-                    while sentence[sent_ptr] == " ":
+                    while text[sent_ptr] == " ":
                         sent_ptr += 1
                     res.append((" ", "SP"))
                 res.append((token, pos))
                 sent_ptr += len(token)
-        else:
-            res = self._pos(sentence, flatten=flatten)
+        return res
 
-        return [s[0] + "/" + s[1] if concat_surface_and_pos else s for s in res]
+    def pos(
+        self,
+        text: str,
+        flatten: bool = True,
+        include_whitespace_token: bool = False,
+    ) -> List[Tuple[str, str]]:
+        return self.parse(
+            text, flatten=flatten, include_whitespace_token=include_whitespace_token
+        )
 
-    def _pos(self, sentence, flatten=True):
-        if flatten:
-            return [(surface, feature.pos) for surface, feature in self.parse(sentence)]
-        else:
-            res = []
-            for surface, feature in self.parse(sentence):
-                if feature.expression is None:
-                    res.append((surface, feature.pos))
-                else:
-                    for elem in feature.expression.split("+"):
-                        s = elem.split("/")
-                        res.append((s[0], s[1]))
-            return res
+    def tokenize(
+        self,
+        text: str,
+        flatten: bool = True,
+        include_whitespace_token: bool = False,
+        strip_pos: bool = False,
+        postag_delim: str = "/",
+    ) -> List[str]:
+        tokens = self.parse(
+            text, flatten=flatten, include_whitespace_token=include_whitespace_token
+        )
 
-    def morphs(self, sentence, flatten=True, include_whitespace_token=True):
         return [
-            surface
-            for surface, _ in self.pos(
-                sentence,
-                flatten=flatten,
-                concat_surface_and_pos=False,
-                include_whitespace_token=include_whitespace_token,
-            )
+            token_pos[0] if strip_pos else f"{token_pos[0]}{postag_delim}{token_pos[1]}"
+            for token_pos in tokens
         ]
 
+    def morphs(self, text: str, flatten: bool = True) -> List[str]:
+        return self.tokenize(
+            text, flatten=flatten, strip_pos=True, include_whitespace_token=False
+        )
+
     def nouns(
         self,
-        sentence,
-        flatten=True,
-        include_whitespace_token=True,
-        noun_pos=["NNG", "NNP", "XSN", "SL", "XR", "NNB", "NR"],
-    ):
-        return [
-            surface
-            for surface, pos in self.pos(
-                sentence,
-                flatten=flatten,
-                concat_surface_and_pos=False,
-                include_whitespace_token=include_whitespace_token,
-            )
-            if pos in noun_pos
-        ]
+        text: Union[str, List[Tuple[str, str]]],
+        flatten: bool = True,
+        noun_pos: Optional[List[str]] = None,
+    ) -> List[str]:
+        if not noun_pos:
+            noun_pos = ["NNG", "NNP", "XSN", "SL", "XR", "NNB", "NR"]
+        tagged = (
+            self.pos(text, flatten=flatten, include_whitespace_token=False)
+            if isinstance(text, str)
+            else text
+        )
+        return [surface for surface, pos in tagged if pos in noun_pos]
 
 
 if __name__ == "__main__":
-    tagger = MeCab()
+    tagger = Mecab()
     text = "아버지가 방에 들어가신다."
-    print(tagger.parse(text))
+    print(tagger._parse(text))
     print(tagger.pos(text))
     print(tagger.morphs(text))
     print(tagger.nouns(text))
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/mecab/_userdic.py` & `ekonlpy-1.2.0/src/ekonlpy/mecab/_userdic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import logging
 import os
 import subprocess
 from collections import namedtuple
 from pathlib import Path
+from typing import Any, Dict, List, Optional, Sequence, Tuple
 
+import mecab_ko_dic
 import pandas as pd
 
+logger = logging.getLogger(__name__)
+
 DicEntry = namedtuple(
     "DicEntry",
     [
         "surface",
         "left_id",
         "right_id",
         "cost",
@@ -48,65 +53,73 @@
 
 
 def has_jongseong(c):
     return int((ord(c[-1]) - 0xAC00) % 28) != 0
 
 
 class MecabDicConfig:
-    def __init__(self, userdic_path=None):
-        import mecab_ko_dic
+    userdic: Dict[str, DicEntry] = {}
+    dicdir: str = mecab_ko_dic.DICDIR
+    left_ids: List[ContextEntry] = []
+    right_ids: List[ContextEntry] = []
 
+    def __init__(self, userdic_path: Optional[str] = None):
         if userdic_path:
             self.load_userdic(userdic_path)
         else:
             self.userdic = {}
         self.dicdir = mecab_ko_dic.DICDIR
         self.left_ids = self.load_context_ids("left-id.def")
         self.right_ids = self.load_context_ids("right-id.def")
 
-    def load_context_ids(self, id_file):
+    def load_context_ids(self, id_file: str) -> List[ContextEntry]:
         id_file = os.path.join(self.dicdir, id_file)
         context_ids = []
         with open(id_file, "r", encoding="utf-8") as f:
             for line in f:
                 id, vals = line.split()
                 entry = ContextEntry(id, *vals.split(","))
                 context_ids.append(entry)
         return context_ids
 
-    def find_left_context_id(self, search):
+    def find_left_context_id(self, search: DicEntry) -> Optional[str]:
         for entry in self.left_ids:
             if entry.pos == search.pos and entry.semantic == search.semantic:
                 return entry.id
 
-    def find_right_context_id(self, search):
+    def find_right_context_id(self, search: DicEntry) -> Optional[str]:
         for entry in self.right_ids:
             if (
                 entry.pos == search.pos
                 and entry.semantic == search.semantic
                 and entry.has_jongseong == search.has_jongseong
             ):
                 return entry.id
 
-    def load_userdic(self, userdic_path):
-        userdic_path = Path(userdic_path)
+    def load_userdic(self, userdic_path: str):
+        userdic_path_ = Path(userdic_path)
 
-        if userdic_path.is_dir():
+        if userdic_path_.is_dir():
             self.userdic = {}
-            for f in userdic_path.glob("*.csv"):
+            for f in userdic_path_.glob("*.csv"):
                 df = pd.read_csv(f, names=DicEntry._fields)
-                dic = {e.surface: e for e in iternamedtuples(df)}
+                dic = {e.surface: DicEntry(*e) for e in iternamedtuples(df)}
                 self.userdic = {**self.userdic, **dic}
         else:
-            df = pd.read_csv(userdic_path, names=DicEntry._fields)
-            self.userdic = {e.surface: e for e in iternamedtuples(df)}
-        print(" No. of user dictionary entires loaded: %d" % len(self.userdic))
+            df = pd.read_csv(userdic_path_, names=DicEntry._fields)
+            self.userdic = {e.surface: DicEntry(*e) for e in iternamedtuples(df)}
+        logger.info("No. of user dictionary entires loaded: %d", len(self.userdic))
 
     def add_entry_to_userdic(
-        self, surface, pos="NNP", semantic="*", reading=None, cost=1000
+        self,
+        surface: str,
+        pos: str = "NNP",
+        semantic: str = "*",
+        reading: Optional[str] = None,
+        cost: int = 1000,
     ):
         entry = DicEntry(
             surface=surface,
             cost=cost,
             pos=pos,
             semantic=semantic,
             has_jongseong={True: "T", False: "F"}.get(has_jongseong(surface)),
@@ -122,28 +135,29 @@
         for entry in self.userdic.values():
             entry = entry._replace(
                 left_id=self.find_left_context_id(entry),
                 right_id=self.find_right_context_id(entry),
             )
             self.userdic[entry.surface] = entry
 
-    def adjust_costs(self, cost=1000):
+    def adjust_costs(self, cost: int = 1000):
         for surface, entry in self.userdic.items():
             self.userdic[surface] = entry._replace(cost=cost)
 
-    def save_userdic(self, save_path):
+    def save_userdic(self, save_path: str):
         if len(self.userdic) > 0:
             df = pd.DataFrame(self.userdic.values())
             df.to_csv(save_path, header=False, index=False)
             self.userdic_path = save_path
-            print("Saved the userdic to {}".format(save_path))
+            logger.info("No. of user dictionary entires saved: %d", len(self.userdic))
+            logger.info("User dictionary saved to %s", save_path)
         else:
-            print("No userdic to save...")
+            logger.warning("No user dictionary entries to save.")
 
-    def build_userdic(self, built_userdic_path, userdic_path=None):
+    def build_userdic(
+        self, built_userdic_path: str, userdic_path: Optional[str] = None
+    ):
         if userdic_path:
             self.userdic_path = userdic_path
-        args = '-d "{}" -u "{}" {}'.format(
-            self.dicdir, built_userdic_path, self.userdic_path
-        )
+        args = f'-d "{self.dicdir}" -u "{built_userdic_path}" {self.userdic_path}'
         # print(args)
         subprocess.run(["fugashi-build-dict", args])
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/base.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 This module contains base classes for dictionaries.
 """
 
+
 import abc
 
 from ..utils.io import installpath
 
-LEXICON_PATH = "%s/data/lexicon" % installpath
+LEXICON_PATH = f"{installpath}/data/lexicon"
 
 
 class BaseDict(object):
     """
     A base class for sentiment analysis.
     For now, only 'positive' and 'negative' analysis is supported.
 
@@ -62,15 +63,15 @@
         self._intensity_cutoff = intensity_cutoff
         self.init_dict(kind, intensity_cutoff)
         if tokenizer is None:
             self.init_tokenizer(kind)
         else:
             self._tokenizer = tokenizer
 
-        assert len(self._posdict) > 0 and len(self._negdict) > 0
+        assert self._posdict and self._negdict
 
     def tokenize(self, text):
         """
         :type text: str
         :returns: list
         """
         return self._tokenizer.tokenize(text)
@@ -94,37 +95,33 @@
         """Get score for a single term.
         - +1 for positive terms.
         - -1 for negative terms.
         - 0 for others.
 
         :returns: int
         """
-        if by_count:
-            if term in self._posdict.keys():
-                return self._posdict[term]
-            elif term in self._negdict.keys():
-                return self._negdict[term]
-            else:
-                return 0
+        if not by_count:
+            return self._poldict[term] if term in self._poldict.keys() else 0
+        if term in self._posdict.keys():
+            return self._posdict[term]
+        elif term in self._negdict.keys():
+            return self._negdict[term]
         else:
-            if term in self._poldict.keys():
-                return self._poldict[term]
-            else:
-                return 0
+            return 0
 
     def get_score(self, terms, by_count=True):
         """Get score for a list of terms.
 
         :type terms: list
         :param terms: A list of terms to be analyzed.
         :param by_count; if True, use number of occruences of sentiment tokens
 
         :returns: dict
         """
-        assert isinstance(terms, list) or isinstance(terms, tuple)
+        assert isinstance(terms, (list, tuple))
         score_li = [self._get_score(t, by_count) for t in terms]
         pos_score_li = [s for s in score_li if s > 0]
         neg_score_li = [s for s in score_li if s < 0]
 
         s_pos = sum(pos_score_li)
         s_neg = sum(neg_score_li)
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/euko.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/euko.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,18 @@
     def init_tokenizer(self, kind=None):
         self._tokenizer = MPTokenizer(kind, self._poldict, keep_overlapping_ngram=True)
 
     def init_dict(self, kind=None, intensity_cutoff=None):
         kind = kind if kind in self.KINDS.keys() else 0
         if intensity_cutoff is not None:
             self._intensity_cutoff = intensity_cutoff
+        elif kind in self.INTENSITY_KINDS.keys():
+            self._intensity_cutoff = self.INTENSITY_KINDS[kind]
         else:
-            if kind in self.INTENSITY_KINDS.keys():
-                self._intensity_cutoff = self.INTENSITY_KINDS[kind]
-            else:
-                self._intensity_cutoff = 1.1
+            self._intensity_cutoff = 1.1
         self._intensity_cutoff = min(3, self._intensity_cutoff)
         # print('Initialize the dictionary using a lexicon file: {}'.format(self.KINDS[kind]))
         path = os.path.join(LEXICON_PATH, "euko", self.KINDS[kind])
         with open(path, encoding="utf-8") as f:
             for line in f:
                 word = line.split(",")
                 w = word[0]
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/hiv4.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/hiv4.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,14 @@
     def init_tokenizer(self, kind=None, intensity_cutoff=None):
         self._tokenizer = Tokenizer()
 
     def init_dict(self, kind=None):
         data = pd.read_csv(self.PATH, low_memory=False)
         for category in ["Positiv", "Negativ"]:
             terms = data["Entry"][data[category] == category]
-            if category == "Positiv":
-                for t in terms:
-                    t = self.tokenize(t)
-                    if len(t) > 0:
+            for t in terms:
+                t = self.tokenize(t)
+                if len(t) > 0:
+                    if category == "Positiv":
                         self._posdict[t[0]] = 1
-            else:
-                for t in terms:
-                    t = self.tokenize(t)
-                    if len(t) > 0:
+                    else:
                         self._negdict[t[0]] = -1
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/kosac.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/kosac.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,18 @@
         path = os.path.join(LEXICON_PATH, "kosac", "polarity.csv")
         with open(path, encoding="utf-8") as f:
             for line in f:
                 word = line.split(",")
                 w = word[0]
                 if w == "ngram":
                     continue
-                p = float(word[6].strip())
-                n = float(word[3].strip())
-                s = p - n
                 if len(w) > 1:
+                    n = float(word[3].strip())
+                    p = float(word[6].strip())
+                    s = p - n
                     if s > 0:
                         self._posdict[w] = 1
                         self._poldict[w] = s
                     elif s < 0:
                         self._negdict[w] = -1
                         self._poldict[w] = s
 
@@ -74,42 +74,36 @@
         vocab = {}
         if os.path.isfile(file_path):
             with open(file_path) as f:
                 for lno, line in enumerate(f):
                     # skip header
                     if lno == 0:
                         headers = line.strip().split(delimiter)
-                    else:
-                        if len(line) > 0:
-                            row = line.strip().split(delimiter)
-                            ngram = row[0]
-                            # ngram_split = tuple(ngram.split(';'))
-                            data = {}
-                            for i, header in enumerate(headers):
-                                if i > 0:
-                                    data[header] = row[i]
-                            vocab[ngram] = data
+                    elif len(line) > 0:
+                        row = line.strip().split(delimiter)
+                        data = {header: row[i] for i, header in enumerate(headers) if i > 0}
+                        vocab[row[0]] = data
         return vocab
 
     def morpheme(self, dataset):
         return self.align_morpheme(self._tagger.pos(dataset))
 
     def align_morpheme(self, morpheme):
-        return ["{}/{}".format(w, t) for w, t in morpheme]
+        return [f"{w}/{t}" for w, t in morpheme]
 
     def percentage(self, obj):
         return {k: v / sum(obj.values()) for k, v in obj.items()}
 
     def calc(self, keypairs, source, target, func):
         for keypair in keypairs:
             sourcekey = keypair[0]
-            targetkey = keypair[1]
             if sourcekey in source:
                 sourcedata = source[sourcekey]
                 sourcedata = float(sourcedata)
+                targetkey = keypair[1]
                 target[targetkey] = func(sourcedata, target[targetkey])
         return target
 
     def match(self, data, pairdata, keypairs):
         ret = {k[1]: 0 for k in keypairs}
         for m in data:
             if m in pairdata:
@@ -171,16 +165,15 @@
         return self.ngramize(tokens)
 
     def ngramize(self, tokens):
         ngram_tokens = []
         tokens = [w for w in tokens if w.split("/")[1] not in self._skiptags]
         for pos in range(len(tokens)):
             for gram in range(1, self._ngram + 1):
-                token = self.get_ngram(tokens, pos, gram)
-                if token:
+                if token := self.get_ngram(tokens, pos, gram):
                     ngram_tokens.append(token)
         return ngram_tokens
 
     def get_ngram(self, tokens, pos, gram):
         if pos < 0:
             return None
         if pos + gram > len(tokens):
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/lm.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/lm.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     def init_tokenizer(self, kind=None, intensity_cutoff=None):
         self._tokenizer = Tokenizer()
 
     def init_dict(self, kind=None):
         data = pd.read_csv(self.PATH, low_memory=False)
         for category in ["Positive", "Negative"]:
             terms = data["Word"][data[category] > 0]
-            if category == "Positive":
-                for t in terms:
-                    t = self.tokenize(t)
-                    if len(t) > 0:
+            for t in terms:
+                t = self.tokenize(t)
+                if len(t) > 0:
+                    if category == "Positive":
                         self._posdict[t[0]] = 1
-            else:
-                for t in terms:
-                    t = self.tokenize(t)
-                    if len(t) > 0:
+                    else:
                         self._negdict[t[0]] = -1
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/mpck.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/mpck.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module contains classes for monetary policy sentiment classifier.
 """
 
+
 import os
 import pickle
 from collections import defaultdict, namedtuple
 
 import nltk
 import numpy as np
 from nltk.classify import NaiveBayesClassifier
@@ -16,15 +17,15 @@
 from scipy.stats import pearsonr, spearmanr
 
 from ..data.tagset import aux_tags
 from ..tag import Mecab
 from ..utils.io import installpath
 from .base import LEXICON_PATH
 
-MODEL_PATH = "%s/data/model" % installpath
+MODEL_PATH = f"{installpath}/data/model"
 
 
 class MPCK(object):
     """
     A class for monetary policy sentiment classifier.
     """
 
@@ -47,15 +48,15 @@
         self._aux_tags = aux_tags
         self._auxwords = {"못하/VX", "아니/VCN", "않/VX", "지만/VCP"}
 
     def get_vocab(self, file):
         vocab = {}
         vocab_path = os.path.join(LEXICON_PATH, file)
         with open(vocab_path) as f:
-            for i, line in enumerate(f):
+            for line in f:
                 w = line.strip().split()
                 if len(w[0]) > 0:
                     vocab[w[0]] = w[1]
         return vocab
 
     def load_default_classifier(self):
         classifier_path = os.path.join(MODEL_PATH, "MPKC.nbc")
@@ -67,15 +68,15 @@
                 self.classifier = pickle.load(f)
         else:
             raise ValueError("There is no classifier file.")
 
     def save_classifier(self, file_path):
         with open(file_path, "wb") as f:
             pickle.dump(self.classifier, f)
-        print("Save the classifier to the file: {}".format(file_path))
+        print(f"Save the classifier to the file: {file_path}")
 
     def tokenize(self, text):
         tokens = self._tokenizer.sent_words(text)
         tokens = [
             w
             for w in tokens
             if (
@@ -86,30 +87,25 @@
         return tokens
 
     def ngramize(self, tokens, keep_overlapping_ngram=False):
         ngram_tokens = []
 
         for pos in range(len(tokens)):
             for gram in range(self._min_ngram, self._ngram + 1):
-                token = self.get_ngram(tokens, pos, gram)
-                if token:
+                if token := self.get_ngram(tokens, pos, gram):
                     if token in self._vocab:
                         ngram_tokens.append(token)
         if not keep_overlapping_ngram:
             filtered_tokens = []
-            if len(ngram_tokens) > 0:
+            if ngram_tokens:
                 ngram_tokens = sorted(
                     ngram_tokens, key=lambda item: len(item), reverse=True
                 )
                 for token in ngram_tokens:
-                    existing_token = False
-                    for check_token in filtered_tokens:
-                        if token in check_token:
-                            existing_token = True
-                            break
+                    existing_token = any(token in check_token for check_token in filtered_tokens)
                     if not existing_token:
                         filtered_tokens.append(token)
             ngram_tokens = filtered_tokens
 
         return ngram_tokens
 
     def get_ngram(self, tokens, pos, gram):
@@ -117,33 +113,29 @@
             return None
         if pos + gram > len(tokens):
             return None
         token = tokens[pos]
         check_noun = False
 
         tag = token.split("/")[1] if "/" in token else None
-        if tag in self._start_tags:
-            if tag in self._noun_tags:
-                check_noun = True
-            for i in range(1, gram):
-                if tokens[pos + i] != tokens[pos + i - 1]:
-                    tag = (
-                        tokens[pos + i].split("/")[1]
-                        if "/" in tokens[pos + i]
-                        else None
-                    )
-                    if tag in self._noun_tags:
-                        check_noun = True
-                    token += self._delimiter + tokens[pos + i]
-            if check_noun:
-                return token
-            else:
-                return None
-        else:
+        if tag not in self._start_tags:
             return None
+        if tag in self._noun_tags:
+            check_noun = True
+        for i in range(1, gram):
+            if tokens[pos + i] != tokens[pos + i - 1]:
+                tag = (
+                    tokens[pos + i].split("/")[1]
+                    if "/" in tokens[pos + i]
+                    else None
+                )
+                if tag in self._noun_tags:
+                    check_noun = True
+                token += self._delimiter + tokens[pos + i]
+        return token if check_noun else None
 
     def classify(self, tokens, intensity_cutoff=1.3):
         eps = 1e-6
         features = {token: True for token in tokens}
         result = self.classifier.prob_classify(features)
         pos_score = result.prob(self._positive_label)
         neg_score = result.prob(self._negative_label)
@@ -161,15 +153,15 @@
             "Neg score": neg_score,
         }
 
     def get_informative_features(self, cutoff_ratio=1.2):
         cpdist = (
             self.classifier._feature_probdist
         )  # probability distribution for feature values given labels
-        fcnt = len(set([w for _, w in cpdist.keys()]))
+        fcnt = len({w for _, w in cpdist.keys()})
         feature_list = []
         epsilon = 1e-6
         feature = namedtuple("Feature", ["Word", "Label", "Polarity", "Intensity"])
 
         for feature_name, feature_val in self.classifier.most_informative_features(
             n=fcnt
         ):
@@ -224,23 +216,21 @@
     ):
         """
         Bootstrap aggregating classifiers
         """
 
         if verbose:
             print(
-                "\nNo. of iterations: {}. feature function: {}, train ratio: {}, best words ratio: {}".format(
-                    iterations, feature_fn_name, train_ratio, best_words_ratio
-                )
+                f"\nNo. of iterations: {iterations}. feature function: {feature_fn_name}, train ratio: {train_ratio}, best words ratio: {best_words_ratio}"
             )
 
         clfs = []
         mlst = []
 
-        for i in range(iterations):
+        for _ in range(iterations):
             classifier, metrics = self.train_classifier(
                 dataset,
                 feature_fn_name=feature_fn_name,
                 verbose=False,
                 train_ratio=train_ratio,
                 best_ratio=best_words_ratio,
                 token_column=token_column,
@@ -258,20 +248,20 @@
             if metrics["Accuracy"] > best_accuracy:
                 best_accuracy = metrics["Accuracy"]
                 best_index = i
             if i == 0:
                 for key in metrics.keys():
                     mean_metrics[key] = metrics[key]
             else:
-                for key in mean_metrics.keys():
-                    mean_metrics[key] += metrics[key]
-        for key in mean_metrics.keys():
+                for key, value in mean_metrics.items():
+                    value += metrics[key]
+        for key in mean_metrics:
             mean_metrics[key] = mean_metrics[key] / len(mlst)
         if verbose:
-            print("Best classifier: {}".format(best_index))
+            print(f"Best classifier: {best_index}")
             print(mlst[best_index])
             print("- Average metrics of classifiers -")
             print(mean_metrics)
 
         return best_index, clfs, mlst, mean_metrics
 
     def train_classifier(
@@ -348,15 +338,15 @@
                 )
                 word_scores[word] = pos_score + neg_score
 
             best_cnt = int(len(word_scores) * best_ratio)
             best = sorted(word_scores.items(), key=lambda item: item[1], reverse=True)[
                 :best_cnt
             ]
-            bestwords = set([w for w, s in best])
+            bestwords = {w for w, s in best}
             if feature_fn_name == "best_trigram_word_feats":
                 feat_fn = best_trigram_word_feats
             elif feature_fn_name == "best_bigram":
                 feat_fn = best_bigram_word_feats
             else:
                 feat_fn = best_word_feats
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/mpko.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/mpko.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,19 +23,18 @@
     def init_tokenizer(self, kind=None):
         self._tokenizer = MPTokenizer(kind, self._poldict)
 
     def init_dict(self, kind=None, intensity_cutoff=None):
         kind = kind if kind in self.KINDS.keys() else 0
         if intensity_cutoff is not None:
             self._intensity_cutoff = intensity_cutoff
+        elif kind in self.INTENSITY_KINDS.keys():
+            self._intensity_cutoff = self.INTENSITY_KINDS[kind]
         else:
-            if kind in self.INTENSITY_KINDS.keys():
-                self._intensity_cutoff = self.INTENSITY_KINDS[kind]
-            else:
-                self._intensity_cutoff = 1.1
+            self._intensity_cutoff = 1.1
         self._intensity_cutoff = min(2, self._intensity_cutoff)
         # print('Initialize the dictionary using a lexicon file: {}'.format(self.KINDS[kind]))
         path = os.path.join(LEXICON_PATH, "mpko", self.KINDS[kind])
         with open(path, encoding="utf-8") as f:
             for line in f:
                 word = line.split(",")
                 w = word[0]
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/sentiment/utils.py` & `ekonlpy-1.2.0/src/ekonlpy/sentiment/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,21 +87,21 @@
         return self.ngramize(tokens)
 
     def ngramize(self, tokens):
         ngram_tokens = []
         tokens = [w for w in tokens if w.split("/")[1] not in self._skiptags]
         for pos in range(len(tokens)):
             for gram in range(1, self._ngram + 1):
-                token = self.get_ngram(tokens, pos, gram)
-                if token:
-                    if self._vocab is None:
+                if token := self.get_ngram(tokens, pos, gram):
+                    if (
+                        self._vocab is not None
+                        and token in self._vocab
+                        or self._vocab is None
+                    ):
                         ngram_tokens.append(token)
-                    else:
-                        if token in self._vocab:
-                            ngram_tokens.append(token)
         return ngram_tokens
 
     def get_ngram(self, tokens, pos, gram):
         if pos < 0:
             return None
         if pos + gram > len(tokens):
             return None
@@ -110,15 +110,15 @@
             token += self._delimiter + tokens[pos + i]
         return token
 
     def morpheme(self, dataset):
         return self.align_morpheme(self._tagger.pos(dataset))
 
     def align_morpheme(self, morpheme):
-        return ["{}/{}".format(w, t) for w, t in morpheme]
+        return [f"{w}/{t}" for w, t in morpheme]
 
 
 class MPTokenizer(BaseTokenizer):
     """
     The default tokenizer for MPKO sub class, which yields 5-gram tokens.
     The output of the tokenizer is tagged by Mecab.
     """
@@ -132,18 +132,15 @@
     def __init__(self, kind=None, vocab=None, keep_overlapping_ngram=False):
         self._kind = kind if kind in self.KINDS.keys() else 0
         self._keep_overlapping_ngram = keep_overlapping_ngram
         self._min_ngram = 1
         self._delimiter = ";"
         self._ngram = self.KINDS[self._kind]
         self._tagger = Mecab()
-        if vocab:
-            self._vocab = vocab
-        else:
-            self._vocab = self.get_vocab(self.FILES["vocab"])
+        self._vocab = vocab if vocab else self.get_vocab(self.FILES["vocab"])
         self._wordset = self.get_wordset(self.FILES["wordset"])
         self._start_tags = {"NNG", "VA", "VAX", "MAG"}
         self._noun_tags = {"NNG"}
 
     def tokenize(self, text):
         if type(text) == list:
             ngram_tokens = []
@@ -157,33 +154,29 @@
 
     def ngramize(self, tokens):
         ngram_tokens = []
         tokens = [w for w in tokens if w in self._wordset]
 
         for pos in range(len(tokens)):
             for gram in range(self._min_ngram, self._ngram + 1):
-                token = self.get_ngram(tokens, pos, gram)
-                if token:
-                    if self._keep_overlapping_ngram:
+                if token := self.get_ngram(tokens, pos, gram):
+                    if (
+                        not self._keep_overlapping_ngram
+                        and token in self._vocab
+                        or self._keep_overlapping_ngram
+                    ):
                         ngram_tokens.append(token)
-                    else:
-                        if token in self._vocab:
-                            ngram_tokens.append(token)
         if not self._keep_overlapping_ngram:
             filtered_tokens = []
-            if len(ngram_tokens) > 0:
+            if ngram_tokens:
                 ngram_tokens = sorted(
                     ngram_tokens, key=lambda item: len(item), reverse=True
                 )
                 for token in ngram_tokens:
-                    existing_token = False
-                    for check_token in filtered_tokens:
-                        if token in check_token:
-                            existing_token = True
-                            break
+                    existing_token = any(token in check_token for check_token in filtered_tokens)
                     if not existing_token:
                         filtered_tokens.append(token)
             ngram_tokens = filtered_tokens
 
         return ngram_tokens
 
     def get_phrase(self, ngram_tokens):
@@ -199,50 +192,45 @@
             return None
         if pos + gram > len(tokens):
             return None
         token = tokens[pos]
         check_noun = False
 
         tag = token.split("/")[1] if "/" in token else None
-        if tag in self._start_tags:
-            if tag in self._noun_tags:
-                check_noun = True
-            for i in range(1, gram):
-                if tokens[pos + i] != tokens[pos + i - 1]:
-                    tag = (
-                        tokens[pos + i].split("/")[1]
-                        if "/" in tokens[pos + i]
-                        else None
-                    )
-                    if tag in self._noun_tags:
-                        check_noun = True
-                    token += self._delimiter + tokens[pos + i]
-            if check_noun:
-                return token
-            else:
-                return None
-        else:
+        if tag not in self._start_tags:
             return None
+        if tag in self._noun_tags:
+            check_noun = True
+        for i in range(1, gram):
+            if tokens[pos + i] != tokens[pos + i - 1]:
+                tag = (
+                    tokens[pos + i].split("/")[1]
+                    if "/" in tokens[pos + i]
+                    else None
+                )
+                if tag in self._noun_tags:
+                    check_noun = True
+                token += self._delimiter + tokens[pos + i]
+        return token if check_noun else None
 
     def get_wordset(self, files):
         wordset = set()
         for file in files:
-            fin = open(os.path.join(LEXICON_PATH, file), "r", encoding="utf-8")
-            for line in fin.readlines():
-                word = line.strip().split()[0]
-                if len(word) > 1:
-                    wordset.add(word)
-            fin.close()
+            with open(os.path.join(LEXICON_PATH, file), "r", encoding="utf-8") as fin:
+                for line in fin:
+                    word = line.strip().split()[0]
+                    if len(word) > 1:
+                        wordset.add(word)
         return wordset
 
     def get_vocab(self, file):
         vocab = {}
         vocab_path = os.path.join(LEXICON_PATH, file)
         with open(vocab_path, "r", encoding="utf-8") as f:
-            for i, line in enumerate(f):
+            for line in f:
                 w = line.strip().split()
                 if len(w[0]) > 0:
                     vocab[w[0]] = w[1]
         return vocab
 
 
 class Tokenizer(BaseTokenizer):
@@ -275,23 +263,22 @@
             "DatesandNumbers.txt",
             "Generic.txt",
             "Geographic.txt",
             "Names.txt",
         ]
         stopset = set()
         for f in files:
-            fin = open("%s/%s" % (LEXICON_PATH, f), "rb")
-            for line in fin.readlines():
-                line = line.decode(encoding="latin-1")
-                match = re.search(r"(\w+)", line)
-                if match is None:
-                    continue
-                word = match.group(1)
-                stopset.add(self._stemmer.stem(word.lower()))
-            fin.close()
+            with open(f"{LEXICON_PATH}/{f}", "rb") as fin:
+                for line in fin:
+                    line = line.decode(encoding="latin-1")
+                    match = re.search(r"(\w+)", line)
+                    if match is None:
+                        continue
+                    word = match[1]
+                    stopset.add(self._stemmer.stem(word.lower()))
         return stopset
 
 
 def calc_polarity(scores, by_count=True):
     eps = 1e-6
     if by_count:
         pos_score = [1 for s in scores if s > 0]
@@ -299,14 +286,19 @@
     else:
         pos_score = [s for s in scores if s > 0]
         neg_score = [s for s in scores if s < 0]
 
     s_pos = sum(pos_score)
     s_neg = sum(neg_score)
 
-    s_pol = (
+    return (
         (s_pos + s_neg)
         * 1.0
-        / (((s_pos - s_neg) if by_count else (len(pos_score) + len(pos_score))) + eps)
+        / (
+            (
+                (s_pos - s_neg)
+                if by_count
+                else (len(pos_score) + len(pos_score))
+            )
+            + eps
+        )
     )
-
-    return s_pol
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/tag/_postprocess.py` & `ekonlpy-1.2.0/src/ekonlpy/tag/_postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             return (w_, w[1]) if isinstance(w_, str) else w_
 
         words = self.base_tagger.pos(phrase)
         if self.stopwords:
             words = [
                 w
                 for w in words
-                if not ((w in self.stopwords) or (w[0] in self.stopwords))
+                if w not in self.stopwords and w[0] not in self.stopwords
             ]
         if self.passwords:
             words = [
                 w for w in words if ((w in self.passwords) or (w[0] in self.passwords))
             ]
         if self.passtags:
             words = [w for w in words if w[1] in self.passtags]
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/utils/dictionary.py` & `ekonlpy-1.2.0/src/ekonlpy/utils/dictionary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Set, Union
+from typing import Dict, List, Optional, Set, Union
 
 term_tags = {
     "COUNTRY": "국가",
     "INDUSTRY": "산업용어",
     "NAME": "명칭",
     "SECTOR": "산업/업종",
     "ENTITY": "기업/종목",
@@ -13,15 +13,15 @@
 }
 
 
 class TermDictionary:
     def __init__(self):
         self._pos2words: Dict[str, Set[str]] = {}
 
-    def add_dictionary(self, words: Union[str, List[str]], tag: str) -> None:
+    def add_dictionary(self, words: Union[str, List[str], Set[str]], tag: str) -> None:
         """
         Add a list of words or a single word to the dictionary under the given tag.
 
         :param words: Words to be added to the dictionary
         :param tag: Tag for the words being added
         """
         if isinstance(words, str):
@@ -40,22 +40,22 @@
 
         def load(filename: str) -> Set[str]:
             try:
                 with open(filename, encoding="utf-8") as f:
                     words = {word.strip().lower() for word in f}
                     return words
             except Exception as e:
-                print("load_dictionary error: %s" % e)
+                print(f"load_dictionary error: {e}")
                 return set()
 
         wordset = self._pos2words.get(tag, set())
         wordset.update(load(fname))
         self._pos2words[tag] = wordset
 
-    def get_tags(self, word: str) -> str:
+    def get_tags(self, word: str) -> Optional[str]:
         """
         Get the tag associated with the given word.
 
         :param word: Word to get the tag for
         :return: The tag associated with the word
         """
         for tag, words in self._pos2words.items():
@@ -84,22 +84,19 @@
 
         :param word: Word to check the tag for
         :param tag: Tag to be checked against
         :return: True if the word has the specified tag, False otherwise
         """
         return word.lower() in self._pos2words.get(tag, {})
 
-    def exists(self, word: str, tag: str = None) -> bool:
+    def exists(self, word: str, tag: Optional[str] = None) -> bool:
         """
         Check if the given word exists in the dictionary under the specified tag, or under any tag if no tag is given.
 
         :param word: Word to check
         :param tag: Tag to be checked against, or None to check all tags
         :return: True if the word exists in the dictionary under the specified tag or any tag, False otherwise
         """
-        if tag in self._pos2words:
-            return True if word.lower() in self._pos2words[tag] else False
+        if tag and tag in self._pos2words:
+            return word.lower() in self._pos2words[tag]
         else:
-            for tag, words in self._pos2words.items():
-                if word.lower() in words:
-                    return True
-            return False
+            return any(word.lower() in words for tag, words in self._pos2words.items())
```

### Comparing `ekonlpy-1.1.7/src/ekonlpy/utils/io.py` & `ekonlpy-1.2.0/src/ekonlpy/utils/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,30 +72,28 @@
     """
     Save vocabulary to a file.
 
     :param vocab: Dictionary of vocabulary to be saved
     :param file_path: File name to save vocabulary
     :param delimiter: Delimiter used to separate words and their values
     """
-    vocab = [(w, c) for w, c in vocab.items()]
+    vocab = list(vocab.items())
     with open(file_path, "w", encoding="utf-8") as f:
         for w, c in vocab:
             f.write(w + delimiter + str(c) + "\n")
 
 
 def save_wordlist(words: List[str], file_path: str) -> None:
     """
     Save a list of words to a file.
 
     :param words: List of words to be saved
     :param file_path: File name to save the list of words
     """
-    print(
-        "Save the list to the file: {}, no. of words: {}".format(file_path, len(words))
-    )
+    print(f"Save the list to the file: {file_path}, no. of words: {len(words)}")
     with open(file_path, "w", encoding="utf-8") as f:
         for word in words:
             f.write(word + "\n")
 
 
 def load_wordlist(
     file_path: str,
@@ -133,30 +131,22 @@
 
     if remove_delimiter:
         words = [word.replace(";", "") for word in words]
 
     if max_ngram:
         words = [word for word in words if len(word.split(";")) <= max_ngram]
 
-    if sort:
-        words = sorted(set(words))
-    else:
-        words = set(words)
-
-    print("Loaded the file: {}, No. of words: {}".format(file_path, len(words)))
+    words = sorted(set(words)) if sort else set(words)
+    print(f"Loaded the file: {file_path}, No. of words: {len(words)}")
 
     if rewrite:
         with open(file_path, "w", encoding="utf-8") as f:
             for word in words:
                 f.write(word + "\n")
-        print(
-            "Saved the words to the file: {}, No. of words: {}".format(
-                file_path, len(words)
-            )
-        )
+        print(f"Saved the words to the file: {file_path}, No. of words: {len(words)}")
 
     words = [word for word in words if not word.startswith("#")]
     words = [
         word.lower() if lowercase else word
         for word in words
         if not word.startswith("#")
     ]
@@ -191,20 +181,17 @@
             if word.split(";")[0] in check_list:
                 return True
         else:
             for w in word.split(";"):
                 if w in check_list:
                     return True
     else:
-        if endswith:
-            for check_word in check_list:
+        for check_word in check_list:
+            if endswith:
                 if word.endswith(check_word.lower()):
                     return True
-        elif startswith:
-            for check_word in check_list:
+            elif startswith:
                 if word.startswith(check_word.lower()):
                     return True
-        else:
-            for check_word in check_list:
-                if check_word.lower() in word:
-                    return True
+            elif check_word.lower() in word:
+                return True
     return False
```

### Comparing `ekonlpy-1.1.7/PKG-INFO` & `ekonlpy-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: ekonlpy
-Version: 1.1.7
+Version: 1.2.0
 Summary: A Korean natural language processing toolkit for economic analysis
 Home-page: https://ekonlpy.entelecheia.ai/
 License: MIT
 Keywords: KoNLPy,Tokenization,Sentiment analysis,Monetary policy
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: fugashi (>=1.2.1,<2.0.0)
 Requires-Dist: mecab-ko-dic (>=1.0.0,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/eKoNLPy
 Description-Content-Type: text/markdown
@@ -41,28 +42,27 @@
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/eKoNLPy
 [release-url]: https://github.com/entelecheia/eKoNLPy/releases
 [pypi-downloads-image]: https://img.shields.io/pypi/dm/ekonlpy
 [codecov-image]: https://codecov.io/gh/entelecheia/eKoNLPy/branch/master/graph/badge.svg?token=8I4ORHRREL
 [codecov-url]: https://codecov.io/gh/entelecheia/eKoNLPy
 [zenodo-image]: https://zenodo.org/badge/DOI/10.5281/zenodo.7809447.svg
 [zenodo-url]: https://doi.org/10.5281/zenodo.7809447
-
 [repo-url]: https://github.com/entelecheia/eKoNLPy
 [pypi-url]: https://pypi.org/project/ekonlpy
 [docs-url]: https://ekonlpy.entelecheia.ai
 [changelog]: https://github.com/entelecheia/eKoNLPy/blob/master/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/eKoNLPy/blob/master/CONTRIBUTING.md
 
 <!-- Links: -->
 
 `eKoNLPy` is a Korean Natural Language Processing (NLP) Python library specifically designed for economic analysis. It extends the functionality of the `MeCab` tagger from KoNLPy to improve the handling of economic terms, financial institutions, and company names, classifying them as single nouns. Additionally, it incorporates sentiment analysis features to determine the tone of monetary policy statements, such as Hawkish or Dovish.
 
-**Important Note:**
-
-eKoNLPy is built on the [fugashi](https://github.com/polm/fugashi) and [mecab-ko-dic](https://github.com/LuminosoInsight/mecab-ko-dic) libraries. For more information on using the `Mecab` tagger, please refer to the [fugashi documentation](https://github.com/polm/fugashi). As eKoNLPy no longer relies on the [KoNLPy](https://konlpy.org) library, Java is not required for its use. This makes eKoNLPy compatible with Windows, Linux, and Mac OS, without the need for Java installation. You can also use eKoNLPy on Google Colab.
+> **Note**
+>
+> eKoNLPy is built on the [fugashi](https://github.com/polm/fugashi) and [mecab-ko-dic](https://github.com/LuminosoInsight/mecab-ko-dic) libraries. For more information on using the `Mecab` tagger, please refer to the [fugashi documentation](https://github.com/polm/fugashi). As eKoNLPy no longer relies on the [KoNLPy](https://konlpy.org) library, Java is not required for its use. This makes eKoNLPy compatible with Windows, Linux, and Mac OS, without the need for Java installation. You can also use eKoNLPy on Google Colab.
 
 If you wish to tokenize general Korean text with eKoNLPy, you do not need to install the `KoNLPy` library. Instead, utilize `ekonlpy.mecab.MeCab` as a replacement for `ekonlpy.tag.Mecab`.
 
 However, if you plan to use the [Korean Sentiment Analyzer (KSA)](#korean-sentiment-analyzer-ksa), which employs the `Kkma` morpheme analyzer, you will need to install the [KoNLPy](https://konlpy.org) library.
 
 ## Installation
 
@@ -75,28 +75,36 @@
 ## Usage
 
 ### Part of Speech Tagging
 
 To use the part of speech tagging feature, input `Mecab.pos(phrase)` just like KoNLPy. First, the input is processed using KoNLPy's Mecab morpheme analyzer. Then, if a combination of consecutive tokens matches a term in the user dictionary, the phrase is separated into compound nouns.
 
 ```python
-from ekonlpy.tag import Mecab
+from ekonlpy import Mecab
 
 mecab = Mecab()
 mecab.pos('금통위는 따라서 물가안정과 병행, 경기상황에 유의하는 금리정책을 펼쳐나가기로 했다고 밝혔다.')
 ```
 
 > [('금', 'MAJ'), ('통', 'MAG'), ('위', 'NNG'), ('는', 'JX'), ('따라서', 'MAJ'), ('물가', 'NNG'), ('안정', 'NNG'), ('과', 'JC'), ('병행', 'NNG'), (',', 'SC'), ('경기', 'NNG'), ('상황', 'NNG'), ('에', 'JKB'), ('유의', 'NNG'), ('하', 'XSV'), ('는', 'ETM'), ('금리', 'NNG'), ('정책', 'NNG'), ('을', 'JKO'), ('펼쳐', 'VV+EC'), ('나가', 'VX'), ('기', 'ETN'), ('로', 'JKB'), ('했', 'VV+EP'), ('다고', 'EC'), ('밝혔', 'VV+EP'), ('다', 'EF'), ('.', 'SF')]
 
+You can also use the Command Line Interface (CLI) to perform part of speech tagging:
+
+```bash
+ekonlpy --input "안녕하세요"
+```
+
+> [('안녕', 'NNG'), ('하', 'XSV'), ('세요', 'EP')]
+
 ### cf. MeCab POS Tagging (fugashi)
 
 ```python
-from ekonlpy.mecab import MeCab # Be careful! `C` is capital.
+from ekonlpy import Mecab
 
-mecab = MeCab()
+mecab = Mecab(use_original_tagger=True) # set use_original_tagger=True
 mecab.pos('금통위는 따라서 물가안정과 병행, 경기상황에 유의하는 금리정책을 펼쳐나가기로 했다고 밝혔다.')
 ```
 
 > [('금', 'MAJ'), ('통', 'MAG'), ('위', 'NNG'), ('는', 'JX'), ('따라서', 'MAJ'), ('물가', 'NNG'), ('안정', 'NNG'), ('과', 'JC'), ('병행', 'NNG'), (',', 'SC'), ('경기', 'NNG'), ('상황', 'NNG'), ('에', 'JKB'), ('유의', 'NNG'), ('하', 'XSV'), ('는', 'ETM'), ('금리', 'NNG'), ('정책', 'NNG'), ('을', 'JKO'), ('펼쳐', 'VV+EC'), ('나가', 'VX'), ('기', 'ETN'), ('로', 'JKB'), ('했', 'VV+EP'), ('다고', 'EC'), ('밝혔', 'VV+EP'), ('다', 'EF'), ('.', 'SF')]
 
 ### Lemmatization and Synonyms
```

