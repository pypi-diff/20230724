# Comparing `tmp/jwskate-0.8.0.tar.gz` & `tmp/jwskate-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwskate-0.8.0.tar", max compression
+gzip compressed data, was "jwskate-0.9.0.tar", max compression
```

## Comparing `jwskate-0.8.0.tar` & `jwskate-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-06-23 11:45:56.677552 jwskate-0.8.0/LICENSE
--rw-r--r--   0        0        0    18475 2023-06-23 11:45:56.677552 jwskate-0.8.0/README.md
--rw-r--r--   0        0        0     3955 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/__init__.py
--rw-r--r--   0        0        0     2639 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/enums.py
--rw-r--r--   0        0        0     2809 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/__init__.py
--rw-r--r--   0        0        0     9503 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/base.py
--rw-r--r--   0        0        0     4716 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/ec.py
--rw-r--r--   0        0        0      323 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/encryption/__init__.py
--rw-r--r--   0        0        0     6207 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/encryption/aescbchmac.py
--rw-r--r--   0        0        0     3322 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/encryption/aesgcm.py
--rw-r--r--   0        0        0     1059 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/__init__.py
--rw-r--r--   0        0        0     2427 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/aesgcmkw.py
--rw-r--r--   0        0        0     2221 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/aeskw.py
--rw-r--r--   0        0        0      740 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/dir.py
--rw-r--r--   0        0        0     9749 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/ecdh.py
--rw-r--r--   0        0        0     3583 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/pbes2.py
--rw-r--r--   0        0        0     3471 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/rsa.py
--rw-r--r--   0        0        0     4766 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/okp.py
--rw-r--r--   0        0        0      621 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/__init__.py
--rw-r--r--   0        0        0     3669 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/ec.py
--rw-r--r--   0        0        0     2421 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/eddsa.py
--rw-r--r--   0        0        0     2058 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/hmac.py
--rw-r--r--   0        0        0     3988 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/rsa.py
--rw-r--r--   0        0        0      216 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwe/__init__.py
--rw-r--r--   0        0        0    12773 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwe/compact.py
--rw-r--r--   0        0        0      796 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/__init__.py
--rw-r--r--   0        0        0     6121 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/alg.py
--rw-r--r--   0        0        0    47667 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/base.py
--rw-r--r--   0        0        0     8264 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/ec.py
--rw-r--r--   0        0        0     6988 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/jwks.py
--rw-r--r--   0        0        0     8275 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/oct.py
--rw-r--r--   0        0        0    11436 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/okp.py
--rw-r--r--   0        0        0    10820 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwk/rsa.py
--rw-r--r--   0        0        0      265 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/__init__.py
--rw-r--r--   0        0        0     6064 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/compact.py
--rw-r--r--   0        0        0    10698 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/json.py
--rw-r--r--   0        0        0     5262 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/signature.py
--rw-r--r--   0        0        0      413 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/__init__.py
--rw-r--r--   0        0        0     9410 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/base.py
--rw-r--r--   0        0        0    11659 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/signed.py
--rw-r--r--   0        0        0     6688 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/signer.py
--rw-r--r--   0        0        0     5036 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/verifier.py
--rw-r--r--   0        0        0        0 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/py.typed
--rw-r--r--   0        0        0     4969 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/token.py
--rw-r--r--   0        0        0     2360 2023-06-23 11:45:56.681552 jwskate-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       75 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/.pydocstyle
--rw-r--r--   0        0        0       37 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     2236 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/__init__.py
--rw-r--r--   0        0        0     2276 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_base.py
--rw-r--r--   0        0        0     2915 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_encryption.py
--rw-r--r--   0        0        0     7279 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_examples.py
--rw-r--r--   0        0        0     1601 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_key_mgmt.py
--rw-r--r--   0        0        0      259 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_signature.py
--rw-r--r--   0        0        0    31129 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwe.py
--rw-r--r--   0        0        0        0 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/__init__.py
--rw-r--r--   0        0        0     3962 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_alg.py
--rw-r--r--   0        0        0     4704 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_ec.py
--rw-r--r--   0        0        0     4316 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_generate.py
--rw-r--r--   0        0        0    21121 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_jwk.py
--rw-r--r--   0        0        0    11153 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_jwks.py
--rw-r--r--   0        0        0    11281 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_okp.py
--rw-r--r--   0        0        0    17351 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_rsa.py
--rw-r--r--   0        0        0     2425 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_symmetric.py
--rw-r--r--   0        0        0    22043 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jws.py
--rw-r--r--   0        0        0    25653 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwt.py
--rw-r--r--   0        0        0    19452 1970-01-01 00:00:00.000000 jwskate-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-24 14:48:00.942355 jwskate-0.9.0/LICENSE
+-rw-r--r--   0        0        0    19751 2023-07-24 14:48:00.942355 jwskate-0.9.0/README.md
+-rw-r--r--   0        0        0     3991 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/__init__.py
+-rw-r--r--   0        0        0     2713 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/enums.py
+-rw-r--r--   0        0        0     2844 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/__init__.py
+-rw-r--r--   0        0        0     9401 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/base.py
+-rw-r--r--   0        0        0     4683 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/ec.py
+-rw-r--r--   0        0        0      358 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/encryption/__init__.py
+-rw-r--r--   0        0        0     6173 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/encryption/aescbchmac.py
+-rw-r--r--   0        0        0     3303 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/encryption/aesgcm.py
+-rw-r--r--   0        0        0     1094 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/__init__.py
+-rw-r--r--   0        0        0     2419 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/aesgcmkw.py
+-rw-r--r--   0        0        0     2244 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/aeskw.py
+-rw-r--r--   0        0        0      750 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/dir.py
+-rw-r--r--   0        0        0     9729 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/ecdh.py
+-rw-r--r--   0        0        0     3600 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/pbes2.py
+-rw-r--r--   0        0        0     3493 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/key_mgmt/rsa.py
+-rw-r--r--   0        0        0     4734 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/okp.py
+-rw-r--r--   0        0        0      656 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/signature/__init__.py
+-rw-r--r--   0        0        0     3674 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/signature/ec.py
+-rw-r--r--   0        0        0     2438 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/signature/eddsa.py
+-rw-r--r--   0        0        0     2062 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/signature/hmac.py
+-rw-r--r--   0        0        0     3999 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwa/signature/rsa.py
+-rw-r--r--   0        0        0      251 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwe/__init__.py
+-rw-r--r--   0        0        0    12661 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwe/compact.py
+-rw-r--r--   0        0        0      831 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/__init__.py
+-rw-r--r--   0        0        0     6109 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/alg.py
+-rw-r--r--   0        0        0    47377 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/base.py
+-rw-r--r--   0        0        0     8223 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/ec.py
+-rw-r--r--   0        0        0     6962 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/jwks.py
+-rw-r--r--   0        0        0     8187 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/oct.py
+-rw-r--r--   0        0        0    11414 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/okp.py
+-rw-r--r--   0        0        0    11360 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwk/rsa.py
+-rw-r--r--   0        0        0      300 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jws/__init__.py
+-rw-r--r--   0        0        0     5995 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jws/compact.py
+-rw-r--r--   0        0        0    10588 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jws/json.py
+-rw-r--r--   0        0        0     5198 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jws/signature.py
+-rw-r--r--   0        0        0      448 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwt/__init__.py
+-rw-r--r--   0        0        0     9646 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwt/base.py
+-rw-r--r--   0        0        0    11617 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwt/signed.py
+-rw-r--r--   0        0        0     6630 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwt/signer.py
+-rw-r--r--   0        0        0     5023 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/jwt/verifier.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/py.typed
+-rw-r--r--   0        0        0     4986 2023-07-24 14:48:00.942355 jwskate-0.9.0/jwskate/token.py
+-rw-r--r--   0        0        0     2306 2023-07-24 14:48:00.942355 jwskate-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/.pydocstyle
+-rw-r--r--   0        0        0       72 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2271 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/test_jwa/__init__.py
+-rw-r--r--   0        0        0     2287 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/test_jwa/test_base.py
+-rw-r--r--   0        0        0     2950 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/test_jwa/test_encryption.py
+-rw-r--r--   0        0        0     7315 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/test_jwa/test_examples.py
+-rw-r--r--   0        0        0     1602 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/test_jwa/test_key_mgmt.py
+-rw-r--r--   0        0        0      294 2023-07-24 14:48:00.942355 jwskate-0.9.0/tests/test_jwa/test_signature.py
+-rw-r--r--   0        0        0    31117 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwe.py
+-rw-r--r--   0        0        0        0 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/__init__.py
+-rw-r--r--   0        0        0     3998 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_alg.py
+-rw-r--r--   0        0        0     4740 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_ec.py
+-rw-r--r--   0        0        0     4328 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_generate.py
+-rw-r--r--   0        0        0    21132 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_jwk.py
+-rw-r--r--   0        0        0    11183 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_jwks.py
+-rw-r--r--   0        0        0    11303 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_okp.py
+-rw-r--r--   0        0        0    18004 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_rsa.py
+-rw-r--r--   0        0        0     2461 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwk/test_symmetric.py
+-rw-r--r--   0        0        0    22082 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jws.py
+-rw-r--r--   0        0        0    25822 2023-07-24 14:48:00.946355 jwskate-0.9.0/tests/test_jwt.py
+-rw-r--r--   0        0        0    20711 1970-01-01 00:00:00.000000 jwskate-0.9.0/PKG-INFO
```

### Comparing `jwskate-0.8.0/LICENSE` & `jwskate-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jwskate-0.8.0/README.md` & `jwskate-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 
 [![PyPi](https://img.shields.io/pypi/v/jwskate.svg)](https://pypi.python.org/pypi/jwskate)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A Pythonic implementation of the JOSE set of IETF specifications: [Json Web Signature][rfc7515], [Keys][rfc7517],
 [Algorithms][rfc7518], [Tokens][rfc7519] and [Encryption][rfc7516] (RFC7515 to 7519), and their extensions
 [ECDH Signatures][rfc8037] (RFC8037), [JWK Thumbprints][rfc7638] (RFC7638), and [JWK Thumbprint URI][rfc9278] (RFC9278),
-and with respect to [JWT Best Current Practices][rfc8725].
+and with respects to [JWT Best Current Practices][rfc8725] (RFC8725).
 
 - Free software: MIT
 - Documentation: [https://guillp.github.io/jwskate/](https://guillp.github.io/jwskate/)
 
-A quick usage example, generating an RSA private key, signing some data, then validating that signature:
+Here is a quick usage example: generating a private RSA key, signing some data, then validating that signature with the matching public key:
 
 ```python
 from jwskate import Jwk
 
 # Let's generate a random private key, to use with alg 'RS256'.
 # Based on that alg, jwskate knows it must be an RSA key.
+# RSA keys can be of variable size, so let's pass the requested key size as parameter
 rsa_private_jwk = Jwk.generate(alg="RS256", key_size=2048)
 
-data = b"Signing is easy!"
-signature = rsa_private_jwk.sign(data)
+data = b"Signing is easy!"  # we will sign this
+signature = rsa_private_jwk.sign(data)  # done!
 
-# extract the public key, and verify the signature with it
+# now extract the public key, and verify the signature with it
 rsa_public_jwk = rsa_private_jwk.public_jwk()
 assert rsa_public_jwk.verify(data, signature)
 
 # let's see what a Jwk looks like:
 assert isinstance(rsa_private_jwk, dict)  # Jwk are dict
 
 print(rsa_private_jwk.with_usage_parameters())
@@ -47,49 +48,61 @@
  'qi': '...',
  'alg': 'RS256',
  'kid': '...',
  'use': 'sig',
  'key_ops': ['sign']}
 ```
 
-Now let's sign a JWT containing arbitrary claims, this time using an EC key:
+Now let's sign a JWT containing arbitrary claims, this time using an Elliptic Curve (`EC`) key:
 
 ```python
 from jwskate import Jwk, Jwt
 
 # This time let's try an EC key, based on `alg` parameter,
-# and let's specigy an arbitrary Key ID (kid).
+# and let's specify an arbitrary Key ID (kid).
+# additional args are either options (like 'key_size' above for RSA keys)
+# or additional parameters to include in the JWK
 private_jwk = Jwk.generate(alg="ES256", kid="my_key")
+# note that based only on the `alg` value, the appropriate key type and curve
+# are automatically deduced and included in the JWK
+print(private_jwk)
+# {'kty': 'EC', 'crv': 'P-256', 'x': 'Ppe...', 'y': '9Si...', 'd': 'g09...', 'alg': 'ES256'}
+assert private_jwk.kty == "EC"
+assert private_jwk.crv == "P-256"
+assert private_jwk.alg == "ES256"
+# this is a private key and 'ES256' is a signature alg, so 'use' and 'key_ops' can also be deduced:
+assert private_jwk.use == "sig"
+assert private_jwk.key_ops == ("sign",)
 
-# here are claims to sign in a JWT:
+# here are the claims to sign in a JWT:
 claims = {"sub": "some_sub", "claim1": "value1"}
 
 jwt = Jwt.sign(claims, private_jwk)
-# that's it! we have a signed JWT
+# that's it! we have a signed JWT.
+print(jwt)
+# eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.SBQIlGlFdwoEMViWUFsBmCsXShtOq4lnp3Im5ZVh1PFCGJFdW-dTG9qJjlFSAA_BkM5PF9u38PL7Ai9cC2_DJw
 assert isinstance(jwt, Jwt)  # Jwt are objects
 assert jwt.claims == claims  # claims can be accessed as a dict
-assert jwt.headers == {"alg": "ES256", "kid": "my_key"}  # headers too
+assert jwt.headers == {"typ": "JWT", "alg": "ES256", "kid": "my_key"}  # headers too
 assert jwt.sub == "some_sub"  # individual claims can be accessed as attributes
 assert jwt["claim1"] == "value1"  # or as dict items (with "subscription")
 assert jwt.alg == "ES256"  # alg and kid headers are also accessible as attributes
 assert jwt.kid == private_jwk.kid
-# notice that alg and kid are automatically set with appropriate values
+# notice that alg and kid are automatically set with appropriate values taken from our private jwk
 assert isinstance(jwt.signature, bytes)  # signature is accessible too
 # verifying the jwt signature is as easy as:
 assert jwt.verify_signature(private_jwk.public_jwk())
 # since our jwk contains an 'alg' parameter (here 'ES256'), the signature is automatically verified using that alg
 # you could also specify an alg manually, useful for keys with no "alg" hint:
 assert jwt.verify_signature(private_jwk.public_jwk(), alg="ES256")
-
-print(jwt)
-# eyJhbGciOiJFUzI1NiIsImtpZCI6Im15a2V5In0.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.C1KcDyDT8qXwUqcWzPKkQD7f6xai-gCgaRFMdKPe80Vk7XeYNa8ovuLwvdXgGW4ZZ_lL73QIyncY7tHGXUthag
-# This will output the full JWT compact representation. You can inspect it for example at <https://jwt.io>
+# note that jwskate will only trust the alg(s) you provide as parameter, either part of the JWK
+# or with `alg` or `algs` params, and will ignore the 'alg' that is set in the JWT, for security reasons.
 ```
 
-Or let's sign a JWT with the standardised lifetime, subject, audience and ID claims, plus arbitrary custom claims:
+Now let's sign a JWT with the standardised lifetime, subject, audience and ID claims, plus arbitrary custom claims:
 
 ```python
 from jwskate import Jwk, JwtSigner
 
 private_jwk = Jwk.generate(alg="ES256")
 signer = JwtSigner(issuer="https://myissuer.com", jwk=private_jwk)
 jwt = signer.sign(
@@ -97,15 +110,16 @@
     audience="some_aud",
     extra_claims={"custom_claim1": "value1", "custom_claim2": "value2"},
 )
 
 print(jwt.claims)
 ```
 
-The generated JWT claims will include the standardised claims:
+The generated JWT will include the standardised claims (`iss`, `aud`, `sub`, `iat`, `exp` and `jti`),
+together with the `extra_claims` provided to `.sign()`:
 
 ```
 {'custom_claim1': 'value1',
  'custom_claim2': 'value2',
  'iss': 'https://myissuer.com',
  'aud': 'some_aud',
  'sub': 'some_sub',
@@ -137,107 +151,107 @@
 | Json Web Signature (JWS)  | ☑ Compact<br/> ☑ JSON Flat <br/> ☑ JSON General <br/> |
 | Json Web Encryption (JWE) | ☑ Compact<br/> ☐ JSON Flat <br/> ☐ JSON General <br/> |
 | Json Web Tokens (JWT)     | ☑ Signed<br/> ☑ Signed and Encrypted                   |
 
 ### Supported Signature algorithms
 
 
-| Signature Alg | Description                                    | Key Type | Reference                          | Note                           |
-| ------------- | ---------------------------------------------- | -------- | ---------------------------------- | ------------------------------ |
-| HS256         | HMAC using SHA-256                             | oct      | [RFC7518, Section 3.2]             |                                |
-| HS384         | HMAC using SHA-384                             | oct      | [RFC7518, Section 3.2]             |                                |
-| HS512         | HMAC using SHA-512                             | oct      | [RFC7518, Section 3.2]             |                                |
-| RS256         | RSASSA-PKCS1-v1_5 using SHA-256                | RSA      | [RFC7518, Section 3.3]             |                                |
-| RS384         | RSASSA-PKCS1-v1_5 using SHA-384                | RSA      | [RFC7518, Section 3.3]             |                                |
-| RS512         | RSASSA-PKCS1-v1_5 using SHA-512                | RSA      | [RFC7518, Section 3.3]             |                                |
-| ES256         | ECDSA using P-256 and SHA-256                  | EC       | [RFC7518, Section 3.4]             |                                |
-| ES384         | ECDSA using P-384 and SHA-384                  | EC       | [RFC7518, Section 3.4]             |                                |
-| ES512         | ECDSA using P-521 and SHA-512                  | EC       | [RFC7518, Section 3.4]             |                                |
-| PS256         | RSASSA-PSS using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 3.5]             |                                |
-| PS384         | RSASSA-PSS using SHA-384 and MGF1 with SHA-384 | RSA      | [RFC7518, Section 3.5]             |                                |
-| PS512         | RSASSA-PSS using SHA-512 and MGF1 with SHA-512 | RSA      | [RFC7518, Section 3.5]             |                                |
-| EdDSA         | EdDSA signature algorithms                     | OKP      | [RFC8037, Section 3.1]             | Ed2219 and Ed448 are supported |
-| ES256K        | ECDSA using secp256k1 curve and SHA-256        | EC       | [RFC8812, Section 3.2]             |                                |
-| HS1           | HMAC using SHA-1                               | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
-| RS1           | RSASSA-PKCS1-v1_5 with SHA-1                   | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
-| none          | No digital signature or MAC performed          |          | [RFC7518, Section 3.6]             | Not usable by mistake          |
+| Signature Alg   | Description                                      | Key Type | Reference                          | Note                           |
+|-----------------|--------------------------------------------------|----------| ---------------------------------- | ------------------------------ |
+| `HS256`         | HMAC using SHA-256                               | `oct`    | [RFC7518, Section 3.2]             |                                |
+| `HS384`         | HMAC using SHA-384                               | `oct`    | [RFC7518, Section 3.2]             |                                |
+| `HS512`         | HMAC using SHA-512                               | `oct`    | [RFC7518, Section 3.2]             |                                |
+| `RS256`         | RSASSA-PKCS1-v1_5 using SHA-256                  | `RSA`    | [RFC7518, Section 3.3]             |                                |
+| `RS384`         | RSASSA-PKCS1-v1_5 using SHA-384                  | `RSA`    | [RFC7518, Section 3.3]             |                                |
+| `RS512`         | RSASSA-PKCS1-v1_5 using SHA-512                  | `RSA`    | [RFC7518, Section 3.3]             |                                |
+| `ES256`         | ECDSA using P-256 and SHA-256                    | `EC`     | [RFC7518, Section 3.4]             |                                |
+| `ES384`         | ECDSA using P-384 and SHA-384                    | `EC`     | [RFC7518, Section 3.4]             |                                |
+| `ES512`         | ECDSA using P-521 and SHA-512                    | `EC`     | [RFC7518, Section 3.4]             |                                |
+| `PS256`         | RSASSA-PSS using SHA-256 and MGF1 with SHA-256   | `RSA`    | [RFC7518, Section 3.5]             |                                |
+| `PS384`         | RSASSA-PSS using SHA-384 and MGF1 with SHA-384   | `RSA`    | [RFC7518, Section 3.5]             |                                |
+| `PS512`         | RSASSA-PSS using SHA-512 and MGF1 with SHA-512   | `RSA`    | [RFC7518, Section 3.5]             |                                |
+| `EdDSA`         | EdDSA signature algorithms                       | `OKP`    | [RFC8037, Section 3.1]             | Ed2219 and Ed448 are supported |
+| `ES256K`        | ECDSA using secp256k1 curve and SHA-256          | `EC`     | [RFC8812, Section 3.2]             |                                |
+| `HS1`           | HMAC using SHA-1                                 | `oct`    | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
+| `RS1`           | RSASSA-PKCS1-v1_5 with SHA-1                     | `oct`    | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
+| `none`          | No digital signature or MAC performed            |          | [RFC7518, Section 3.6]             | Not usable by mistake          |
 
 ### Supported Key Management algorithms
 
 
-| Signature Alg      | Description                                    | Key Type | Reference                          | Note        |
-| ------------------ | ---------------------------------------------- | -------- | ---------------------------------- | ----------- |
-| RSA1_5             | RSAES-PKCS1-v1_5                               | RSA      | [RFC7518, Section 4.2]             | Unwrap Only |
-| RSA-OAEP           | RSAES OAEP using default parameters            | RSA      | [RFC7518, Section 4.3]             |             |
-| RSA-OAEP-256       | RSAES OAEP using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 4.3]             |             |
-| RSA-OAEP-384       | RSA-OAEP using SHA-384 and MGF1 with SHA-384   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
-| RSA-OAEP-512       | RSA-OAEP using SHA-512 and MGF1 with SHA-512   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
-| A128KW             | AES Key Wrap using 128-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
-| A192KW             | AES Key Wrap using 192-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
-| A256KW             | AES Key Wrap using 256-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
-| dir                | Direct use of a shared symmetric key           | oct      | [RFC7518, Section 4.5]             |             |
-| ECDH-ES            | ECDH-ES using Concat KDF                       | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A128KW     | ECDH-ES using Concat KDF and "A128KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A192KW     | ECDH-ES using Concat KDF and "A192KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A256KW     | ECDH-ES using Concat KDF and "A256KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
-| A128GCMKW          | Key wrapping with AES GCM using 128-bit key    | oct      | [RFC7518, Section 4.7]             |             |
-| A192GCMKW          | Key wrapping with AES GCM using 192-bit key    | oct      | [RFC7518, Section 4.7]             |             |
-| A256GCMKW          | Key wrapping with AES GCM using 256-bit key    | oct      | [RFC7518, Section 4.7]             |             |
-| PBES2-HS256+A128KW | PBES2 with HMAC SHA-256 and "A128KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
-| PBES2-HS384+A192KW | PBES2 with HMAC SHA-384 and "A192KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
-| PBES2-HS512+A256KW | PBES2 with HMAC SHA-512 and "A256KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+| Signature Alg      | Description                                    | Key Type      | Reference                          | Note        |
+| ------------------ | ---------------------------------------------- |---------------| ---------------------------------- | ----------- |
+| `RSA1_5`             | RSAES-PKCS1-v1_5                               | `RSA`       | [RFC7518, Section 4.2]             | Unwrap Only |
+| `RSA-OAEP`           | RSAES OAEP using default parameters            | `RSA`       | [RFC7518, Section 4.3]             |             |
+| `RSA-OAEP-256`       | RSAES OAEP using SHA-256 and MGF1 with SHA-256 | `RSA`       | [RFC7518, Section 4.3]             |             |
+| `RSA-OAEP-384`       | RSA-OAEP using SHA-384 and MGF1 with SHA-384   | `RSA`       | https://www.w3.org/TR/WebCryptoAPI |             |
+| `RSA-OAEP-512`       | RSA-OAEP using SHA-512 and MGF1 with SHA-512   | `RSA`       | https://www.w3.org/TR/WebCryptoAPI |             |
+| `A128KW`             | AES Key Wrap using 128-bit key                 | `oct`       | [RFC7518, Section 4.4]             |             |
+| `A192KW`             | AES Key Wrap using 192-bit key                 | `oct`       | [RFC7518, Section 4.4]             |             |
+| `A256KW`             | AES Key Wrap using 256-bit key                 | `oct`       | [RFC7518, Section 4.4]             |             |
+| `A128GCMKW`          | Key wrapping with AES GCM using 128-bit key    | `oct`       | [RFC7518, Section 4.7]             |             |
+| `A192GCMKW`          | Key wrapping with AES GCM using 192-bit key    | `oct`       | [RFC7518, Section 4.7]             |             |
+| `A256GCMKW`          | Key wrapping with AES GCM using 256-bit key    | `oct`       | [RFC7518, Section 4.7]             |             |
+| `dir`                | Direct use of a shared symmetric key           | `oct`       | [RFC7518, Section 4.5]             |             |
+| `ECDH-ES`            | ECDH-ES using Concat KDF                       | `EC`        | [RFC7518, Section 4.6]             |             |
+| `ECDH-ES+A128KW`     | ECDH-ES using Concat KDF and "A128KW" wrapping | `EC`        | [RFC7518, Section 4.6]             |             |
+| `ECDH-ES+A192KW`     | ECDH-ES using Concat KDF and "A192KW" wrapping | `EC`        | [RFC7518, Section 4.6]             |             |
+| `ECDH-ES+A256KW`     | ECDH-ES using Concat KDF and "A256KW" wrapping | `EC`        | [RFC7518, Section 4.6]             |             |
+| `PBES2-HS256+A128KW` | PBES2 with HMAC SHA-256 and "A128KW" wrapping  | `password`  | [RFC7518, Section 4.8]             |             |
+| `PBES2-HS384+A192KW` | PBES2 with HMAC SHA-384 and "A192KW" wrapping  | `password`  | [RFC7518, Section 4.8]             |             |
+| `PBES2-HS512+A256KW` | PBES2 with HMAC SHA-512 and "A256KW" wrapping  | `password`  | [RFC7518, Section 4.8]             |             |
 
 ### Supported Encryption algorithms
 
 
 | Signature Alg | Description                                                 | Reference                |
 | ------------- | ----------------------------------------------------------- | ------------------------ |
-| A128CBC-HS256 | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
-| A192CBC-HS384 | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
-| A256CBC-HS512 | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
-| A128GCM       | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
-| A192GCM       | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
-| A256GCM       | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
+| `A128CBC-HS256` | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
+| `A192CBC-HS384` | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
+| `A256CBC-HS512` | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
+| `A128GCM`       | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
+| `A192GCM`       | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
+| `A256GCM`       | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
 
 ### Supported Elliptic Curves
 
 
-| Curve     | Description                           | Key Type | Usage                 | Reference                  |
-| --------- | ------------------------------------- | -------- | --------------------- | -------------------------- |
-| P-256     | P-256 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
-| P-384     | P-384 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
-| P-521     | P-521 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
-| Ed25519   | Ed25519 signature algorithm key pairs | OKP      | signature             | [RFC8037, Section 3.1]     |
-| Ed448     | Ed448 signature algorithm key pairs   | OKP      | signature             | [RFC8037, Section 3.1]     |
-| X25519    | X25519 function key pairs             | OKP      | encryption            | [RFC8037, Section 3.2]     |
-| X448      | X448 function key pairs               | OKP      | encryption            | [RFC8037, Section 3.2]     |
-| secp256k1 | SECG secp256k1 curve                  | EC       | signature, encryption | [RFC8812, Section 3.1]     |
+| Curve       | Description                           | Key Type | Usage                 | Reference                  |
+|-------------|---------------------------------------|----------| --------------------- | -------------------------- |
+| `P-256`     | P-256 Curve                           | `EC`     | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| `P-384`     | P-384 Curve                           | `EC`     | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| `P-521`     | P-521 Curve                           | `EC`     | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| `Ed25519`   | Ed25519 signature algorithm key pairs | `OKP`    | signature             | [RFC8037, Section 3.1]     |
+| `Ed448`     | Ed448 signature algorithm key pairs   | `OKP`    | signature             | [RFC8037, Section 3.1]     |
+| `X25519`    | X25519 function key pairs             | `OKP`    | encryption            | [RFC8037, Section 3.2]     |
+| `X448`      | X448 function key pairs               | `OKP`    | encryption            | [RFC8037, Section 3.2]     |
+| `secp256k1` | SECG secp256k1 curve                  | `EC`     | signature, encryption | [RFC8812, Section 3.1]     |
 
 ## Why a new lib ?
 
 There are already multiple modules implementing JOSE and Json Web Crypto related specifications in Python. However, I
 have been dissatisfied by all of them so far, so I decided to come up with my own module.
 
 - [PyJWT](https://pyjwt.readthedocs.io)
 - [JWCrypto](https://jwcrypto.readthedocs.io/)
 - [Python-JOSE](https://python-jose.readthedocs.io/)
 - [AuthLib](https://docs.authlib.org/en/latest/jose/)
 
 Not to say that those are _bad_ libs (I actually use `jwcrypto` myself for `jwskate` unit tests), but they either don't
-support some important features, lack documentation, or generally have APIs that don't feel easy-enough, Pythonic-enough
+support some important features, lack documentation, or more generally have APIs that don't feel easy-enough, Pythonic-enough
 to use.
 
 ## Design
 
 ### JWK are dicts
 
 JWK are specified as JSON objects, which are parsed as `dict` in Python. The `Jwk` class in `jwskate` is actually a
-`dict` subclass, so you can use it exactly like you would use a dict: you can access its members, dump it back as JSON,
-etc. The same is true for Signed or Encrypted Json Web tokens in JSON format. You cannot change the key cryptographic
-material, however, since that would lead to unusable keys.
+`dict` subclass, so you can use it exactly like you would use a `dict`: you can access its members, dump it back as JSON,
+etc. The same is true for Signed or Encrypted Json Web tokens in JSON format. However, you cannot change the key cryptographic
+materials, since that would lead to unusable keys.
 
 ### JWA Wrappers
 
 You can use `cryptography` to do the cryptographic operations that are described in
 [JWA](https://www.rfc-editor.org/info/rfc7518), but since `cryptography` is a general purpose library, its usage is not
 straightforward and gives you plenty of options to carefully select and combine, leaving room for mistakes, errors and
 confusion. It has also a quite inconsistent API to handle the different type of keys and algorithms. To work around
```

### Comparing `jwskate-0.8.0/jwskate/__init__.py` & `jwskate-0.9.0/jwskate/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 The `jwskate` module implements the various Json Web Crypto-related
 standards: JWA, JWK, JWKS, JWE, JWT. Each standard has its own submodule, but
 for convenience, you can import any class or component directly from the root
 `jwskate` module.
 
 `jwskate` doesn't implement any actual cryptographic operation, it just
 provides a set of convenient wrappers around the `cryptography` module.
+
 """
+from __future__ import annotations
 
 __author__ = """Guillaume Pujol"""
 __email__ = "guill.p.linux@gmail.com"
 
 from .enums import EncryptionAlgs, KeyManagementAlgs, KeyTypes, SignatureAlgs
 from .jwa import (
     A128CBC_HS256,
```

### Comparing `jwskate-0.8.0/jwskate/enums.py` & `jwskate-0.9.0/jwskate/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """This module contains enums for the various identifiers used in JWA and JWK.
 
 See [IANA JOSE](https://www.iana.org/assignments/jose/jose.xhtml).
 
 """
+from __future__ import annotations
 
 
 class SignatureAlgs:
     """Identifiers for Signature algorithms."""
 
     RS256 = "RS256"
     RS384 = "RS384"
     RS512 = "RS512"
     ES256 = "ES256"
+    ES256k = "ES256k"
     ES384 = "ES384"
     ES512 = "ES512"
     PS256 = "PS256"
     PS384 = "PS384"
     PS512 = "PS512"
     EdDSA = "EdDSA"
 
@@ -25,14 +27,15 @@
 
     ALL_SYMMETRIC = {HS256, HS384, HS512}
     ALL_ASYMMETRIC = {
         RS256,
         RS384,
         RS512,
         ES256,
+        ES256k,
         ES384,
         ES512,
         PS256,
         PS384,
         PS512,
         EdDSA,
     }
@@ -108,13 +111,13 @@
         PBES2_HS512_A256KW,
     }
     ALL_KEY_BASED = ALL_ASYMMETRIC | ALL_SYMMETRIC
     ALL = ALL_ASYMMETRIC | ALL_SYMMETRIC | ALL_PASSWORD_BASED
 
 
 class KeyTypes:
-    """Identifier for Key Types (kty)."""
+    """Identifiers for Key Types (kty)."""
 
     OCT = "oct"
     RSA = "RSA"
     EC = "EC"
     OKP = "OKP"
```

### Comparing `jwskate-0.8.0/jwskate/jwa/__init__.py` & `jwskate-0.9.0/jwskate/jwa/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Each algorithm is represented as a wrapper around a symmetric or asymmetric key, and exposes the
 cryptographic operations as methods. The cryptographic operations themselves are delegated to
 `cryptography`.
 
 [RFC7518]: https://www.rfc-editor.org/rfc/rfc7518
 
 """
+from __future__ import annotations
 
 from .base import (
     BaseAESEncryptionAlg,
     BaseAlg,
     BaseAsymmetricAlg,
     BaseKeyManagementAlg,
     BaseSignatureAlg,
```

### Comparing `jwskate-0.8.0/jwskate/jwa/base.py` & `jwskate-0.9.0/jwskate/jwa/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implement base classes for the algorithms defined in JWA."""
-
 from __future__ import annotations
 
 from contextlib import contextmanager
-from typing import Generic, Iterator, SupportsBytes, Tuple, Type, TypeVar, Union
+from typing import Generic, Iterator, SupportsBytes, TypeVar
 
 import cryptography.exceptions
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from typing_extensions import Self, override
 
 
@@ -84,14 +83,15 @@
         This is a convenience wrapper around `check_key(key)`.
 
         Args:
           key: the key to check for this alg class
 
         Returns:
           `True` if the key is suitable for this alg class, `False` otherwise
+
         """
         try:
             cls.check_key(key)
             return True
         except Exception:
             return False
 
@@ -107,23 +107,23 @@
     the provided key type.
 
     Args:
         key: the key to use.
 
     """
 
-    private_key_class: Union[Type[Kpriv], Tuple[Type[Kpriv], ...]]
-    public_key_class: Union[Type[Kpub], Tuple[Type[Kpub], ...]]
+    private_key_class: type[Kpriv] | tuple[type[Kpriv], ...]
+    public_key_class: type[Kpub] | tuple[type[Kpub], ...]
 
-    def __init__(self, key: Union[Kpriv, Kpub]):
+    def __init__(self, key: Kpriv | Kpub):
         self.check_key(key)
         self.key = key
 
     @classmethod
-    def check_key(cls, key: Union[Kpriv, Kpub]) -> None:
+    def check_key(cls, key: Kpriv | Kpub) -> None:
         """Check that a given key is suitable for this alg class.
 
         This must be implemented by subclasses as required.
 
         Args:
           key: the key to use.
 
@@ -179,28 +179,28 @@
 
 class BaseSignatureAlg(BaseAlg):
     """Base class for signature algorithms."""
 
     use = "sig"
     hashing_alg: hashes.HashAlgorithm
 
-    def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:
+    def sign(self, data: bytes | SupportsBytes) -> BinaPy:
         """Sign arbitrary data, return the signature.
 
         Args:
           data: raw data to sign
 
         Returns:
           the raw signature
 
         """
         raise NotImplementedError
 
     def verify(
-        self, data: Union[bytes, SupportsBytes], signature: Union[bytes, SupportsBytes]
+        self, data: bytes | SupportsBytes, signature: bytes | SupportsBytes
     ) -> bool:
         """Verify a signature against some data.
 
         Args:
           data: the raw data to verify
           signature: the raw signature
 
@@ -254,19 +254,19 @@
             a random IV
 
         """
         return BinaPy.random_bits(cls.iv_size)
 
     def encrypt(
         self,
-        plaintext: Union[bytes, SupportsBytes],
+        plaintext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
-    ) -> Tuple[BinaPy, BinaPy]:
+        iv: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
+    ) -> tuple[BinaPy, BinaPy]:
         """Encrypt arbitrary data, with optional Authenticated Encryption.
 
         This needs as parameters:
 
         - the raw data to encrypt (`plaintext`)
         - a given random Initialisation Vector (`iv`) of the appropriate size
         - optional Additional Authentication Data (`aad`)
@@ -282,19 +282,19 @@
           a tuple of ciphered data and authentication tag
 
         """
         raise NotImplementedError
 
     def decrypt(
         self,
-        ciphertext: Union[bytes, SupportsBytes],
+        ciphertext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        auth_tag: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
+        iv: bytes | SupportsBytes,
+        auth_tag: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
     ) -> BinaPy:
         """Decrypt and verify a ciphertext with Authenticated Encryption.
 
         This needs:
         - the raw encrypted Data (`ciphertext`) and Authentication Tag (`auth_tag`) that were produced by encryption,
         - the same Initialisation Vector (`iv`) and optional Additional Authentication Data that were provided for encryption.
         and returns the resulting clear text data.
```

### Comparing `jwskate-0.8.0/jwskate/jwa/ec.py` & `jwskate-0.9.0/jwskate/jwa/ec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module contains classes that describe Elliptic Curves as described in RFC7518."""
-
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, ClassVar, Dict, Tuple, Union
+from typing import Any, ClassVar
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives.asymmetric import ec
 
 from jwskate import KeyTypes
 
 
@@ -28,22 +27,22 @@
 
     cryptography_curve: ec.EllipticCurve
     """`cryptography` curve instance."""
 
     coordinate_size: int
     """Coordinate size, in bytes."""
 
-    instances: ClassVar[Dict[str, EllipticCurve]] = {}
+    instances: ClassVar[dict[str, EllipticCurve]] = {}
     """Registry of subclasses, in a {name: instance} mapping."""
 
     def __post_init__(self) -> None:
         """Automatically register subclasses in the instance registry."""
         self.instances[self.name] = self
 
-    def generate(self) -> Tuple[int, int, int]:
+    def generate(self) -> tuple[int, int, int]:
         """Generate a new EC key on this curve.
 
         Returns:
              a tuple of 4 `int`s: `x` and `y` coordinates (public key) and `d` (private key)
 
         """
         key = ec.generate_private_key(self.cryptography_curve)
@@ -51,51 +50,53 @@
         x = pn.public_numbers.x
         y = pn.public_numbers.y
         d = pn.private_value
         return x, y, d
 
     @classmethod
     def get_curve(
-        cls, key: Union[ec.EllipticCurvePublicKey, ec.EllipticCurvePrivateKey]
-    ) -> "EllipticCurve":
+        cls, key: ec.EllipticCurvePublicKey | ec.EllipticCurvePrivateKey
+    ) -> EllipticCurve:
         """Get the appropriate `EllipticCurve` instance for a given key.
 
         The provided key must be an `EllipticCurvePublicKey` or `EllipticCurvePrivateKey`
         from the `cryptography` module.
 
         Args:
           key: an Elliptic Curve private or public key from `cryptography`.
 
         Returns:
           the appropriate instance of EllipticCurve for the given key.
 
         Raises:
             NotImplementedError: if the curve is not supported
+
         """
         for c in cls.instances.values():
             if c.cryptography_curve.name == key.curve.name:
                 return c
         raise NotImplementedError(f"Unsupported Curve {key.curve.name}")
 
     @classmethod
     def get_jwk_parameters(
-        cls, key: Union[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]
-    ) -> Dict[str, Any]:
+        cls, key: ec.EllipticCurvePrivateKey | ec.EllipticCurvePublicKey
+    ) -> dict[str, Any]:
         """Extract all private and public parameters from the given `cryptography` key.
 
         Key must be an instance of `EllipticCurvePrivateKey` or `EllipticCurvePublicKey`.
 
         Args:
           key: an Elliptic Curve public or private key from `cryptography`.
 
         Returns:
           a dict of JWK parameters matching that key
 
         Raises:
             TypeError: if the provided key is not an EllipticCurvePrivateKey or EllipticCurvePublicKey
+
         """
         public_numbers: ec.EllipticCurvePublicNumbers
         if isinstance(key, ec.EllipticCurvePrivateKey):
             public_numbers = key.public_key().public_numbers()
         elif isinstance(key, ec.EllipticCurvePublicKey):
             public_numbers = key.public_numbers()
         else:
```

### Comparing `jwskate-0.8.0/jwskate/jwa/encryption/aescbchmac.py` & `jwskate-0.9.0/jwskate/jwa/encryption/aescbchmac.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements AES-CBC with HMAC-SHA based Encryption algorithms."""
+from __future__ import annotations
 
-from typing import SupportsBytes, Tuple, Union
+from typing import SupportsBytes
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import ciphers, constant_time, hashes, hmac, padding
 from cryptography.hazmat.primitives.ciphers import algorithms, modes
 
 from ..base import BaseAESEncryptionAlg, MismatchingAuthTag
 
@@ -34,28 +35,29 @@
         super().__init__(key)
         self.mac_key = self.key[: self.mac_key_size // 8]
         self.aes_key = self.key[self.mac_key_size // 8 :]
         self.padding = padding.PKCS7(algorithms.AES.block_size)
 
     def mac(
         self,
-        ciphertext: Union[bytes, SupportsBytes],
+        ciphertext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
+        iv: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
     ) -> BinaPy:
         """Produce a Message Authentication Code for the given `ciphertext`, `iv` and `aad`.
 
         Args:
           ciphertext: the ciphertext
           iv: the Initialization Vector
           aad: the Additional Authenticated data
 
         Returns:
           the resulting MAC.
+
         """
         if not isinstance(ciphertext, bytes):
             ciphertext = bytes(ciphertext)
         if not isinstance(iv, bytes):
             iv = bytes(iv)
         if aad is None:  # pragma: no branch
             aad = b""
@@ -69,31 +71,32 @@
             hasher.update(param)
         digest = hasher.finalize()
         mac = digest[: self.tag_size]
         return BinaPy(mac)
 
     def encrypt(
         self,
-        plaintext: Union[bytes, SupportsBytes],
+        plaintext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
-    ) -> Tuple[BinaPy, BinaPy]:
+        iv: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
+    ) -> tuple[BinaPy, BinaPy]:
         """Encrypt and MAC the given `plaintext`.
 
         This requires a given Initialization Vector (`iv`).
         An optional Additional Authenticated Data can be passed as parameter `aad`.
 
         Args:
           plaintext: the plain data to encrypt
           iv: the Initialization Vector
           aad: the Additional Authenticated Data, if any
 
         Returns:
           a tuple (encrypted_data, authentication_tag)
+
         """
         if not isinstance(plaintext, bytes):
             plaintext = bytes(plaintext)
         if not isinstance(iv, bytes):
             iv = bytes(iv)
         if aad is None:
             aad = b""
@@ -108,19 +111,19 @@
         padded_text = padder.update(plaintext) + padder.finalize()
         ciphertext = cipher.update(padded_text) + cipher.finalize()
         mac = self.mac(ciphertext, iv=iv, aad=aad)
         return BinaPy(ciphertext), BinaPy(mac)
 
     def decrypt(
         self,
-        ciphertext: Union[bytes, SupportsBytes],
+        ciphertext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        auth_tag: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
+        iv: bytes | SupportsBytes,
+        auth_tag: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
     ) -> BinaPy:
         """Decrypt and authenticate a given ciphertext.
 
          An optional Additional Authenticated Data must be authentication tag must be supplied, if the text was encryptwith authentication tag, as produced by `encrypt()`.
 
         Args:
           ciphertext: the ciphertext
```

### Comparing `jwskate-0.8.0/jwskate/jwa/encryption/aesgcm.py` & `jwskate-0.9.0/jwskate/jwa/encryption/aesgcm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements AES-GCM based encryption algorithms."""
+from __future__ import annotations
 
-from typing import SupportsBytes, Tuple, Union
+from typing import SupportsBytes
 
 import cryptography.exceptions
 from binapy import BinaPy
 from cryptography.hazmat.primitives.ciphers import aead
 
 from ..base import BaseAESEncryptionAlg, MismatchingAuthTag
 
@@ -13,19 +14,19 @@
     """Base class for AES-GCM encryption algorithms."""
 
     iv_size = 96
     tag_size = 16
 
     def encrypt(
         self,
-        plaintext: Union[bytes, SupportsBytes],
+        plaintext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
-    ) -> Tuple[BinaPy, BinaPy]:
+        iv: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
+    ) -> tuple[BinaPy, BinaPy]:
         """Encrypt a plaintext, with the given IV and Additional Authenticated Data.".
 
         Args:
           plaintext: the data to encrypt
           iv: the IV to use
           aad: Additional Authenticated Data, if any
 
@@ -48,19 +49,19 @@
             plaintext = bytes(plaintext)
         ciphertext_with_tag = BinaPy(aead.AESGCM(self.key).encrypt(iv, plaintext, aad))
         ciphertext, tag = ciphertext_with_tag.cut_at(-self.tag_size)
         return ciphertext, tag
 
     def decrypt(
         self,
-        ciphertext: Union[bytes, SupportsBytes],
+        ciphertext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        auth_tag: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
+        iv: bytes | SupportsBytes,
+        auth_tag: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
     ) -> BinaPy:
         """Decrypt a ciphertext.
 
         Args:
           ciphertext: the data to decrypt
           auth_tag: the Authentication Tag
           iv: the Initialization Vector
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/__init__.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module exposes all Key Management algorithms available in `jwskate`."""
+from __future__ import annotations
 
 from .aesgcmkw import A128GCMKW, A192GCMKW, A256GCMKW, BaseAesGcmKeyWrap
 from .aeskw import A128KW, A192KW, A256KW, BaseAesKeyWrap
 from .dir import DirectKeyUse
 from .ecdh import BaseEcdhEs_AesKw, EcdhEs, EcdhEs_A128KW, EcdhEs_A192KW, EcdhEs_A256KW
 from .pbes2 import BasePbes2, Pbes2_HS256_A128KW, Pbes2_HS384_A192KW, Pbes2_HS512_A256KW
 from .rsa import (
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/aesgcmkw.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/aesgcmkw.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements AES-GCM based Key Management algorithms."""
+from __future__ import annotations
 
-from typing import SupportsBytes, Tuple, Union
+from typing import SupportsBytes
 
 from binapy import BinaPy
 
 from ..base import BaseKeyManagementAlg
 from ..encryption.aesgcm import BaseAESGCM
 
 
@@ -17,16 +18,16 @@
     """Required key size, in bits."""
     tag_size: int = 16
     """Authentication tag size, in bits."""
     iv_size: int = 96
     """Initialisation Vector size, in bits."""
 
     def wrap_key(
-        self, plainkey: Union[bytes, SupportsBytes], *, iv: Union[bytes, SupportsBytes]
-    ) -> Tuple[BinaPy, BinaPy]:
+        self, plainkey: bytes | SupportsBytes, *, iv: bytes | SupportsBytes
+    ) -> tuple[BinaPy, BinaPy]:
         """Wrap a symmetric key, which is typically used as Content Encryption Key (CEK).
 
         This method is used by the sender of the encrypted message.
 
         This needs a random Initialisation Vector (`iv`) of the appropriate size,
         which you can generate using the classmethod `generate_iv()`.
 
@@ -38,18 +39,18 @@
           a tuple (wrapped_key, authentication_tag)
 
         """
         return self.encrypt(plainkey, iv=iv)
 
     def unwrap_key(
         self,
-        cipherkey: Union[bytes, SupportsBytes],
+        cipherkey: bytes | SupportsBytes,
         *,
-        tag: Union[bytes, SupportsBytes],
-        iv: Union[bytes, SupportsBytes]
+        tag: bytes | SupportsBytes,
+        iv: bytes | SupportsBytes,
     ) -> BinaPy:
         """Unwrap a symmetric key.
 
         This method is used by the recipient of an encrypted message.
 
         This requires:
         - the same IV that was provided during encryption
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/aeskw.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/aeskw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module implements AES based Key Management algorithms."""
-from typing import SupportsBytes, Union
+from __future__ import annotations
+
+from typing import SupportsBytes
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import keywrap
 from typing_extensions import Self, override
 
 from ..base import BaseKeyManagementAlg, BaseSymmetricAlg
 
@@ -44,15 +46,15 @@
 
         Returns:
           BinaPy: the wrapped key.
 
         """
         return BinaPy(keywrap.aes_key_wrap(self.key, plainkey))
 
-    def unwrap_key(self, cipherkey: Union[bytes, SupportsBytes]) -> BinaPy:
+    def unwrap_key(self, cipherkey: bytes | SupportsBytes) -> BinaPy:
         """Unwrap a key.
 
         Args:
           cipherkey: the wrapped key.
 
         Returns:
           BinaPy: the unwrapped key.
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/dir.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/dir.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """This module implements direct use of a shared symmetric key as Key Management algorithm."""
-
-from typing import Type
+from __future__ import annotations
 
 from binapy import BinaPy
 
 from ..base import BaseKeyManagementAlg, BaseSymmetricAlg
 
 
 class DirectKeyUse(BaseKeyManagementAlg, BaseSymmetricAlg):
     """Direct use of a shared symmetric key as the CEK."""
 
     name = "dir"
     description = __doc__
 
-    def direct_key(self, aesalg: Type[BaseSymmetricAlg]) -> BinaPy:
+    def direct_key(self, aesalg: type[BaseSymmetricAlg]) -> BinaPy:
         """Check that the current key is appropriate for a given alg and return that same key.
 
         Args:
           aesalg: the AES encryption alg to use
 
         Returns:
           the current configured key, as-is
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/ecdh.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/ecdh.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements Elliptic Curve Diffie-Hellman based Key Management algorithms."""
+from __future__ import annotations
 
-from typing import Any, SupportsBytes, Type, Union
+from typing import Any, SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ec, x448, x25519
 from cryptography.hazmat.primitives.kdf.concatkdf import ConcatKDFHash
 from typing_extensions import Self, override
 
@@ -59,20 +60,20 @@
         supppubinfo = BinaPy.from_int(key_size or key_size, length=4)
         otherinfo = b"".join((algorithm_id, partyuinfo, partyvinfo, supppubinfo))
         return BinaPy(otherinfo)
 
     @classmethod
     def ecdh(
         cls,
-        private_key: Union[
-            ec.EllipticCurvePrivateKey, x25519.X25519PrivateKey, x448.X448PrivateKey
-        ],
-        public_key: Union[
-            ec.EllipticCurvePublicKey, x25519.X25519PublicKey, x448.X448PublicKey
-        ],
+        private_key: (
+            ec.EllipticCurvePrivateKey | x25519.X25519PrivateKey | x448.X448PrivateKey
+        ),
+        public_key: (
+            ec.EllipticCurvePublicKey | x25519.X25519PublicKey | x448.X448PublicKey
+        ),
     ) -> BinaPy:
         """Perform an Elliptic Curve Diffie-Hellman key exchange.
 
         This derives a shared key between a sender and a receiver, based on a public and a private key from each side.
         ECDH exchange produces the same key with either a sender private key and a recipient public key,
         or the matching sender public key and recipient private key.
 
@@ -104,20 +105,20 @@
             )
         return BinaPy(shared_key)
 
     @classmethod
     def derive(
         cls,
         *,
-        private_key: Union[
-            ec.EllipticCurvePrivateKey, x25519.X25519PrivateKey, x448.X448PrivateKey
-        ],
-        public_key: Union[
-            ec.EllipticCurvePublicKey, x25519.X25519PublicKey, x448.X448PublicKey
-        ],
+        private_key: (
+            ec.EllipticCurvePrivateKey | x25519.X25519PrivateKey | x448.X448PrivateKey
+        ),
+        public_key: (
+            ec.EllipticCurvePublicKey | x25519.X25519PublicKey | x448.X448PublicKey
+        ),
         otherinfo: bytes,
         key_size: int,
     ) -> BinaPy:
         """Derive a key using ECDH and Concat KDF Hash.
 
         Args:
           private_key: the private key
@@ -133,17 +134,15 @@
         ckdf = ConcatKDFHash(
             algorithm=hashes.SHA256(), length=key_size // 8, otherinfo=otherinfo
         )
         return BinaPy(ckdf.derive(shared_key))
 
     def generate_ephemeral_key(
         self,
-    ) -> Union[
-        ec.EllipticCurvePrivateKey, x25519.X25519PrivateKey, x448.X448PrivateKey
-    ]:
+    ) -> ec.EllipticCurvePrivateKey | x25519.X25519PrivateKey | x448.X448PrivateKey:
         """Generate an ephemeral key that is suitable for use with this algorithm.
 
         Returns:
             a generated EllipticCurvePrivateKey, on the same curve as this algorithm key
 
         """
         if isinstance(
@@ -153,17 +152,17 @@
         elif isinstance(self.key, (x25519.X25519PrivateKey, x25519.X25519PublicKey)):
             return x25519.X25519PrivateKey.generate()
         elif isinstance(self.key, (x448.X448PublicKey, x448.X448PrivateKey)):
             return x448.X448PrivateKey.generate()
 
     def sender_key(
         self,
-        ephemeral_private_key: Union[
-            ec.EllipticCurvePrivateKey, x25519.X25519PrivateKey, x448.X448PrivateKey
-        ],
+        ephemeral_private_key: (
+            ec.EllipticCurvePrivateKey | x25519.X25519PrivateKey | x448.X448PrivateKey
+        ),
         *,
         alg: str,
         key_size: int,
         **headers: Any,
     ) -> BinaPy:
         """Compute a CEK for encryption of a message. This method is meant for usage by a sender.
 
@@ -187,17 +186,17 @@
                 otherinfo=otherinfo,
                 key_size=key_size,
             )
             return cek
 
     def recipient_key(
         self,
-        ephemeral_public_key: Union[
-            ec.EllipticCurvePublicKey, x25519.X25519PublicKey, x448.X448PublicKey
-        ],
+        ephemeral_public_key: (
+            ec.EllipticCurvePublicKey | x25519.X25519PublicKey | x448.X448PublicKey
+        ),
         *,
         alg: str,
         key_size: int,
         **headers: Any,
     ) -> BinaPy:
         """Compute a shared key, for use by the recipient of an encrypted message.
 
@@ -223,22 +222,22 @@
             )
             return cek
 
 
 class BaseEcdhEs_AesKw(EcdhEs):
     """Base class for ECDH-ES+AESKW algorithms."""
 
-    kwalg: Type[BaseAesKeyWrap]
+    kwalg: type[BaseAesKeyWrap]
 
     def wrap_key_with_epk(
         self,
         plainkey: bytes,
-        ephemeral_private_key: Union[
-            ec.EllipticCurvePrivateKey, x25519.X25519PrivateKey, x448.X448PrivateKey
-        ],
+        ephemeral_private_key: (
+            ec.EllipticCurvePrivateKey | x25519.X25519PrivateKey | x448.X448PrivateKey
+        ),
         **headers: Any,
     ) -> BinaPy:
         """Wrap a key for content encryption.
 
         Args:
           plainkey: the key to wrap
           ephemeral_private_key: the EPK to use
@@ -251,18 +250,18 @@
         aes_key = self.sender_key(
             ephemeral_private_key, key_size=self.kwalg.key_size, **headers
         )
         return self.kwalg(aes_key).wrap_key(plainkey)
 
     def unwrap_key_with_epk(
         self,
-        cipherkey: Union[bytes, SupportsBytes],
-        ephemeral_public_key: Union[
-            ec.EllipticCurvePublicKey, x25519.X25519PublicKey, x448.X448PublicKey
-        ],
+        cipherkey: bytes | SupportsBytes,
+        ephemeral_public_key: (
+            ec.EllipticCurvePublicKey | x25519.X25519PublicKey | x448.X448PublicKey
+        ),
         **headers: Any,
     ) -> BinaPy:
         """Unwrap a key for content decryption.
 
         Args:
           cipherkey: the wrapped key
           ephemeral_public_key: the EPK
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/pbes2.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/pbes2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements password-based Key Management Algorithms relying on PBES2."""
+from __future__ import annotations
 
-from typing import SupportsBytes, Type, Union
+from typing import SupportsBytes
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf import pbkdf2
 
 from ..base import BaseKeyManagementAlg
 from .aeskw import A128KW, A192KW, A256KW, BaseAesKeyWrap
@@ -16,18 +17,18 @@
     PBES2 derives a cryptographic key from a human-provided password.
 
     Args:
         password: the encryption/decryption password to use
 
     """
 
-    kwalg: Type[BaseAesKeyWrap]
+    kwalg: type[BaseAesKeyWrap]
     hash_alg: hashes.HashAlgorithm
 
-    def __init__(self, password: Union[SupportsBytes, bytes, str]):
+    def __init__(self, password: SupportsBytes | bytes | str):
         if isinstance(password, str):
             password = password.encode("utf-8")
         if not isinstance(password, bytes):
             password = bytes(password)
         self.password = password
 
     @classmethod
```

### Comparing `jwskate-0.8.0/jwskate/jwa/key_mgmt/rsa.py` & `jwskate-0.9.0/jwskate/jwa/key_mgmt/rsa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements RSA based Key Management algorithms."""
+from __future__ import annotations
 
-from typing import Any, SupportsBytes, Union
+from typing import Any, SupportsBytes
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from typing_extensions import Self, override
 
 from ..base import BaseAsymmetricAlg, BaseKeyManagementAlg
@@ -49,15 +50,15 @@
         if self.read_only:
             raise NotImplementedError(
                 "Due to security reasons, this algorithm is only usable for decryption."
             )
         with self.public_key_required() as key:
             return BinaPy(key.encrypt(plainkey, self.padding))
 
-    def unwrap_key(self, cipherkey: Union[bytes, SupportsBytes]) -> BinaPy:
+    def unwrap_key(self, cipherkey: bytes | SupportsBytes) -> BinaPy:
         """Unwrap a symmetric key with this alg.
 
         Args:
           cipherkey: the wrapped key
 
         Returns:
             the unwrapped clear-text key
```

### Comparing `jwskate-0.8.0/jwskate/jwa/okp.py` & `jwskate-0.9.0/jwskate/jwa/okp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """This module implements CFRG Elliptic Curve Diffie-Hellman algorithms as specified in [RFC8037].
 
 [RFC8037]
 : https: //www.rfc-editor.org/rfc/rfc8037.html
 
 """
-
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Any, ClassVar, Dict, Tuple, Type, Union
+from typing import Any, ClassVar, runtime_checkable
 
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519, x448, x25519
-from typing_extensions import Protocol, runtime_checkable
+from typing_extensions import Protocol
 
 
 @runtime_checkable
 class PublicKeyProtocol(Protocol):
     """A protocol that each `cryptography` ECDH public key class implements."""
 
     def public_bytes(
@@ -57,31 +56,31 @@
 
     This name will appear in `crv` headers.
     """
 
     description: str
     """Curve description (human readable)."""
 
-    cryptography_private_key_class: Type[Any]
+    cryptography_private_key_class: type[Any]
     """`cryptography` private key class."""
 
-    cryptography_public_key_class: Type[Any]
+    cryptography_public_key_class: type[Any]
     """`cryptography` public key class."""
 
     use: str
     """Curve usage (`'sig'` or '`enc'`)."""
 
-    instances: ClassVar[Dict[str, OKPCurve]] = {}
+    instances: ClassVar[dict[str, OKPCurve]] = {}
     """Registry of subclasses, in a {name: instance} mapping."""
 
     def __post_init__(self) -> None:
         """Automatically registers subclasses in the instance registry."""
         self.instances[self.name] = self
 
-    def generate(self) -> Tuple[bytes, bytes]:
+    def generate(self) -> tuple[bytes, bytes]:
         """Generate a new private key on this curve.
 
         Returns:
             a tuple of `x` (public  part), and `d` (private part), as bytes
 
         """
         key = self.cryptography_private_key_class.generate()
@@ -92,27 +91,28 @@
             serialization.Encoding.Raw,
             serialization.PrivateFormat.Raw,
             serialization.NoEncryption(),
         )
         return x, d
 
     @classmethod
-    def get_curve(cls, key: Union[PublicKeyProtocol, PrivateKeyProtocol]) -> OKPCurve:
+    def get_curve(cls, key: PublicKeyProtocol | PrivateKeyProtocol) -> OKPCurve:
         """Return the appropriate `OKPCurve` instance for a given key.
 
         This takes a `cryptography` private or public key as parameter. If the key type matches an OKP curve
 
         Args:
           key: `cryptography` private or public OKP key.
 
         Returns:
           OKPCurve: the appropriate `OKPCurve` for the given key
 
         Raises:
             NotImplementedError: if the required OKP curve is not supported
+
         """
         for c in cls.instances.values():
             if isinstance(
                 key, (c.cryptography_private_key_class, c.cryptography_public_key_class)
             ):
                 return c
         raise TypeError(
```

### Comparing `jwskate-0.8.0/jwskate/jwa/signature/__init__.py` & `jwskate-0.9.0/jwskate/jwa/signature/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module exposes all the Signature algorithms available from `jwskate`."""
+from __future__ import annotations
 
 from .ec import ES256, ES256K, ES384, ES512, BaseECSignatureAlg
 from .eddsa import Ed448Dsa, Ed25519Dsa, EdDsa
 from .hmac import HS256, HS384, HS512, BaseHMACSigAlg
 from .rsa import PS256, PS384, PS512, RS256, RS384, RS512, BaseRSASigAlg
 
 __all__ = [
```

### Comparing `jwskate-0.8.0/jwskate/jwa/signature/ec.py` & `jwskate-0.9.0/jwskate/jwa/signature/ec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module implement Elliptic Curve signature algorithms."""
-from typing import SupportsBytes, Union
+from __future__ import annotations
+
+from typing import SupportsBytes
 
 from binapy import BinaPy
 from cryptography import exceptions
 from cryptography.hazmat.primitives import asymmetric, hashes
 from cryptography.hazmat.primitives.asymmetric import ec
 from typing_extensions import Self, override
 
@@ -19,39 +21,39 @@
 
     curve: EllipticCurve
     public_key_class = ec.EllipticCurvePublicKey
     private_key_class = ec.EllipticCurvePrivateKey
 
     @classmethod
     def check_key(
-        cls, key: Union[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey]
+        cls, key: ec.EllipticCurvePrivateKey | ec.EllipticCurvePublicKey
     ) -> None:  # noqa: D102
         if key.curve.name != cls.curve.cryptography_curve.name:
             raise ValueError(
                 f"This key is on curve {key.curve.name}. An EC key on curve {cls.curve.name} is expected."
             )
 
     @classmethod
     @override
     def with_random_key(cls) -> Self:
         return cls(ec.generate_private_key(cls.curve.cryptography_curve))
 
-    def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:  # noqa: D102
+    def sign(self, data: bytes | SupportsBytes) -> BinaPy:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         with self.private_key_required() as key:
             dss_sig = key.sign(data, ec.ECDSA(self.hashing_alg))
             r, s = asymmetric.utils.decode_dss_signature(dss_sig)
             return BinaPy.from_int(r, self.curve.coordinate_size) + BinaPy.from_int(
                 s, self.curve.coordinate_size
             )
 
     def verify(
-        self, data: Union[bytes, SupportsBytes], signature: Union[bytes, SupportsBytes]
+        self, data: bytes | SupportsBytes, signature: bytes | SupportsBytes
     ) -> bool:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         if not isinstance(signature, bytes):
             signature = bytes(signature)
```

### Comparing `jwskate-0.8.0/jwskate/jwa/signature/eddsa.py` & `jwskate-0.9.0/jwskate/jwa/signature/eddsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module implements the Edwards-curve Digital Signature Algorithm (EdDSA)."""
+from __future__ import annotations
 
 from typing import SupportsBytes, Union
 
 from binapy import BinaPy
 from cryptography import exceptions
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519
@@ -27,23 +28,23 @@
     description = __doc__
 
     @classmethod
     @override
     def with_random_key(cls) -> Self:
         return cls(ed25519.Ed25519PrivateKey.generate())
 
-    def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:  # noqa: D102
+    def sign(self, data: bytes | SupportsBytes) -> BinaPy:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         with self.private_key_required() as key:
             return BinaPy(key.sign(data))
 
     def verify(
-        self, data: Union[bytes, SupportsBytes], signature: Union[bytes, SupportsBytes]
+        self, data: bytes | SupportsBytes, signature: bytes | SupportsBytes
     ) -> bool:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
         if not isinstance(signature, bytes):
             signature = bytes(signature)
 
         with self.public_key_required() as key:
```

### Comparing `jwskate-0.8.0/jwskate/jwa/signature/hmac.py` & `jwskate-0.9.0/jwskate/jwa/signature/hmac.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 """This module implements HMAC based signature algorithms."""
+from __future__ import annotations
 
-from typing import SupportsBytes, Type, Union
+from typing import SupportsBytes
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes, hmac
 from typing_extensions import Self, override
 
 from ..base import BaseSignatureAlg, BaseSymmetricAlg
 
 
 class BaseHMACSigAlg(BaseSymmetricAlg, BaseSignatureAlg):
     """Base class for HMAC signature algorithms."""
 
-    mac: Type[hmac.HMAC] = hmac.HMAC
+    mac: type[hmac.HMAC] = hmac.HMAC
     min_key_size: int
 
     @classmethod
     @override
     def with_random_key(cls) -> Self:
         return cls(BinaPy.random_bits(cls.min_key_size))
 
-    def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:  # noqa: D102
+    def sign(self, data: bytes | SupportsBytes) -> BinaPy:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         if self.read_only:
             raise NotImplementedError
         m = self.mac(self.key, self.hashing_alg)
         m.update(data)
         signature = m.finalize()
         return BinaPy(signature)
 
     def verify(
-        self, data: Union[bytes, SupportsBytes], signature: Union[bytes, SupportsBytes]
+        self, data: bytes | SupportsBytes, signature: bytes | SupportsBytes
     ) -> bool:  # noqa: D102
         if not isinstance(data, bytes):
             data = bytes(data)
 
         if not isinstance(signature, bytes):
             signature = bytes(signature)
```

### Comparing `jwskate-0.8.0/jwskate/jwa/signature/rsa.py` & `jwskate-0.9.0/jwskate/jwa/signature/rsa.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module implements RSA signature algorithms."""
-from typing import SupportsBytes, Union
+from __future__ import annotations
+
+from typing import SupportsBytes
 
 from binapy import BinaPy
 from cryptography import exceptions
 from cryptography.hazmat.primitives import asymmetric, hashes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa
 from typing_extensions import Self, override
 
@@ -25,15 +27,15 @@
     @classmethod
     @override
     def with_random_key(cls) -> Self:
         return cls(
             rsa.generate_private_key(public_exponent=65537, key_size=cls.min_key_size)
         )
 
-    def sign(self, data: Union[bytes, SupportsBytes]) -> BinaPy:
+    def sign(self, data: bytes | SupportsBytes) -> BinaPy:
         """Sign arbitrary data.
 
         Args:
           data: the data to sign
 
         Returns:
             the generated signature
@@ -49,15 +51,15 @@
         if not isinstance(data, bytes):
             data = bytes(data)
 
         with self.private_key_required() as key:
             return BinaPy(key.sign(data, self.padding_alg, self.hashing_alg))
 
     def verify(
-        self, data: Union[bytes, SupportsBytes], signature: Union[bytes, SupportsBytes]
+        self, data: bytes | SupportsBytes, signature: bytes | SupportsBytes
     ) -> bool:
         """Verify a signature against some data.
 
         Args:
           data: the data to verify
           signature: the signature
```

### Comparing `jwskate-0.8.0/jwskate/jwe/compact.py` & `jwskate-0.9.0/jwskate/jwe/compact.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """This module implements the JWE Compact format."""
-
 from __future__ import annotations
 
 import warnings
 from functools import cached_property
-from typing import Any, Dict, Iterable, Mapping, Optional, SupportsBytes, Type, Union
+from typing import Any, Iterable, Mapping, SupportsBytes
 
 from binapy import BinaPy
 
 from jwskate.jwa import (
     BasePbes2,
     Pbes2_HS256_A128KW,
     Pbes2_HS384_A192KW,
@@ -27,15 +26,15 @@
     """Represents a Json Web Encryption object, in compact representation, as defined in RFC7516.
 
     Args:
         value: the compact representation for this Jwe
 
     """
 
-    def __init__(self, value: Union[bytes, str], max_size: int = 16 * 1024):
+    def __init__(self, value: bytes | str, max_size: int = 16 * 1024):
         super().__init__(value, max_size)
 
         if self.value.count(b".") != 4:
             raise InvalidJwe(
                 "Invalid JWE: a JWE must contain a header, an encrypted key, an IV, a ciphertext and an authentication tag, separated by dots."
             )
 
@@ -99,14 +98,15 @@
           cek: the raw CEK
           iv: the raw IV
           ciphertext: the raw ciphertext
           tag: the authentication tag
 
         Returns:
             the initialized `JweCompact` instance
+
         """
         return cls(
             b".".join(
                 (
                     BinaPy.serialize_to("json", headers).to("b64u"),
                     BinaPy(cek).to("b64u"),
                     BinaPy(iv).to("b64u"),
@@ -123,30 +123,31 @@
         The `enc` header contains the identifier of the CEK encryption algorithm.
 
         Returns:
             the enc value
 
         Raises:
             AttributeError: if there is no enc header or it is not a string
+
         """
         return self.get_header("enc")  # type: ignore[no-any-return]
         # header has been checked at init time
 
     @classmethod
     def encrypt(
         cls,
-        plaintext: Union[bytes, SupportsBytes],
-        key: Union[Jwk, Dict[str, Any], Any],
+        plaintext: bytes | SupportsBytes,
+        key: Jwk | dict[str, Any] | Any,
         *,
         enc: str,
-        alg: Optional[str] = None,
-        extra_headers: Optional[Dict[str, Any]] = None,
-        cek: Optional[bytes] = None,
-        iv: Optional[bytes] = None,
-        epk: Optional[Jwk] = None,
+        alg: str | None = None,
+        extra_headers: dict[str, Any] | None = None,
+        cek: bytes | None = None,
+        iv: bytes | None = None,
+        epk: Jwk | None = None,
     ) -> JweCompact:
         """Encrypt an arbitrary plaintext into a `JweCompact`.
 
         Args:
           plaintext: the raw plaintext to encrypt
           key: the public or symmetric key to use for encryption
           enc: the encryption algorithm to use
@@ -154,14 +155,15 @@
           extra_headers: additional headers to include in the generated token
           cek: the CEK to force use, for algorithms relying on a random CEK. Leave `None` to have a safe value generated by `jwskate`.
           iv: the IV to force use. Leave `None` to have a safe value generated by `jwskate`.
           epk: the EPK to force use. Leave `None` to have a safe value generated by `jwskate`.
 
         Returns:
             the generated JweCompact instance
+
         """
         extra_headers = extra_headers or {}
         key = to_jwk(key)
         alg = select_alg_class(
             key.KEY_MANAGEMENT_ALGORITHMS, jwk_alg=key.alg, alg=alg
         ).name
 
@@ -177,34 +179,35 @@
 
         ciphertext, iv, tag = cek_jwk.encrypt(plaintext, aad=aad, iv=iv, alg=enc)
 
         return cls.from_parts(
             headers=headers, cek=wrapped_cek, iv=iv, ciphertext=ciphertext, tag=tag
         )
 
-    PBES2_ALGORITHMS: Mapping[str, Type[BasePbes2]] = {
+    PBES2_ALGORITHMS: Mapping[str, type[BasePbes2]] = {
         alg.name: alg
         for alg in [Pbes2_HS256_A128KW, Pbes2_HS384_A192KW, Pbes2_HS512_A256KW]
     }
 
     def unwrap_cek(
         self,
-        key_or_password: Union[Jwk, Dict[str, Any], bytes, str],
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        key_or_password: Jwk | dict[str, Any] | bytes | str,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> Jwk:
         """Unwrap the CEK from this `Jwe` using the provided key or password.
 
         Args:
           key_or_password: the decryption JWK or password
           alg: allowed key management algorithm, if there is only 1
           algs: allowed key managements algorithms, if there are several
 
         Returns:
             the unwrapped CEK, as a SymmetricJwk
+
         """
         if isinstance(key_or_password, (bytes, str)):
             password = key_or_password
             return self.unwrap_cek_with_password(password)
 
         jwk = to_jwk(key_or_password)
         select_alg_classes(
@@ -215,27 +218,28 @@
             strict=True,
         )
         cek = jwk.recipient_key(self.wrapped_cek, **self.headers)
         return cek
 
     def decrypt(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> BinaPy:
         """Decrypts this `Jwe` payload using a `Jwk`.
 
         Args:
           key: the decryption key
           alg: allowed key management algorithm, if there is only 1
           algs: allowed keys management algorithms, if there are several
 
         Returns:
           the decrypted payload
+
         """
         cek_jwk = self.unwrap_cek(key, alg=alg, algs=algs)
 
         plaintext = cek_jwk.decrypt(
             ciphertext=self.ciphertext,
             iv=self.initialization_vector,
             tag=self.authentication_tag,
@@ -243,24 +247,24 @@
             alg=self.enc,
         )
         return plaintext
 
     @classmethod
     def encrypt_with_password(
         cls,
-        plaintext: Union[SupportsBytes, bytes],
-        password: Union[SupportsBytes, bytes, str],
+        plaintext: SupportsBytes | bytes,
+        password: SupportsBytes | bytes | str,
         *,
         alg: str,
         enc: str,
-        salt: Optional[bytes] = None,
+        salt: bytes | None = None,
         count: int = 2000,
-        cek: Optional[bytes] = None,
-        iv: Optional[bytes] = None,
-    ) -> "JweCompact":
+        cek: bytes | None = None,
+        iv: bytes | None = None,
+    ) -> JweCompact:
         """Encrypt a payload with a password and return the resulting JweCompact.
 
         This performs symmetric encryption using PBES2.
 
         Args:
           plaintext: the data to encrypt
           password: the password to use
@@ -311,15 +315,15 @@
             plaintext=plaintext, aad=aad, alg=enc, iv=iv
         )
 
         return cls.from_parts(
             headers=headers, cek=wrapped_cek, iv=iv, ciphertext=ciphertext, tag=tag
         )
 
-    def unwrap_cek_with_password(self, password: Union[bytes, str]) -> Jwk:
+    def unwrap_cek_with_password(self, password: bytes | str) -> Jwk:
         """Unwrap a CEK using a password. Works only for password-encrypted JWE Tokens.
 
         Args:
           password: the decryption password
 
         Returns:
             the CEK, as a SymmetricJwk instance
@@ -346,15 +350,15 @@
             raise InvalidJwe(
                 "Invalid JWE: invalid value for the 'p2c' header, must be a positive integer."
             )
         wrapper = keyalg(password)
         cek = wrapper.unwrap_key(self.wrapped_cek, salt=salt, count=p2c)
         return SymmetricJwk.from_bytes(cek)
 
-    def decrypt_with_password(self, password: Union[bytes, str]) -> bytes:
+    def decrypt_with_password(self, password: bytes | str) -> bytes:
         """Decrypt this JWE with a password.
 
         This only works for tokens encrypted with a password.
 
         Args:
           password: the password to use
```

### Comparing `jwskate-0.8.0/jwskate/jwk/__init__.py` & `jwskate-0.9.0/jwskate/jwk/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module implements [Json Web Key RFC7517](https://tools.ietf.org/html/rfc7517)."""
+from __future__ import annotations
 
 from .alg import (
     ExpectedAlgRequired,
     MismatchingAlg,
     UnsupportedAlg,
     select_alg_class,
     select_alg_classes,
```

### Comparing `jwskate-0.8.0/jwskate/jwk/alg.py` & `jwskate-0.9.0/jwskate/jwk/alg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module contains several utilities for algorithmic agility."""
+from __future__ import annotations
 
 import warnings
-from typing import Iterable, List, Mapping, Optional, Type, TypeVar, Union
+from typing import Iterable, Mapping, Type, TypeVar
 
 from jwskate.jwa import BaseAlg
 
 
 class UnsupportedAlg(ValueError):
     """Raised when a unsupported alg is requested."""
 
@@ -21,30 +22,30 @@
     algorithm specified in the key or the token.
 
     """
 
     def __init__(
         self,
         target_alg: str,
-        alg: Optional[str] = None,
-        algs: Union[Iterable[str], None] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> None:
         self.target_alg = target_alg
         self.alg = alg
         self.algs = list(algs) if algs else None
 
 
 T = TypeVar("T", bound=Type[BaseAlg])
 
 
 def select_alg_class(
     supported_algs: Mapping[str, T],
     *,
-    jwk_alg: Optional[str] = None,
-    alg: Optional[str] = None,
+    jwk_alg: str | None = None,
+    alg: str | None = None,
     strict: bool = False,
 ) -> T:
     """Choose the appropriate alg class to use for cryptographic operations.
 
     Given:
     - a mapping of supported algs names to wrapper classes
     - a preferred alg name (usually the one mentioned in a JWK)
@@ -100,19 +101,19 @@
             f"Alg {choosen_alg} is not supported. Supported algs: {list(supported_algs)}."
         )
 
 
 def select_alg_classes(
     supported_algs: Mapping[str, T],
     *,
-    jwk_alg: Optional[str] = None,
-    alg: Optional[str] = None,
-    algs: Optional[Iterable[str]] = None,
+    jwk_alg: str | None = None,
+    alg: str | None = None,
+    algs: Iterable[str] | None = None,
     strict: bool = False,
-) -> List[T]:
+) -> list[T]:
     """Select several appropriate algs classes to use on cryptographic operations.
 
     This method is typically used to get the list of valid algorithms when checking a signature, when several algorithms are allowed.
 
     Given:
     - a mapping of supported algorithms name to wrapper classes
     - an alg parameter from a JWK
@@ -151,15 +152,15 @@
             else:
                 requested_alg = f"{alg=}" if alg else f"{algs=}"
                 warnings.warn(
                     f"This key has an 'alg' parameter with value {jwk_alg}, so you should use it with that alg only."
                     f"You requested {requested_alg}."
                 )
 
-    possible_algs: List[str] = []
+    possible_algs: list[str] = []
     if alg:
         possible_algs = [alg]
     elif algs:
         possible_algs = list(algs)
     elif jwk_alg:
         possible_algs = [jwk_alg]
```

### Comparing `jwskate-0.8.0/jwskate/jwk/base.py` & `jwskate-0.9.0/jwskate/jwk/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,21 @@
 
 `Jwk` provides the main interface for using or interacting with JWK keys.
 
 Subclasses of `Jwk` will implement the specific key types, like RSA, EC, OKP, and will provide an
 interface to access the specific attributes for each key type. Unless you are dealing with a
 specific key type and want to access the internal attributes, you should only ever need to use the
 interface from `Jwk`.
-"""
 
+"""
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    ClassVar,
-    Dict,
-    Iterable,
-    List,
-    Mapping,
-    Optional,
-    SupportsBytes,
-    Tuple,
-    Type,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, ClassVar, Iterable, Mapping, SupportsBytes
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import serialization
 
 from jwskate.jwa import (
     BaseAESEncryptionAlg,
     BaseAesGcmKeyWrap,
@@ -96,14 +83,15 @@
 
         Args:
             alg: a signature or key management algorithm identifier
             **kwargs: specific parameters, depending on the key type, or additional members to include in the `Jwk`
 
         Returns:
             the generated `Jwk`
+
         """
         for kty, jwk_class in cls.subclasses.items():
             try:
                 jwk_class._get_alg_class(alg)
                 return jwk_class.generate(alg=alg, **kwargs)
             except UnsupportedAlg:
                 continue
@@ -126,29 +114,29 @@
 
         """
         jwk_class = cls.subclasses.get(kty)
         if jwk_class is None:
             raise UnsupportedKeyType("Unsupported Key Type:", kty)
         return jwk_class.generate(**kwargs)
 
-    subclasses: Dict[str, Type[Jwk]] = {}
+    subclasses: dict[str, type[Jwk]] = {}
     """A dict of 'kty' values to `Jwk` subclasses implementing each specific Key Type."""
-    cryptography_key_types: Dict[Any, Type[Jwk]] = {}
+    cryptography_key_types: dict[Any, type[Jwk]] = {}
     """A dict of cryptography classes to equivalent `Jwk` subclasses."""
 
     PARAMS: Mapping[str, JwkParameter]
 
     KTY: ClassVar[str]
 
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES: ClassVar[Iterable[Any]]
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES: ClassVar[Iterable[Any]]
 
-    SIGNATURE_ALGORITHMS: Mapping[str, Type[BaseSignatureAlg]] = {}
-    KEY_MANAGEMENT_ALGORITHMS: Mapping[str, Type[BaseKeyManagementAlg]] = {}
-    ENCRYPTION_ALGORITHMS: Mapping[str, Type[BaseAESEncryptionAlg]] = {}
+    SIGNATURE_ALGORITHMS: Mapping[str, type[BaseSignatureAlg]] = {}
+    KEY_MANAGEMENT_ALGORITHMS: Mapping[str, type[BaseKeyManagementAlg]] = {}
+    ENCRYPTION_ALGORITHMS: Mapping[str, type[BaseAESEncryptionAlg]] = {}
 
     IANA_HASH_FUNCTION_NAMES: Mapping[str, str] = {
         # IANA registered names to binapy hash name
         "sha-1": "sha1",
         "sha-224": "sha224",
         "sha-256": "sha256",
         "sha-384": "sha384",
@@ -165,47 +153,48 @@
         """
         Jwk.subclasses[cls.KTY] = cls
         for klass in cls.CRYPTOGRAPHY_PRIVATE_KEY_CLASSES:
             Jwk.cryptography_key_types[klass] = cls
         for klass in cls.CRYPTOGRAPHY_PUBLIC_KEY_CLASSES:
             Jwk.cryptography_key_types[klass] = cls
 
-    def __new__(cls, key: Union[Jwk, Dict[str, Any], Any], **kwargs: Any) -> Jwk:
+    def __new__(cls, key: Jwk | dict[str, Any] | Any, **kwargs: Any) -> Jwk:
         """Overridden `__new__` to make the Jwk constructor smarter.
 
         The Jwk constructor will accept:
 
             - a `dict` with the parsed Jwk content
             - another Jwk, which will be used as-is instead of creating a copy
             - an instance from a `cryptography` public or private key class
 
         Args:
             key: a dict containing JWK parameters, or another Jwk instance, or a `cryptography` key
             **kwargs: additional members to include in the Jwk
+
         """
         if cls == Jwk:
             if isinstance(key, Jwk):
                 return cls.from_cryptography_key(key.cryptography_key, **kwargs)
             if isinstance(key, dict):
-                kty: Optional[str] = key.get("kty")
+                kty: str | None = key.get("kty")
                 if kty is None:
                     raise InvalidJwk("A Json Web Key must have a Key Type (kty)")
 
                 subclass = Jwk.subclasses.get(kty)
                 if subclass is None:
                     raise InvalidJwk("Unsupported Key Type", kty)
                 return super().__new__(subclass)  # type: ignore[type-var]
             elif isinstance(key, str):
                 return cls.from_json(key)
             else:
                 return cls.from_cryptography_key(key, **kwargs)
         return super().__new__(cls, key, **kwargs)  # type: ignore[type-var]
 
     def __init__(
-        self, params: Union[Dict[str, Any], Any], include_kid_thumbprint: bool = False
+        self, params: dict[str, Any] | Any, include_kid_thumbprint: bool = False
     ):
         if isinstance(
             params, dict
         ):  # this is to avoid double init due to the __new__ above
             super().__init__(
                 {key: val for key, val in params.items() if val is not None}
             )
@@ -215,25 +204,25 @@
 
         try:
             self.cryptography_key = self._to_cryptography_key()
         except Exception as exc:
             raise InvalidJwk(params) from exc
 
     @classmethod
-    def _get_alg_class(cls, alg: str) -> Type[BaseAlg]:
+    def _get_alg_class(cls, alg: str) -> type[BaseAlg]:
         """Given an alg identifier, return the matching JWA wrapper.
 
         Args:
             alg: an alg identifier
 
         Returns:
             the matching JWA wrapper
 
         """
-        alg_class: Optional[Type[BaseAlg]]
+        alg_class: type[BaseAlg] | None
 
         alg_class = cls.SIGNATURE_ALGORITHMS.get(alg)
         if alg_class is not None:
             return alg_class
 
         alg_class = cls.KEY_MANAGEMENT_ALGORITHMS.get(alg)
         if alg_class is not None:
@@ -247,14 +236,15 @@
 
     @property
     def is_private(self) -> bool:
         """Return `True` if the key is private, `False` otherwise.
 
         Returns:
             `True` if the key is private, `False` otherwise
+
         """
         return True
 
     @property
     def is_symmetric(self) -> bool:
         """Return `True` if the key is symmetric, `False` otherwise."""
         return False
@@ -301,58 +291,58 @@
         Returns:
             the key type
 
         """
         return self.KTY
 
     @property
-    def alg(self) -> Optional[str]:
+    def alg(self) -> str | None:
         """Return the configured key alg, if any.
 
         Returns:
             the key alg
 
         """
         alg = self.get("alg")
         if alg is not None and not isinstance(alg, str):  # pragma: no branch
             raise TypeError(f"Invalid alg type {type(alg)}", alg)
         return alg
 
     @property
-    def kid(self) -> Optional[str]:
+    def kid(self) -> str | None:
         """Return the JWK key ID (kid), if present."""
         kid = self.get("kid")
         if kid is not None and not isinstance(kid, str):  # pragma: no branch
             raise TypeError(f"invalid kid type {type(kid)}", kid)
         return kid
 
     @property
-    def use(self) -> Optional[str]:
+    def use(self) -> str | None:
         """Return the key use.
 
         If no `alg` parameter is present, this returns the `use` parameter from this JWK. If an
         `alg` parameter is present, the use is deduced from this alg. To check for the presence of
         the `use` parameter, use `jwk.get('use')`.
 
         """
         if self.alg:
             return self._get_alg_class(self.alg).use
         else:
             return self.get("use")
 
     @property
-    def key_ops(self) -> Tuple[str, ...]:
+    def key_ops(self) -> tuple[str, ...]:
         """Return the key operations.
 
         If no `alg` parameter is present, this returns the `key_ops` parameter from this JWK. If an
         `alg` parameter is present, the key operations are deduced from this alg. To check for the
         presence of the `key_ops` parameter, use `jwk.get('key_ops')`.
 
         """
-        key_ops: Tuple[str, ...]
+        key_ops: tuple[str, ...]
         if self.use == "sig":
             if self.is_symmetric:
                 key_ops = ("sign", "verify")
             elif self.is_private:
                 key_ops = ("sign",)
             else:
                 key_ops = ("verify",)
@@ -414,17 +404,17 @@
         return (
             f"urn:ietf:params:oauth:jwk-thumbprint:{hashalg}:{self.thumbprint(hashalg)}"
         )
 
     def check(
         self,
         *,
-        is_private: Optional[bool] = None,
-        is_symmetric: Optional[bool] = None,
-        kty: Optional[str] = None,
+        is_private: bool | None = None,
+        is_symmetric: bool | None = None,
+        kty: str | None = None,
     ) -> Jwk:
         """Check this key for type, privateness and/or symmetricness.
 
         This raises a `ValueError` if the key is not as expected.
 
         Args:
             is_private: if `True`, check if the key is private, if `False`, check if it is public, if `None`, do nothing
@@ -520,15 +510,15 @@
                     )
 
         # if key is used for signing, it must be private
         for op in self.get("key_ops", []):
             if op in ("sign", "unwrapKey") and not self.is_private:
                 raise InvalidJwk(f"Key Operation is '{op}' but the key is public")
 
-    def signature_class(self, alg: Optional[str] = None) -> Type[BaseSignatureAlg]:
+    def signature_class(self, alg: str | None = None) -> type[BaseSignatureAlg]:
         """Return the appropriate signature algorithm class to use with this key.
 
         The returned class is a `BaseSignatureAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
@@ -536,15 +526,15 @@
 
         Returns:
             the appropriate `BaseSignatureAlg` subclass
 
         """
         return select_alg_class(self.SIGNATURE_ALGORITHMS, jwk_alg=self.alg, alg=alg)
 
-    def encryption_class(self, alg: Optional[str] = None) -> Type[BaseAESEncryptionAlg]:
+    def encryption_class(self, alg: str | None = None) -> type[BaseAESEncryptionAlg]:
         """Return the appropriate encryption algorithm class to use with this key.
 
         The returned class is a subclass of `BaseAESEncryptionAlg`.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
@@ -553,16 +543,16 @@
         Returns:
             the appropriate `BaseAESEncryptionAlg` subclass
 
         """
         return select_alg_class(self.ENCRYPTION_ALGORITHMS, jwk_alg=self.alg, alg=alg)
 
     def key_management_class(
-        self, alg: Optional[str] = None
-    ) -> Type[BaseKeyManagementAlg]:
+        self, alg: str | None = None
+    ) -> type[BaseKeyManagementAlg]:
         """Return the appropriate key management algorithm class to use with this key.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
             alg: the algorithm identifier, if not already present in this Jwk
 
@@ -570,15 +560,15 @@
             the appropriate `BaseKeyManagementAlg` subclass
 
         """
         return select_alg_class(
             self.KEY_MANAGEMENT_ALGORITHMS, jwk_alg=self.alg, alg=alg
         )
 
-    def signature_wrapper(self, alg: Optional[str] = None) -> BaseSignatureAlg:
+    def signature_wrapper(self, alg: str | None = None) -> BaseSignatureAlg:
         """Initialize a  key management wrapper with this key.
 
         This returns an instance of a `BaseSignatureAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
@@ -591,15 +581,15 @@
         alg_class = self.signature_class(alg)
         if issubclass(alg_class, BaseSymmetricAlg):
             return alg_class(self.key)
         elif issubclass(alg_class, BaseAsymmetricAlg):
             return alg_class(self.cryptography_key)
         raise UnsupportedAlg(alg)  # pragma: no cover
 
-    def encryption_wrapper(self, alg: Optional[str] = None) -> BaseAESEncryptionAlg:
+    def encryption_wrapper(self, alg: str | None = None) -> BaseAESEncryptionAlg:
         """Initialize an encryption wrapper with this key.
 
         This returns an instance of a `BaseAESEncryptionAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
@@ -612,15 +602,15 @@
         alg_class = self.encryption_class(alg)
         if issubclass(alg_class, BaseSymmetricAlg):
             return alg_class(self.key)
         elif issubclass(alg_class, BaseAsymmetricAlg):  # pragma: no cover
             return alg_class(self.cryptography_key)  # pragma: no cover
         raise UnsupportedAlg(alg)  # pragma: no cover
 
-    def key_management_wrapper(self, alg: Optional[str] = None) -> BaseKeyManagementAlg:
+    def key_management_wrapper(self, alg: str | None = None) -> BaseKeyManagementAlg:
         """Initialize a key management wrapper with this key.
 
         This returns an instance of a `BaseKeyManagementAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
@@ -633,44 +623,42 @@
         alg_class = self.key_management_class(alg)
         if issubclass(alg_class, BaseSymmetricAlg):
             return alg_class(self.key)
         elif issubclass(alg_class, BaseAsymmetricAlg):
             return alg_class(self.cryptography_key)
         raise UnsupportedAlg(alg)  # pragma: no cover
 
-    def supported_signing_algorithms(self) -> List[str]:
+    def supported_signing_algorithms(self) -> list[str]:
         """Return the list of Signature algorithms that can be used with this key.
 
         Returns:
           a list of supported algs
 
         """
         return list(self.SIGNATURE_ALGORITHMS)
 
-    def supported_key_management_algorithms(self) -> List[str]:
+    def supported_key_management_algorithms(self) -> list[str]:
         """Return the list of Key Management algorithms that can be used with this key.
 
         Returns:
             a list of supported algs
 
         """
         return list(self.KEY_MANAGEMENT_ALGORITHMS)
 
-    def supported_encryption_algorithms(self) -> List[str]:
+    def supported_encryption_algorithms(self) -> list[str]:
         """Return the list of Encryption algorithms that can be used with this key.
 
         Returns:
             a list of supported algs
 
         """
         return list(self.ENCRYPTION_ALGORITHMS)
 
-    def sign(
-        self, data: Union[bytes, SupportsBytes], alg: Optional[str] = None
-    ) -> BinaPy:
+    def sign(self, data: bytes | SupportsBytes, alg: str | None = None) -> BinaPy:
         """Sign a data using this Jwk, and return the generated signature.
 
         Args:
           data: the data to sign
           alg: the alg to use (if this key doesn't have an `alg` parameter)
 
         Returns:
@@ -679,35 +667,36 @@
         """
         wrapper = self.signature_wrapper(alg)
         signature = wrapper.sign(data)
         return BinaPy(signature)
 
     def verify(
         self,
-        data: Union[bytes, SupportsBytes],
-        signature: Union[bytes, SupportsBytes],
+        data: bytes | SupportsBytes,
+        signature: bytes | SupportsBytes,
         *,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> bool:
         """Verify a signature using this `Jwk`, and return `True` if valid.
 
         Args:
           data: the data to verify
           signature: the signature to verify
           alg: the allowed signature alg, if there is only one
           algs: the allowed signature algs, if there are several
 
         Returns:
           `True` if the signature matches, `False` otherwise
+
         """
         if not self.is_symmetric and self.is_private:
             warnings.warn(
                 "You are trying to validate a signature with a private key. "
-                "Signature should always be verified with a public key."
+                "Signatures should always be verified with a public key."
             )
             public_jwk = self.public_jwk()
         else:
             public_jwk = self
         if algs is None and alg:
             algs = [alg]
         for alg in algs or (None,):
@@ -715,20 +704,20 @@
             if wrapper.verify(data, signature):
                 return True
 
         return False
 
     def encrypt(
         self,
-        plaintext: Union[bytes, SupportsBytes],
+        plaintext: bytes | SupportsBytes,
         *,
-        aad: Optional[bytes] = None,
-        alg: Optional[str] = None,
-        iv: Optional[bytes] = None,
-    ) -> Tuple[BinaPy, BinaPy, BinaPy]:
+        aad: bytes | None = None,
+        alg: str | None = None,
+        iv: bytes | None = None,
+    ) -> tuple[BinaPy, BinaPy, BinaPy]:
         """Encrypt a plaintext with Authenticated Encryption using this key.
 
         Authenticated Encryption with Associated Data (AEAD) is supported, by passing Additional Authenticated Data (`aad`).
         This returns a tuple with 3 raw data, in order:
         - the encrypted Data
         - the Initialization Vector that was used to encrypt data
         - the generated Authentication Tag
@@ -743,20 +732,20 @@
           a tuple (ciphertext, iv, authentication_tag), as raw data
 
         """
         raise NotImplementedError  # pragma: no cover
 
     def decrypt(
         self,
-        ciphertext: Union[bytes, SupportsBytes],
+        ciphertext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        tag: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
-        alg: Optional[str] = None,
+        iv: bytes | SupportsBytes,
+        tag: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
+        alg: str | None = None,
     ) -> BinaPy:
         """Decrypt an encrypted data using this Jwk, and return the encrypted result.
 
         This is implemented by subclasses.
 
         Args:
           ciphertext: the data to decrypt
@@ -771,19 +760,19 @@
         """
         raise NotImplementedError  # pragma: no cover
 
     def sender_key(
         self,
         enc: str,
         *,
-        alg: Optional[str] = None,
-        cek: Optional[bytes] = None,
-        epk: Optional[Jwk] = None,
+        alg: str | None = None,
+        cek: bytes | None = None,
+        epk: Jwk | None = None,
         **headers: Any,
-    ) -> Tuple[Jwk, BinaPy, Mapping[str, Any]]:
+    ) -> tuple[Jwk, BinaPy, Mapping[str, Any]]:
         """Produce a Content Encryption Key, to use for encryption.
 
         This method is meant to be used by encrypted token senders. Recipients should use the matching method `Jwk.recipient_key()`.
 
         Returns a tuple with 3 items:
 
         - the clear text CEK, as a SymmetricJwk instance. Use this key to encrypt your message, but do not communicate this key to anyone!
@@ -818,15 +807,15 @@
             )
             key_alg_wrapper = self.public_jwk().key_management_wrapper(alg)
         else:
             key_alg_wrapper = self.key_management_wrapper(alg)
 
         enc_alg_class = select_alg_class(SymmetricJwk.ENCRYPTION_ALGORITHMS, alg=enc)
 
-        cek_headers: Dict[str, Any] = {}
+        cek_headers: dict[str, Any] = {}
 
         if isinstance(key_alg_wrapper, BaseRsaKeyWrap):
             if cek:
                 enc_alg_class.check_key(cek)
             else:
                 cek = enc_alg_class.generate_key()
             assert cek
@@ -884,18 +873,18 @@
                 f"Unsupported Key Management Alg {key_alg_wrapper}"
             )  # pragma: no cover
 
         return SymmetricJwk.from_bytes(cek), wrapped_cek, cek_headers
 
     def recipient_key(
         self,
-        wrapped_cek: Union[bytes, SupportsBytes],
+        wrapped_cek: bytes | SupportsBytes,
         enc: str,
         *,
-        alg: Optional[str] = None,
+        alg: str | None = None,
         **headers: Any,
     ) -> Jwk:
         """Produce a Content Encryption Key, to use for decryption.
 
         This method is meant to be used by encrypted token recipient. Senders should use the matching method `Jwk.sender_key()`.
 
         Args:
@@ -1028,14 +1017,15 @@
           **kwargs: additional members to include in the Jwk (e.g. kid, use)
 
         Returns:
             the matching `Jwk` instance
 
         Raises:
             TypeError: if the key type is not supported
+
         """
         for cryptography_class, jwk_class in cls.cryptography_key_types.items():
             if isinstance(cryptography_key, cryptography_class):
                 return jwk_class.from_cryptography_key(cryptography_key, **kwargs)
 
         raise TypeError(
             f"Unsupported Jwk class for this Key Type: {type(cryptography_key).__name__}"
@@ -1044,33 +1034,35 @@
     def _to_cryptography_key(self) -> Any:
         """Return a key from the `cryptography` library that matches this Jwk.
 
         This is implemented by subclasses.
 
         Returns:
             a `cryptography`key instance initialized from the current key
+
         """
         raise NotImplementedError
 
     @classmethod
     def from_pem(
         cls,
-        der: Union[bytes, str],
-        password: Union[bytes, str, None] = None,
+        der: bytes | str,
+        password: bytes | str | None = None,
         **kwargs: Any,
     ) -> Jwk:
         """Load a `Jwk` from a PEM encoded private or public key.
 
         Args:
           der: the PEM encoded data to load
           password: the password to decrypt the PEM, if required. Should be bytes. If it is a string, it will be encoded with UTF-8.
           **kwargs: additional members to include in the `Jwk` (e.g. `kid`, `use`)
 
         Returns:
             a `Jwk` instance from the loaded key
+
         """
         der = der.encode() if isinstance(der, str) else der
         password = password.encode("UTF-8") if isinstance(password, str) else password
 
         try:
             cryptography_key = serialization.load_pem_private_key(der, password)
         except Exception as private_exc:
@@ -1085,15 +1077,15 @@
                 raise ValueError(
                     "A public key was loaded from PEM, while a password was provided for decryption."
                     "Only private keys are encrypted using a password."
                 )
 
         return cls.from_cryptography_key(cryptography_key, **kwargs)
 
-    def to_pem(self, password: Union[bytes, str, None] = None) -> str:
+    def to_pem(self, password: bytes | str | None = None) -> str:
         """Serialize this key to PEM format.
 
         For private keys, you can provide a password for encryption. This password should be `bytes`. A `str` is also
         accepted, and will be encoded to `bytes` using UTF-8 before it is used as encryption key.
 
         Args:
           password: password to use to encrypt the PEM.
@@ -1123,15 +1115,15 @@
                 serialization.PublicFormat.SubjectPublicKeyInfo,
             ).decode()
 
     @classmethod
     def from_der(
         cls,
         der: bytes,
-        password: Union[bytes, str, None] = None,
+        password: bytes | str | None = None,
         **kwargs: Any,
     ) -> Jwk:
         """Load a `Jwk` from DER."""
         password = password.encode("UTF-8") if isinstance(password, str) else password
 
         try:
             cryptography_key = serialization.load_der_private_key(der, password)
@@ -1146,15 +1138,15 @@
                 raise ValueError(
                     "A public key was loaded from DER, while a password was provided for decryption."
                     "Only private keys are encrypted using a password."
                 )
 
         return cls.from_cryptography_key(cryptography_key, **kwargs)
 
-    def to_der(self, password: Union[bytes, str, None] = None) -> BinaPy:
+    def to_der(self, password: bytes | str | None = None) -> BinaPy:
         """Serialize this key to DER.
 
         For private keys, you can provide a password for encryption. This password should be bytes. A `str` is also
         accepted, and will be encoded to `bytes` using UTF-8 before it is used as encryption key.
 
         Args:
           password: password to use to encrypt the PEM. Should be bytes. If it is a string, it will be encoded to bytes with UTF-8.
@@ -1186,34 +1178,35 @@
                     serialization.Encoding.DER,
                     serialization.PublicFormat.SubjectPublicKeyInfo,
                 )
             )
 
     @classmethod
     def generate(
-        cls, *, alg: Optional[str] = None, kty: Optional[str] = None, **kwargs: Any
+        cls, *, alg: str | None = None, kty: str | None = None, **kwargs: Any
     ) -> Jwk:
         """Generate a Private Key and return it as a `Jwk` instance.
 
         This method is implemented by subclasses for specific Key Types and returns an instance of that subclass.
 
         Args:
             alg: intended algorithm to use with the generated key
             kty: key type identifier
             **kwargs: specific parameters depending on the type of key, or additional members to include in the `Jwk`
 
         Returns:
             a `Jwk` instance with a generated key
+
         """
         if alg:
             key = cls.generate_for_alg(alg=alg, **kwargs)
             if kty is not None and key.kty != kty:
                 raise ValueError(
                     f"Incompatible `{alg=}` and `{kty=}` parameters. "
-                    f"`{alg=}` points to key with `kty='{key.kty}'`."
+                    f"`{alg=}` points to `kty='{key.kty}'`."
                 )
             return key
         if kty:
             return cls.generate_for_kty(kty=kty, **kwargs)
         raise ValueError(
             "You must provide a hint for jwskate to know what kind of key it must generate. "
             "You can either provide an 'alg' identifier as keyword parameter, and/or a 'kty'."
@@ -1246,15 +1239,15 @@
             return self
         jwk = self.copy()
         jwk["kid"] = self.thumbprint()
         return jwk
 
     def with_usage_parameters(
         self,
-        alg: Optional[str] = None,
+        alg: str | None = None,
         with_alg: bool = True,
         with_use: bool = True,
         with_key_ops: bool = True,
     ) -> Jwk:
         """Copy this Jwk and add the `use` and `key_ops` parameters.
 
         The returned jwk `alg` parameter will be the one passed as parameter to this method, or as dfault the one declared as `alg` parameter in this Jwk.
@@ -1266,14 +1259,15 @@
             alg: the alg to use, if not present in this Jwk
             with_alg: whether to include an `alg` parameter
             with_use: whether to include a `use` parameter
             with_key_ops: whether to include a `key_ops` parameter
 
         Returns:
             a Jwk with the same key, with `alg`, `use` and `key_ops` parameters.
+
         """
         alg = alg or self.alg
 
         if not alg:
             raise ExpectedAlgRequired(
                 "An algorithm is required to set the usage parameters"
             )
@@ -1310,17 +1304,17 @@
         other = to_jwk(other)
         return super(Jwk, self.minimize()).__eq__(other.minimize())
 
 
 def to_jwk(
     key: Any,
     *,
-    kty: Optional[str] = None,
-    is_private: Optional[bool] = None,
-    is_symmetric: Optional[bool] = None,
+    kty: str | None = None,
+    is_private: bool | None = None,
+    is_symmetric: bool | None = None,
 ) -> Jwk:
     """Convert any supported kind of key to a `Jwk`.
 
     This optionally check if that key is private or symmetric.
 
     The key can be any type supported by Jwk:
     - a `cryptography` key instance
@@ -1333,10 +1327,11 @@
         key: the key material
         kty: the expected key type
         is_private: if `True`, check if the key is private, if `False`, check if it is public, if `None`, do nothing
         is_symmetric: if `True`, check if the key is symmetric, if `False`, check if it is asymmetric, if `None`, do nothing
 
     Returns:
         a Jwk key
+
     """
     jwk = key if isinstance(key, Jwk) else Jwk(key)
     return jwk.check(kty=kty, is_private=is_private, is_symmetric=is_symmetric)
```

### Comparing `jwskate-0.8.0/jwskate/jwk/ec.py` & `jwskate-0.9.0/jwskate/jwk/ec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """This module implements JWK representing Elliptic Curve keys."""
-
 from __future__ import annotations
 
 import warnings
 from functools import cached_property
-from typing import Any, List, Mapping, Optional, Type, Union
+from typing import Any, Mapping
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives.asymmetric import ec
 from typing_extensions import override
 
 from jwskate.jwa import (
     ES256,
@@ -62,19 +61,19 @@
         ),
     }
 
     CURVES: Mapping[str, EllipticCurve] = {
         curve.name: curve for curve in [P_256, P_384, P_521, secp256k1]
     }
 
-    SIGNATURE_ALGORITHMS: Mapping[str, Type[BaseECSignatureAlg]] = {
+    SIGNATURE_ALGORITHMS: Mapping[str, type[BaseECSignatureAlg]] = {
         sigalg.name: sigalg for sigalg in [ES256, ES384, ES512, ES256K]
     }
 
-    KEY_MANAGEMENT_ALGORITHMS: Mapping[str, Type[EcdhEs]] = {
+    KEY_MANAGEMENT_ALGORITHMS: Mapping[str, type[EcdhEs]] = {
         keyalg.name: keyalg
         for keyalg in [EcdhEs, EcdhEs_A128KW, EcdhEs_A192KW, EcdhEs_A256KW]
     }
 
     @property
     @override
     def is_private(self) -> bool:
@@ -106,14 +105,15 @@
 
     @property
     def curve(self) -> EllipticCurve:
         """Get the `EllipticCurve` instance for this key.
 
         Returns:
             the `EllipticCurve` instance
+
         """
         return self.get_curve(self.crv)
 
     @classmethod
     def public(cls, *, crv: str, x: int, y: int, **params: str) -> ECJwk:
         """Initialize a public `ECJwk` from its public parameters.
 
@@ -121,14 +121,15 @@
           crv: the curve to use
           x: the x coordinate
           y: the y coordinate
           **params: additional member to include in the Jwk
 
         Returns:
           an ECJwk initialized with the supplied parameters
+
         """
         coord_size = cls.get_curve(crv).coordinate_size
         return cls(
             dict(
                 kty=cls.KTY,
                 crv=crv,
                 x=BinaPy.from_int(x, length=coord_size).to("b64u").ascii(),
@@ -163,15 +164,15 @@
                 **{k: v for k, v in params.items() if v is not None},
             )
         )
 
     @classmethod
     @override
     def generate(
-        cls, *, crv: Optional[str] = None, alg: Optional[str] = None, **kwargs: Any
+        cls, *, crv: str | None = None, alg: str | None = None, **kwargs: Any
     ) -> ECJwk:
         curve: EllipticCurve = P_256
 
         if crv is None and alg is None:
             raise ValueError(
                 "No Curve identifier (crv) or Algorithm identifier (alg) have been provided "
                 "when generating an Elliptic Curve JWK. So there is no hint to determine which curve to use. "
@@ -206,15 +207,15 @@
     def from_cryptography_key(cls, cryptography_key: Any, **kwargs: Any) -> ECJwk:
         parameters = EllipticCurve.get_jwk_parameters(cryptography_key)
         return cls(parameters)
 
     @override
     def _to_cryptography_key(
         self,
-    ) -> Union[ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey,]:
+    ) -> ec.EllipticCurvePrivateKey | ec.EllipticCurvePublicKey:
         if self.is_private:
             return ec.EllipticCurvePrivateNumbers(
                 private_value=self.ecc_private_key,
                 public_numbers=ec.EllipticCurvePublicNumbers(
                     x=self.x_coordinate,
                     y=self.y_coordinate,
                     curve=self.curve.cryptography_curve,
@@ -248,21 +249,21 @@
 
     @cached_property
     def ecc_private_key(self) -> int:
         """Return the *ECC private key*, parameter `d` from this `ECJwk`."""
         return BinaPy(self.d).decode_from("b64u").to_int()
 
     @override
-    def supported_signing_algorithms(self) -> List[str]:
+    def supported_signing_algorithms(self) -> list[str]:
         return [
             name
             for name, alg in self.SIGNATURE_ALGORITHMS.items()
             if alg.curve == self.curve
         ]
 
     @override
-    def supported_key_management_algorithms(self) -> List[str]:
+    def supported_key_management_algorithms(self) -> list[str]:
         return list(self.KEY_MANAGEMENT_ALGORITHMS)
 
     @override
-    def supported_encryption_algorithms(self) -> List[str]:
+    def supported_encryption_algorithms(self) -> list[str]:
         return list(self.ENCRYPTION_ALGORITHMS)
```

### Comparing `jwskate-0.8.0/jwskate/jwk/jwks.py` & `jwskate-0.9.0/jwskate/jwk/jwks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements Json Web Key Sets (JWKS)."""
+from __future__ import annotations
 
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Iterable
 
 from ..token import BaseJsonDict
 from .base import Jwk, to_jwk
 
 
 class JwkSet(BaseJsonDict):
     """A set of JWK keys, with methods for easy management of keys.
@@ -22,16 +23,16 @@
         jwks: a dict, containing the JwkSet, parsed as a JSON object.
         keys: a list of `Jwk`, that will be added to this JwkSet
 
     """
 
     def __init__(
         self,
-        jwks: Optional[Dict[str, Any]] = None,
-        keys: Optional[Iterable[Union[Jwk, Dict[str, Any]]]] = None,
+        jwks: dict[str, Any] | None = None,
+        keys: Iterable[Jwk | dict[str, Any]] | None = None,
     ):
         if jwks is None and keys is None:
             keys = []
 
         if jwks is not None:
             keys = jwks.pop("keys", [])
             super().__init__(
@@ -41,19 +42,20 @@
             super().__init__()
 
         if keys is not None:
             for jwk in keys:
                 self.add_jwk(jwk)
 
     @property
-    def jwks(self) -> List[Jwk]:
+    def jwks(self) -> list[Jwk]:
         """Return the list of keys from this JwkSet, as `Jwk` instances.
 
         Returns:
             a list of `Jwk`
+
         """
         return self.get("keys", [])
 
     def get_jwk_by_kid(self, kid: str) -> Jwk:
         """Return a Jwk from this JwkSet, based on its kid.
 
         Args:
@@ -78,17 +80,17 @@
             the number of keys
 
         """
         return len(self.jwks)
 
     def add_jwk(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
-        kid: Optional[str] = None,
-        use: Optional[str] = None,
+        key: Jwk | dict[str, Any] | Any,
+        kid: str | None = None,
+        use: str | None = None,
     ) -> str:
         """Add a Jwk in this JwkSet.
 
         Args:
           key: the Jwk to add (either a `Jwk` instance, or a dict containing the Jwk parameters)
           kid: the kid to use, if `jwk` doesn't contain one
           use: the defined use for the added Jwk
@@ -116,14 +118,15 @@
         """Remove a Jwk from this JwkSet, based on a `kid`.
 
         Args:
           kid: the `kid` from the key to be removed.
 
         Raises:
             KeyError: if no key matches
+
         """
         try:
             jwk = self.get_jwk_by_kid(kid)
             self.jwks.remove(jwk)
         except KeyError:
             pass
 
@@ -133,24 +136,24 @@
 
         Returns:
             `True` if this JwkSet contains at least one private key
 
         """
         return any(key.is_private for key in self.jwks)
 
-    def public_jwks(self) -> "JwkSet":
+    def public_jwks(self) -> JwkSet:
         """Return another JwkSet with the public keys associated with the current keys.
 
         Returns:
             a public JwkSet
 
         """
         return JwkSet(keys=(key.public_jwk() for key in self.jwks))
 
-    def verification_keys(self) -> List[Jwk]:
+    def verification_keys(self) -> list[Jwk]:
         """Return the list of keys from this JWKS that are usable for signature verification.
 
         To be usable for signature verification, a key must:
 
         - be asymmetric
         - be public
         - be flagged for signature, either with `use=sig` or an `alg` that is compatible with signature
@@ -165,17 +168,17 @@
             if not jwk.is_symmetric and not jwk.is_private and jwk.use == "sig"
         ]
 
     def verify(
         self,
         data: bytes,
         signature: bytes,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
-        kid: Optional[str] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
+        kid: str | None = None,
     ) -> bool:
         """Verify a signature with the keys from this key set.
 
         If a `kid` is provided, only that Key ID will be tried. Otherwise, all keys that are compatible with the
         specified alg(s) will be tried.
 
         Args:
@@ -210,15 +213,15 @@
                 if alg in jwk.supported_signing_algorithms():
                     if jwk.verify(data, signature, alg=alg):
                         return True
 
         # no key matches, so consider the signature invalid
         return False
 
-    def encryption_keys(self) -> List[Jwk]:
+    def encryption_keys(self) -> list[Jwk]:
         """Return the list of keys from this JWKS that are usable for encryption.
 
         To be usable for encryption, a key must:
 
         - be asymmetric
         - be public
         - be flagged for encryption, either with `use=enc` or an `alg` parameter that is an encryption alg
```

### Comparing `jwskate-0.8.0/jwskate/jwk/oct.py` & `jwskate-0.9.0/jwskate/jwk/oct.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implements JWK representing Symmetric keys."""
-
 from __future__ import annotations
 
 import warnings
-from typing import Any, List, Optional, SupportsBytes, Tuple, Union
+from typing import Any, SupportsBytes
 
 from binapy import BinaPy
 from typing_extensions import override
 
 from jwskate.jwa import (
     A128CBC_HS256,
     A128GCM,
@@ -88,32 +87,33 @@
         Raises:
             ValueError: symmetric keys are always private, it makes no sense to use them as public keys
 
         """
         raise ValueError("Symmetric keys don't have a public key")
 
     @classmethod
-    def from_bytes(cls, k: Union[bytes, str], **params: Any) -> SymmetricJwk:
+    def from_bytes(cls, k: bytes | str, **params: Any) -> SymmetricJwk:
         """Initialize a `SymmetricJwk` from a raw secret key.
 
         The provided secret key is encoded and used as the `k` parameter for the returned `SymmetricKey`.
 
         Args:
           k: the key to use
           **params: additional members to include in the `Jwk`
 
         Returns:
           the resulting `SymmetricJwk`
+
         """
         return cls(dict(kty=cls.KTY, k=BinaPy(k).to("b64u").ascii(), **params))
 
     @classmethod
     @override
     def generate(
-        cls, *, alg: Optional[str] = None, key_size: Optional[int] = None, **params: Any
+        cls, *, alg: str | None = None, key_size: int | None = None, **params: Any
     ) -> SymmetricJwk:
         if alg:
             alg_class = cls._get_alg_class(alg)
             # special cases for AES or HMAC based algs which require a specific key size
             if issubclass(alg_class, (BaseAESEncryptionAlg, BaseAesKeyWrap)):
                 if key_size is not None and key_size != alg_class.key_size:
                     raise ValueError(
@@ -158,15 +158,15 @@
             BinaPy.serialize_to("json", {"k": self.k, "kty": self.kty})
             .to("sha256")
             .to("b64u")
             .ascii()
         )
 
     @override
-    def to_pem(self, password: Union[bytes, str, None] = None) -> str:
+    def to_pem(self, password: bytes | str | None = None) -> str:
         raise TypeError("Symmetric keys are not serializable to PEM.")
 
     @property
     def key(self) -> BinaPy:
         """Returns the raw symmetric key, from the `k` parameter, base64u-decoded."""
         return self.cryptography_key  # type: ignore[no-any-return]
 
@@ -174,20 +174,20 @@
     def key_size(self) -> int:
         """The key size, in bits."""
         return len(self.key) * 8
 
     @override
     def encrypt(
         self,
-        plaintext: Union[bytes, SupportsBytes],
+        plaintext: bytes | SupportsBytes,
         *,
-        aad: Optional[bytes] = None,
-        alg: Optional[str] = None,
-        iv: Optional[bytes] = None,
-    ) -> Tuple[BinaPy, BinaPy, BinaPy]:
+        aad: bytes | None = None,
+        alg: str | None = None,
+        iv: bytes | None = None,
+    ) -> tuple[BinaPy, BinaPy, BinaPy]:
         """Encrypt arbitrary data using this key.
 
         Supports Authenticated Encryption with Additional Authenticated Data (use parameter `aad` for Additional
         Authenticated Data).
 
         An *Initialization Vector* (IV) will be generated automatically.
         You can choose your own IV by providing the `iv` parameter (only use this if you know what you are doing).
@@ -211,20 +211,20 @@
 
         ciphertext, tag = wrapper.encrypt(plaintext, iv=iv, aad=aad)
         return ciphertext, BinaPy(iv), tag
 
     @override
     def decrypt(
         self,
-        ciphertext: Union[bytes, SupportsBytes],
+        ciphertext: bytes | SupportsBytes,
         *,
-        iv: Union[bytes, SupportsBytes],
-        tag: Union[bytes, SupportsBytes],
-        aad: Union[bytes, SupportsBytes, None] = None,
-        alg: Optional[str] = None,
+        iv: bytes | SupportsBytes,
+        tag: bytes | SupportsBytes,
+        aad: bytes | SupportsBytes | None = None,
+        alg: str | None = None,
     ) -> BinaPy:
         """Decrypt arbitrary data, and verify Additional Authenticated Data.
 
         Args:
           ciphertext: the encrypted data
           iv: the Initialization Vector (must be the same as generated during encryption)
           tag: the authentication tag
@@ -245,22 +245,22 @@
 
         wrapper = self.encryption_wrapper(alg)
         plaintext: bytes = wrapper.decrypt(ciphertext, auth_tag=tag, iv=iv, aad=aad)
 
         return BinaPy(plaintext)
 
     @override
-    def supported_key_management_algorithms(self) -> List[str]:
+    def supported_key_management_algorithms(self) -> list[str]:
         return [
             name
             for name, alg in self.KEY_MANAGEMENT_ALGORITHMS.items()
             if issubclass(alg, BaseSymmetricAlg)
             and alg.supports_key(self.cryptography_key)
         ]
 
     @override
-    def supported_encryption_algorithms(self) -> List[str]:
+    def supported_encryption_algorithms(self) -> list[str]:
         return [
             name
             for name, alg in self.ENCRYPTION_ALGORITHMS.items()
             if alg.supports_key(self.cryptography_key)
         ]
```

### Comparing `jwskate-0.8.0/jwskate/jwk/okp.py` & `jwskate-0.9.0/jwskate/jwk/okp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """This module implements JWK representing Octet Key Pairs from [RFC8037].
 
 [RFC8037]
 : https: //www.rfc-editor.org/rfc/rfc8037.html
 
 """
-
 from __future__ import annotations
 
 from functools import cached_property
-from typing import Any, Mapping, Optional
+from typing import Any, Mapping
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519, x448, x25519
 from typing_extensions import override
 
 from jwskate.jwa import (
@@ -100,14 +99,15 @@
           crv: a curve identifier
 
         Returns:
             the matching `OKPCurve` instance
 
         Raises:
             UnsupportedOKPCurve: if the curve is not supported
+
         """
         curve = cls.CURVES.get(crv)
         if curve is None:
             raise UnsupportedOKPCurve(crv)
         return curve
 
     @property
@@ -125,16 +125,16 @@
         """Get the private key from this `Jwk`, from param `d`, base64url-decoded."""
         return BinaPy(self.d).decode_from("b64u")
 
     @classmethod
     def from_bytes(
         cls,
         private_key: bytes,
-        crv: Optional[str] = None,
-        use: Optional[str] = None,
+        crv: str | None = None,
+        use: str | None = None,
         **kwargs: Any,
     ) -> OKPJwk:
         """Initialize an `OKPJwk` from its private key, as `bytes`.
 
         The public key will be automatically derived from the supplied private key, according to the OKP curve.
 
         The appropriate curve will be guessed based on the key length or supplied `crv`/`use` hints:
@@ -148,14 +148,15 @@
             private_key: the 32, 56 or 57 bytes private key, as raw `bytes`
             crv: the curve identifier to use
             use: the key usage
             **kwargs: additional members to include in the `Jwk`
 
         Returns:
             the matching `OKPJwk`
+
         """
         if crv and use:
             if (crv in ("Ed25519", "Ed448") and use != "sig") or (
                 crv in ("X25519", "X448") and use != "enc"
             ):
                 raise ValueError(
                     f"Inconsistent `crv={crv}` and `use={use}` parameters. "
@@ -277,14 +278,15 @@
         Args:
           crv: the key curve
           x: the public key
           **params: additional members to include in the `Jwk`
 
         Returns:
             the resulting `OKPJwk`
+
         """
         return cls(dict(kty=cls.KTY, crv=crv, x=BinaPy(x).to("b64u").ascii(), **params))
 
     @classmethod
     def private(cls, *, crv: str, x: bytes, d: bytes, **params: Any) -> OKPJwk:
         """Initialize a private `OKPJwk` based on the provided parameters.
 
@@ -292,29 +294,30 @@
           crv: the OKP curve
           x: the public key
           d: the private key
           **params: additional members to include in the `Jwk`
 
         Returns:
             the resulting `OKPJwk`
+
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 crv=crv,
                 x=BinaPy(x).to("b64u").ascii(),
                 d=BinaPy(d).to("b64u").ascii(),
                 **params,
             )
         )
 
     @classmethod
     @override
     def generate(
-        cls, *, crv: Optional[str] = None, alg: Optional[str] = None, **params: Any
+        cls, *, crv: str | None = None, alg: str | None = None, **params: Any
     ) -> OKPJwk:
         if crv:
             curve = cls.get_curve(crv)
         elif alg:
             if alg in cls.SIGNATURE_ALGORITHMS:
                 curve = Ed25519
             elif alg in cls.KEY_MANAGEMENT_ALGORITHMS:
@@ -328,13 +331,13 @@
             )
 
         x, d = curve.generate()
         return cls.private(crv=curve.name, x=x, d=d, alg=alg, **params)
 
     @cached_property
     @override
-    def use(self) -> Optional[str]:
+    def use(self) -> str | None:
         if self.curve in (Ed25519, Ed448):
             return "sig"
         elif self.curve in (X25519, X448):
             return "enc"
         raise UnsupportedOKPCurve(self.curse)  # pragma: no-cover
```

### Comparing `jwskate-0.8.0/jwskate/jwk/rsa.py` & `jwskate-0.9.0/jwskate/jwk/rsa.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implements JWK representing RSA keys."""
-
 from __future__ import annotations
 
 from functools import cached_property
-from typing import Any, Optional, Tuple, Union
+from typing import Any
 
 from binapy import BinaPy
 from cryptography.hazmat.primitives.asymmetric import rsa
 from typing_extensions import override
 
 from jwskate.jwa import (
     PS256,
@@ -109,15 +108,15 @@
                 n=pub.n,
                 e=pub.e,
             )
         else:
             raise TypeError("A RSAPrivateKey or a RSAPublicKey is required.")
 
     @override
-    def _to_cryptography_key(self) -> Union[rsa.RSAPrivateKey, rsa.RSAPublicKey]:
+    def _to_cryptography_key(self) -> rsa.RSAPrivateKey | rsa.RSAPublicKey:
         if self.is_private:
             return rsa.RSAPrivateNumbers(
                 self.first_prime_factor,
                 self.second_prime_factor,
                 self.private_exponent,
                 self.first_factor_crt_exponent,
                 self.second_factor_crt_exponent,
@@ -133,15 +132,16 @@
 
         Args:
           n: the modulus
           e: the exponent
           **params: additional parameters to include in the `Jwk`
 
         Returns:
-          a `RsaJwk` initialized from the provided parameters
+          a `RSAJwk` initialized from the provided parameters
+
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 n=BinaPy.from_int(n).to("b64u").ascii(),
                 e=BinaPy.from_int(e).to("b64u").ascii(),
                 **params,
@@ -151,36 +151,37 @@
     @classmethod
     def private(
         cls,
         *,
         n: int,
         e: int = 65537,
         d: int,
-        p: Optional[int] = None,
-        q: Optional[int] = None,
-        dp: Optional[int] = None,
-        dq: Optional[int] = None,
-        qi: Optional[int] = None,
+        p: int | None = None,
+        q: int | None = None,
+        dp: int | None = None,
+        dq: int | None = None,
+        qi: int | None = None,
         **params: Any,
     ) -> RSAJwk:
-        """Initialize a private `RsaJwk` from its required parameters.
+        """Initialize a private `RSAJwk` from its required parameters.
 
         Args:
           n: the modulus
           e: the exponent
           d: the private exponent
           p: the first prime factor
           q: the second prime factor
           dp: the first factor CRT exponent
           dq: the second factor CRT exponent
           qi: the first CRT coefficient
           **params: additional parameters to include in the `Jwk`
 
         Returns:
             a `RSAJwk` initialized from the given parameters
+
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 n=BinaPy.from_int(n).to("b64u").ascii(),
                 e=BinaPy.from_int(e).to("b64u").ascii(),
                 d=BinaPy.from_int(d).to("b64u").ascii(),
@@ -189,14 +190,36 @@
                 dp=BinaPy.from_int(dp).to("b64u").ascii() if dp is not None else None,
                 dq=BinaPy.from_int(dq).to("b64u").ascii() if dq is not None else None,
                 qi=BinaPy.from_int(qi).to("b64u").ascii() if qi is not None else None,
                 **params,
             )
         )
 
+    @classmethod
+    def from_prime_factors(cls, p: int, q: int, e: int = 65537) -> RSAJwk:
+        """Initialise a `RSAJwk` from its prime factors and exponent.
+
+        Modulus and Private Exponent are mathematically calculated based on those factors.
+
+        Exponent is usually 65537 (default).
+
+        Args:
+            p: first prime factor
+            q: second prime factor
+            e: exponent
+
+        Returns:
+            a `RSAJwk`
+
+        """
+        n = p * q
+        phi = (p - 1) * (q - 1)
+        d = pow(e, -1, phi)
+        return cls.private(n=n, e=e, d=d)
+
     @cached_property
     def key_size(self) -> int:
         """Key size, in bits."""
         return len(BinaPy(self.n).decode_from("b64u")) * 8
 
     @classmethod
     def generate(cls, key_size: int = 4096, **params: Any) -> RSAJwk:
@@ -204,14 +227,15 @@
 
         Args:
           key_size: the key size to use for the generated key, in bits
           **params: additional parameters to include in the `Jwk`
 
         Returns:
           a generated `RSAJwk`
+
         """
         private_key = rsa.generate_private_key(65537, key_size=key_size)
         pn = private_key.private_numbers()
         return cls.private(
             n=pn.public_numbers.n,
             e=pn.public_numbers.e,
             d=pn.d,
@@ -235,15 +259,15 @@
 
     @cached_property
     def private_exponent(self) -> int:
         """Return the private exponent `d` from this `Jwk`."""
         return BinaPy(self.d).decode_from("b64u").to_int()
 
     @cached_property
-    def prime_factors(self) -> Tuple[int, int]:
+    def prime_factors(self) -> tuple[int, int]:
         """Return the 2 prime factors `p` and `q` from this `Jwk`."""
         if "p" not in self or "q" not in self:
             p, q = rsa.rsa_recover_prime_factors(
                 self.modulus, self.exponent, self.private_exponent
             )
             return (p, q) if p < q else (q, p)
         return (
```

### Comparing `jwskate-0.8.0/jwskate/jws/compact.py` & `jwskate-0.9.0/jwskate/jws/compact.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implements the JWS Compact format."""
-
 from __future__ import annotations
 
 from functools import cached_property
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, SupportsBytes, Union
+from typing import TYPE_CHECKING, Any, Iterable, SupportsBytes
 
 from binapy import BinaPy
 
 from jwskate.jwk.base import Jwk, to_jwk
 from jwskate.token import BaseCompactToken
 
 from .signature import JwsSignature
@@ -24,15 +23,15 @@
     """Represents a Json Web Signature (JWS), using compact serialization, as defined in RFC7515.
 
     Args:
         value: the JWS token value
 
     """
 
-    def __init__(self, value: Union[bytes, str], max_size: int = 16 * 1024):
+    def __init__(self, value: bytes | str, max_size: int = 16 * 1024):
         super().__init__(value, max_size)
 
         if self.value.count(b".") != 2:
             raise InvalidJws(
                 "A JWS must contain a header, a payload and a signature, separated by dots"
             )
 
@@ -58,18 +57,18 @@
             raise InvalidJws(
                 "Invalid JWS signature: it must be a Base64URL-encoded binary data (bytes)"
             )
 
     @classmethod
     def sign(
         cls,
-        payload: Union[bytes, SupportsBytes],
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        extra_headers: Optional[Dict[str, Any]] = None,
+        payload: bytes | SupportsBytes,
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        extra_headers: dict[str, Any] | None = None,
     ) -> JwsCompact:
         """Sign a payload and returns the resulting JwsCompact.
 
         Args:
           payload: the payload to sign
           key: the jwk to use to sign this payload
           alg: the alg to use
@@ -92,16 +91,16 @@
         signed_part = JwsSignature.assemble_signed_part(headers, payload)
         signature = key.sign(signed_part, alg=alg)
         return cls.from_parts(signed_part, signature)
 
     @classmethod
     def from_parts(
         cls,
-        signed_part: Union[bytes, SupportsBytes, str],
-        signature: Union[bytes, SupportsBytes],
+        signed_part: bytes | SupportsBytes | str,
+        signature: bytes | SupportsBytes,
     ) -> JwsCompact:
         """Construct a JWS token based on its signed part and signature values.
 
         Signed part is the concatenation of the header and payload, both encoded in Base64-Url, and joined by a dot.
 
         Args:
           signed_part: the signed part
@@ -129,18 +128,18 @@
             the signed part
 
         """
         return b".".join(self.value.split(b".", 2)[:2])
 
     def verify_signature(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
+        key: Jwk | dict[str, Any] | Any,
         *,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> bool:
         """Verify the signature from this JwsCompact using a Jwk.
 
         Args:
           key: the Jwk to use to validate this signature
           alg: the alg to use, if there is only 1 allowed
           algs: the allowed algs, if here are several
```

### Comparing `jwskate-0.8.0/jwskate/jws/json.py` & `jwskate-0.9.0/jwskate/jws/json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implement the JWS JSON flat and general formats."""
-
 from __future__ import annotations
 
 from functools import cached_property
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Tuple, Union
+from typing import Any, Callable, Iterable, Mapping
 
 from binapy import BinaPy
 
 from jwskate.jwk.base import Jwk
 from jwskate.token import BaseJsonDict
 
 from .compact import JwsCompact
@@ -47,18 +46,18 @@
             content["header"] = self.header
         return JwsSignature(content)
 
     @classmethod
     def sign(
         cls,
         payload: bytes,
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        extra_protected_headers: Optional[Mapping[str, Any]] = None,
-        header: Optional[Any] = None,
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        extra_protected_headers: Mapping[str, Any] | None = None,
+        header: Any | None = None,
         **kwargs: Any,
     ) -> JwsJsonFlat:
         """Signs a payload into a JWS in JSON flat format.
 
         Args:
             payload: the data to sign.
             key: the key to use
@@ -112,18 +111,18 @@
             A `JwsCompact` with the same payload and signature.
 
         """
         return JwsCompact.from_parts(self.signed_part(), self.signature)
 
     def verify_signature(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
+        key: Jwk | dict[str, Any] | Any,
         *,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> bool:
         """Verify this JWS signature with a given key.
 
         Args:
             key: the key to use to validate this signature.
             alg: the signature alg, if only 1 is allowed.
             algs: the allowed signature algs, if there are several.
@@ -151,32 +150,33 @@
             raise AttributeError("This Jws JSON does not contain a 'payload' member")
         return BinaPy(payload).decode_from("b64u")
 
     @classmethod
     def sign(
         cls,
         payload: bytes,
-        *signature_parameters: Union[
-            Tuple[
-                Union[Jwk, Mapping[str, Any]],
+        *signature_parameters: (
+            tuple[
+                Jwk | Mapping[str, Any],
                 str,
-                Optional[Mapping[str, Any]],
-                Optional[Mapping[str, Any]],
-            ],
-            Tuple[
-                Union[Jwk, Mapping[str, Any]],
+                Mapping[str, Any] | None,
+                Mapping[str, Any] | None,
+            ]
+            | tuple[
+                Jwk | Mapping[str, Any],
                 str,
-                Optional[Mapping[str, Any]],
-            ],
-            Tuple[
-                Union[Jwk, Mapping[str, Any]],
+                Mapping[str, Any] | None,
+            ]
+            | tuple[
+                Jwk | Mapping[str, Any],
                 str,
-            ],
-            Union[Jwk, Mapping[str, Any]],
-        ],
+            ]
+            | Jwk
+            | Mapping[str, Any]
+        ),
     ) -> JwsJsonGeneral:
         """Sign a payload with several keys and return the resulting JWS in JSON general format.
 
         Args:
             payload: the data to sign
             *signature_parameters: each of those parameter can be:
                 - a `(jwk, alg, extra_protected_headers, header)` tuple
@@ -191,31 +191,32 @@
         """
         jws = cls({"payload": BinaPy(payload).to("b64u").ascii()})
         for parameters in signature_parameters:
             jws.add_signature(*parameters)
         return jws
 
     @cached_property
-    def signatures(self) -> List[JwsSignature]:
+    def signatures(self) -> list[JwsSignature]:
         """The list of `JwsSignature` from this JWS.
 
         Returns:
             The list of signatures from this JWS.
+
         """
         signatures = self.get("signatures")
         if signatures is None:
             raise AttributeError("This Jws JSON does not contain a 'signatures' member")
         return [JwsSignature(sig) for sig in signatures]
 
     def add_signature(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        extra_protected_headers: Optional[Mapping[str, Any]] = None,
-        header: Optional[Mapping[str, Any]] = None,
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        extra_protected_headers: Mapping[str, Any] | None = None,
+        header: Mapping[str, Any] | None = None,
     ) -> JwsJsonGeneral:
         """Add a new signature in this JWS.
 
         Args:
             key: the private key to use
             alg: the signature algorithm
             extra_protected_headers: additional headers to include, as a {key: value} mapping
@@ -230,15 +231,15 @@
             JwsSignature.sign(self.payload, key, alg, extra_protected_headers, header)
         )
         return self
 
     def signed_part(
         self,
         signature_chooser: Callable[
-            [List[JwsSignature]], JwsSignature
+            [list[JwsSignature]], JwsSignature
         ] = lambda sigs: sigs[0],
     ) -> bytes:
         """Return the signed part from a given signature.
 
         The signed part is a concatenation of the protected header from a specific signature, then the payload,
         separated by a dot (`.`).
         You can select the specific signature with the `signature_chooser` parameter.
@@ -253,15 +254,15 @@
         """
         signature = signature_chooser(self.signatures)
         return JwsSignature.assemble_signed_part(signature.protected, self.payload)
 
     def compact(
         self,
         signature_chooser: Callable[
-            [List[JwsSignature]], JwsSignature
+            [list[JwsSignature]], JwsSignature
         ] = lambda sigs: sigs[0],
     ) -> JwsCompact:
         """Create a compact JWS from a specific signature from this JWS.
 
         Args:
             signature_chooser: a callable that takes the list of signatures from this JWS as parameter and returns the choosen signature.
 
@@ -274,15 +275,15 @@
             JwsSignature.assemble_signed_part(signature.protected, self.payload),
             signature.signature,
         )
 
     def flatten(
         self,
         signature_chooser: Callable[
-            [List[JwsSignature]], JwsSignature
+            [list[JwsSignature]], JwsSignature
         ] = lambda sigs: sigs[0],
     ) -> JwsJsonFlat:
         """Create a JWS in JSON flat format from a specific signature from this JWS.
 
         Args:
             signature_chooser:  a callable that takes the list of signatures from this JWS as parameter and returns the choosen signature.
 
@@ -296,18 +297,18 @@
             protected=signature.protected,
             header=signature.header,
             signature=signature.signature,
         )
 
     def verify_signature(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
+        key: Jwk | dict[str, Any] | Any,
         *,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> bool:
         """Verify the signatures from this JWS.
 
         It will try to validate each signature with the given key, and returns `True` if at least one signature verifies.
         Args:
             key: the public key to use
             alg: the signature algorithm to use, if only 1 is allowed.
```

### Comparing `jwskate-0.8.0/jwskate/jws/signature.py` & `jwskate-0.9.0/jwskate/jws/signature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implement JWS signatures."""
-
 from __future__ import annotations
 
 from functools import cached_property
-from typing import Any, Dict, Iterable, Mapping, Optional, Type, TypeVar, Union
+from typing import Any, Iterable, Mapping, TypeVar
 
 from binapy import BinaPy
 
 from jwskate.jwk import Jwk, to_jwk
 from jwskate.token import BaseJsonDict
 
 S = TypeVar("S", bound="JwsSignature")
@@ -23,18 +22,18 @@
      - an unprotected header (as arbitrary JSON data)
      - optional extra JSON attributes
 
     """
 
     @classmethod
     def from_parts(
-        cls: Type[S],
+        cls: type[S],
         protected: Mapping[str, Any],
         signature: bytes,
-        header: Optional[Any],
+        header: Any | None,
         **kwargs: Any,
     ) -> S:
         """Initialize a JwsSignature based on the provided parts.
 
         Args:
           protected: the protected headers, as a key: value mapping
           signature: the raw signature value
@@ -51,15 +50,15 @@
             signature=BinaPy(signature).to("b64u").ascii(),
         )
         if header is not None:
             content["header"] = header
         return cls(content)
 
     @cached_property
-    def protected(self) -> Dict[str, Any]:
+    def protected(self) -> dict[str, Any]:
         """The protected header.
 
         Returns:
             the protected headers, as a `dict`.
 
         Raises:
             AttributeError: if this signature doesn't have protected headers.
@@ -94,20 +93,20 @@
         signature = self.get("signature")
         if signature is None:
             raise AttributeError("This Jws JSON does not contain a 'signature' member")
         return BinaPy(signature).decode_from("b64u")
 
     @classmethod
     def sign(
-        cls: Type[S],
+        cls: type[S],
         payload: bytes,
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        extra_protected_headers: Optional[Mapping[str, Any]] = None,
-        header: Optional[Any] = None,
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        extra_protected_headers: Mapping[str, Any] | None = None,
+        header: Any | None = None,
         **kwargs: Any,
     ) -> S:
         """Sign a payload and return the generated JWS signature.
 
         Args:
           payload: the raw data to sign
           key: the signature key to use
@@ -131,15 +130,15 @@
         signature = key.sign(signed_part, alg=alg)
         return cls.from_parts(
             protected=headers, signature=signature, header=header, **kwargs
         )
 
     @classmethod
     def assemble_signed_part(
-        cls, headers: Dict[str, Any], payload: Union[bytes, str]
+        cls, headers: dict[str, Any], payload: bytes | str
     ) -> bytes:
         """Assemble the protected header and payload to sign, as specified in.
 
         [RFC7515
         $5.1](https://datatracker.ietf.org/doc/html/rfc7515#section-5.1).
 
         Args:
@@ -156,18 +155,18 @@
                 BinaPy(payload).to("b64u"),
             )
         )
 
     def verify(
         self,
         payload: bytes,
-        key: Union[Jwk, Dict[str, Any], Any],
+        key: Jwk | dict[str, Any] | Any,
         *,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> bool:
         """Verify this signature against the given payload using the provided key.
 
         Args:
           payload: the raw payload
           key: the validation key to use
           alg: the signature alg t if only 1 is allowed
```

### Comparing `jwskate-0.8.0/jwskate/jwt/base.py` & `jwskate-0.9.0/jwskate/jwt/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This modules contains the `Jwt` base class."""
-
 from __future__ import annotations
 
 from datetime import datetime, timezone
-from typing import TYPE_CHECKING, Any, Dict, Iterable, Optional, Union
+from typing import TYPE_CHECKING, Any, Iterable
 
 from binapy import BinaPy
 
 from jwskate.jwe import JweCompact
 from jwskate.jwk import Jwk, to_jwk
 from jwskate.token import BaseCompactToken
 
@@ -18,15 +17,15 @@
 class InvalidJwt(ValueError):
     """Raised when an invalid Jwt is parsed."""
 
 
 class Jwt(BaseCompactToken):
     """Represents a Json Web Token."""
 
-    def __new__(cls, value: Union[bytes, str], max_size: int = 16 * 1024) -> Union[SignedJwt, JweCompact, Jwt]:  # type: ignore[misc]
+    def __new__(cls, value: bytes | str, max_size: int = 16 * 1024) -> SignedJwt | JweCompact | Jwt:  # type: ignore[misc]
         """Allow parsing both Signed and Encrypted JWTs.
 
         This returns the appropriate subclass or instance depending on the number of dots (.) in the serialized JWT.
 
         Args:
             value: the token value
             max_size: maximum allowed size for the token
@@ -46,66 +45,72 @@
                 return JweCompact(value, max_size)
 
         return super().__new__(cls)
 
     @classmethod
     def sign(
         cls,
-        claims: Dict[str, Any],
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        extra_headers: Optional[Dict[str, Any]] = None,
+        claims: dict[str, Any],
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        typ: str | None = "JWT",
+        extra_headers: dict[str, Any] | None = None,
     ) -> SignedJwt:
         """Sign a JSON payload with a private key and return the resulting `SignedJwt`.
 
         This method cannot generate a token without a signature. If you want to use an unsigned token (with alg=none),
         use `.unprotected()` instead.
 
         Args:
           claims: the payload to sign
           key: the key to use for signing
           alg: the alg to use for signing
+          typ: typ (token type) header to include. If `None`, do not include this header.
           extra_headers: additional headers to include in the Jwt
 
         Returns:
           the resulting token
+
         """
         key = to_jwk(key)
 
         alg = alg or key.get("alg")
 
         if alg is None:
             raise ValueError("a signing alg is required")
 
         extra_headers = extra_headers or {}
         headers = dict(alg=alg, **extra_headers)
+        if typ:
+            headers["typ"] = typ
         if key.kid:
             headers["kid"] = key.kid
 
         return cls.sign_arbitrary(claims=claims, headers=headers, key=key, alg=alg)
 
     @classmethod
     def sign_arbitrary(
         self,
-        claims: Dict[str, Any],
-        headers: Dict[str, Any],
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
+        claims: dict[str, Any],
+        headers: dict[str, Any],
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
     ) -> SignedJwt:
         """Sign provided headers and claims with a private key and return the resulting `SignedJwt`.
 
         This does not check the consistency between headers, key, alg and kid.
         DO NOT USE THIS METHOD UNLESS YOU KNOW WHAT YOU ARE DOING!!!
         Use `Jwt.sign()` to make sure you are signing tokens properly.
 
         Args:
              claims: the payload to sign
              headers: the headers to sign
              key: the key to use for signing
              alg: the alg to use for signing
+
         """
         from .signed import SignedJwt
 
         key = to_jwk(key)
 
         alg = alg or key.get("alg")
 
@@ -117,49 +122,53 @@
         signed_value = b".".join((headers_part, claims_part))
         signature = key.sign(signed_value, alg=alg).to("b64u")
         return SignedJwt(b".".join((signed_value, signature)))
 
     @classmethod
     def unprotected(
         cls,
-        claims: Dict[str, Any],
-        extra_headers: Optional[Dict[str, Any]] = None,
+        claims: dict[str, Any],
+        typ: str | None = "JWT",
+        extra_headers: dict[str, Any] | None = None,
     ) -> SignedJwt:
         """Generate a JWT that is not signed and not encrypted (with alg=none).
 
         Args:
           claims: the claims to set in the token.
+          typ: typ (token type) header to include. If `None`, do not include this header.
           extra_headers: additional headers to insert in the token.
 
         Returns:
             the resulting token
 
         """
         from .signed import SignedJwt
 
         headers = dict(extra_headers or {}, alg="none")
+        if typ:
+            headers["typ"] = typ
 
         headers_part = BinaPy.serialize_to("json", headers).to("b64u")
         claims_part = BinaPy.serialize_to("json", claims).to("b64u")
         signed_value = b".".join((headers_part, claims_part))
         signature = b""
         return SignedJwt(b".".join((signed_value, signature)))
 
     @classmethod
     def sign_and_encrypt(
         cls,
-        claims: Dict[str, Any],
-        sign_key: Union[Jwk, Dict[str, Any], Any],
-        enc_key: Union[Jwk, Dict[str, Any], Any],
+        claims: dict[str, Any],
+        sign_key: Jwk | dict[str, Any] | Any,
+        enc_key: Jwk | dict[str, Any] | Any,
         enc: str,
         *,
-        sign_alg: Optional[str] = None,
-        enc_alg: Optional[str] = None,
-        sign_extra_headers: Optional[Dict[str, Any]] = None,
-        enc_extra_headers: Optional[Dict[str, Any]] = None,
+        sign_alg: str | None = None,
+        enc_alg: str | None = None,
+        sign_extra_headers: dict[str, Any] | None = None,
+        enc_extra_headers: dict[str, Any] | None = None,
     ) -> JweCompact:
         """Sign a JWT, then encrypt it as JWE payload.
 
         This is a convenience method to do both the signing and encryption, in appropriate order.
 
         Args:
           claims: the payload to encrypt
@@ -184,15 +193,15 @@
         jwe = JweCompact.encrypt(
             inner_jwt, enc_key, enc=enc, alg=enc_alg, extra_headers=enc_extra_headers
         )
         return jwe
 
     @classmethod
     def decrypt_nested_jwt(
-        cls, jwe: Union[str, JweCompact], key: Union[Jwk, Dict[str, Any], Any]
+        cls, jwe: str | JweCompact, key: Jwk | dict[str, Any] | Any
     ) -> Jwt:
         """Decrypt a JWE that contains a nested JWT.
 
         It will return a [Jwt] instance for the inner JWT.
 
         Args:
             jwe: the JWE containing a nested Token
@@ -209,19 +218,19 @@
             jwe = JweCompact(jwe)
         cleartext = jwe.decrypt(key)
         return Jwt(cleartext)
 
     @classmethod
     def decrypt_and_verify(
         cls,
-        jwt: Union[str, JweCompact],
-        enc_key: Union[Jwk, Dict[str, Any], Any],
-        sig_key: Union[Jwk, Dict[str, Any], None, Any],
-        sig_alg: Optional[str] = None,
-        sig_algs: Optional[Iterable[str]] = None,
+        jwt: str | JweCompact,
+        enc_key: Jwk | dict[str, Any] | Any,
+        sig_key: Jwk | dict[str, Any] | None | Any,
+        sig_alg: str | None = None,
+        sig_algs: Iterable[str] | None = None,
     ) -> SignedJwt:
         """Decrypt then verify the signature of a JWT nested in a JWE.
 
         This can only be used with signed then encrypted Jwt, such as those produce by `Jwt.sign_and_encrypt()`.
 
         Args:
             jwt: the JWE containing a nested signed JWT
@@ -277,9 +286,10 @@
         Returned datetime is always in the UTC timezone.
 
         Args:
             timestamp: a timestamp from a JWT token
 
         Returns:
             the corresponding `datetime` in UTC timezone
+
         """
         return datetime.fromtimestamp(timestamp, tz=timezone.utc)
```

### Comparing `jwskate-0.8.0/jwskate/jwt/signed.py` & `jwskate-0.9.0/jwskate/jwt/signed.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This modules contains classes and utilities to generate and validate signed JWT."""
+from __future__ import annotations
 
 from datetime import datetime, timedelta, timezone
 from functools import cached_property
-from typing import Any, Dict, Iterable, List, Optional, Union
+from typing import Any, Iterable
 
 from binapy import BinaPy
 
 from jwskate.jwk import Jwk, to_jwk
 
 from .base import InvalidJwt, Jwt
 
@@ -31,15 +32,15 @@
     To sign a JWT, use [Jwt.sign][jwskate.jwt.Jwt.sign].
 
     Args:
         value: the token value.
 
     """
 
-    def __init__(self, value: Union[bytes, str]) -> None:
+    def __init__(self, value: bytes | str) -> None:
         super().__init__(value)
 
         if self.value.count(b".") != 2:
             raise InvalidJwt(
                 "A JWT must contain a header, a payload and a signature, separated by dots",
                 value,
             )
@@ -76,17 +77,17 @@
           the signed part as bytes
 
         """
         return b".".join(self.value.split(b".", 2)[:2])
 
     def verify_signature(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        key: Jwk | dict[str, Any] | Any,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
     ) -> bool:
         """Verify this JWT signature using a given key and algorithm(s).
 
         Args:
           key: the private Jwk to use to verify the signature
           alg: the alg to use to verify the signature, if only 1 is allowed
           algs: the allowed signature algs, if there are several
@@ -97,68 +98,71 @@
         """
         key = to_jwk(key)
 
         return key.verify(
             data=self.signed_part, signature=self.signature, alg=alg, algs=algs
         )
 
-    def is_expired(self, leeway: int = 0) -> Optional[bool]:
+    def is_expired(self, leeway: int = 0) -> bool | None:
         """Check if this token is expired, based on its `exp` claim.
 
         Args:
             leeway: additional number of seconds for leeway.
 
         Returns:
             `True` if the token is expired, `False` if it's not, `None` if there is no `exp` claim.
+
         """
         exp = self.expires_at
         if exp is None:
             return None
         return exp < (datetime.now(timezone.utc) + timedelta(seconds=leeway))
 
     @cached_property
-    def expires_at(self) -> Optional[datetime]:
+    def expires_at(self) -> datetime | None:
         """Get the *Expires At* (`exp`) date from this token.
 
         Returns:
           a `datetime` initialized from the `exp` claim, or `None` if there is no `exp` claim
 
         Raises:
             AttributeError: if the `exp` claim cannot be parsed to a date
+
         """
         exp = self.get_claim("exp")
         if not exp:
             return None
         try:
             exp_dt = Jwt.timestamp_to_datetime(exp)
             return exp_dt
         except (TypeError, OSError):
             raise AttributeError("invalid `exp `claim", exp)
 
     @cached_property
-    def issued_at(self) -> Optional[datetime]:
+    def issued_at(self) -> datetime | None:
         """Get the *Issued At* (`iat`) date from this token.
 
         Returns:
           a `datetime` initialized from the `iat` claim, or `None` if there is no `iat` claim
 
         Raises:
             AttributeError: if the `iss` claim cannot be parsed to a date
+
         """
         iat = self.get_claim("iat")
         if not iat:
             return None
         try:
             iat_dt = Jwt.timestamp_to_datetime(iat)
             return iat_dt
         except (TypeError, OSError):
             raise AttributeError("invalid `iat `claim", iat)
 
     @cached_property
-    def not_before(self) -> Optional[datetime]:
+    def not_before(self) -> datetime | None:
         """Get the *Not Before* (nbf) date from this token.
 
         Returns:
           a `datetime` initialized from the `nbf` claim, or `None` if there is no `nbf` claim
 
         Raises:
             AttributeError: if the `nbf` claim cannot be parsed to a date
@@ -170,73 +174,77 @@
         try:
             nbf_dt = Jwt.timestamp_to_datetime(nbf)
             return nbf_dt
         except (TypeError, OSError):
             raise AttributeError("invalid `nbf `claim", nbf)
 
     @cached_property
-    def issuer(self) -> Optional[str]:
+    def issuer(self) -> str | None:
         """Get the *Issuer* (`iss`) claim from this token.
 
         Returns:
           the issuer, as `str`, or `None` if there is no `ìss` claim
 
         Raises:
             AttributeError: if the `ìss` claim value is not a string
+
         """
         iss = self.get_claim("iss")
         if iss is None or isinstance(iss, str):
             return iss
         raise AttributeError("iss has an unexpected type", type(iss))
 
     @cached_property
-    def audiences(self) -> List[str]:
+    def audiences(self) -> list[str]:
         """Get the *Audience(s)* (`aud`) claim from this token.
 
         If this token has a single audience, this will return a `list` anyway.
 
         Returns:
             the list of audiences from this token, from the `aud` claim.
 
         Raises:
             AttributeError: if the audience is an unexpected type
+
         """
         aud = self.get_claim("aud")
         if aud is None:
             return []
         if isinstance(aud, str):
             return [aud]
         if isinstance(aud, list):
             return aud
         raise AttributeError("aud has an unexpected type", type(aud))
 
     @cached_property
-    def subject(self) -> Optional[str]:
+    def subject(self) -> str | None:
         """Get the *Subject* (`sub`) from this token.
 
         Returns:
           the subject, as `str`, or `None` if there is no `sub` claim
 
         Raises:
             AttributeError: if the `sub` value is not a string
+
         """
         sub = self.get_claim("sub")
         if sub is None or isinstance(sub, str):
             return sub
         raise AttributeError("sub has an unexpected type", type(sub))
 
     @cached_property
-    def jwt_token_id(self) -> Optional[str]:
+    def jwt_token_id(self) -> str | None:
         """Get the *JWT Token ID* (`jti`) from this token.
 
         Returns:
           the token identifier, as `str`, or `None` if there is no `jti` claim
 
         Raises:
           AttributeError: if the `jti` value is not a string
+
         """
         jti = self.get_claim("jti")
         if jti is None or isinstance(jti, str):
             return jti
         raise AttributeError("jti has an unexpected type", type(jti))
 
     def get_claim(self, key: str, default: Any = None) -> Any:
@@ -283,33 +291,35 @@
         return value
 
     def __str__(self) -> str:
         """Return the Jwt serialized value, as `str`.
 
         Returns:
             the serialized token value.
+
         """
         return self.value.decode()
 
     def __bytes__(self) -> bytes:
         """Return the Jwt serialized value, as `bytes`.
 
         Returns:
             the serialized token value.
+
         """
         return self.value
 
     def validate(
         self,
-        key: Union[Jwk, Dict[str, Any], Any],
+        key: Jwk | dict[str, Any] | Any,
         *,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
-        issuer: Optional[str] = None,
-        audience: Union[None, str] = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
+        issuer: str | None = None,
+        audience: None | str = None,
         check_exp: bool = True,
         **kwargs: Any,
     ) -> None:
         """Validate a `SignedJwt` signature and expected claims.
 
         This verifies the signature using the provided `jwk` and `alg`, then checks the token issuer, audience and expiration date.
         This can also check custom claims using extra `kwargs`, whose values can be:
@@ -329,14 +339,15 @@
         Returns:
           Raises exceptions if any validation check fails.
 
         Raises:
           InvalidSignature: if the signature is not valid
           InvalidClaim: if a claim doesn't validate
           ExpiredJwt: if the expiration date is passed
+
         """
         if not self.verify_signature(key, alg, algs):
             raise InvalidSignature("Signature is not valid.")
 
         if issuer is not None:
             if self.issuer != issuer:
                 raise InvalidClaim("iss", "Unexpected issuer", self.issuer)
```

### Comparing `jwskate-0.8.0/jwskate/jwt/signer.py` & `jwskate-0.9.0/jwskate/jwt/signer.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 assert isinstance(signer.jwk, ECJwk) and signer.jwk.is_private
 ```
 
 """
 from __future__ import annotations
 
 import uuid
-from typing import Any, Callable, Dict, Iterable, Optional, Union
+from typing import Any, Callable, Iterable
 
 from jwskate.jwk import Jwk
 
 from .base import Jwt
 from .signed import SignedJwt
 from .verifier import JwtVerifier
 
@@ -63,32 +63,32 @@
 
     """
 
     def __init__(
         self,
         issuer: str,
         jwk: Jwk,
-        alg: Optional[str] = None,
+        alg: str | None = None,
         default_lifetime: int = 60,
-        default_leeway: Optional[int] = None,
+        default_leeway: int | None = None,
     ):
         self.issuer = issuer
         self.jwk = jwk
         self.alg = jwk.alg or alg
         self.default_lifetime = default_lifetime
         self.default_leeway = default_leeway
 
     def sign(
         self,
-        subject: Optional[str] = None,
-        audience: Union[str, Iterable[str], None] = None,
-        extra_claims: Optional[Dict[str, Any]] = None,
-        extra_headers: Optional[Dict[str, Any]] = None,
-        lifetime: Optional[int] = None,
-        leeway: Optional[int] = None,
+        subject: str | None = None,
+        audience: str | Iterable[str] | None = None,
+        extra_claims: dict[str, Any] | None = None,
+        extra_headers: dict[str, Any] | None = None,
+        lifetime: int | None = None,
+        leeway: int | None = None,
     ) -> SignedJwt:
         """Sign a Jwt.
 
         Claim 'issuer' will have the value defined at initialization time. Claim `iat`, `nbf` and `exp` will reflect
         the current time when the token is signed. `exp` includes `lifetime` seconds in the future, and `nbf`
         includes `leeway` seconds in the past.
 
@@ -140,16 +140,16 @@
 
     @classmethod
     def with_random_key(
         cls,
         issuer: str,
         alg: str,
         default_lifetime: int = 60,
-        default_leeway: Optional[int] = None,
-        kid: Optional[str] = None,
+        default_leeway: int | None = None,
+        kid: str | None = None,
     ) -> JwtSigner:
         """Initialize a JwtSigner with a randomly generated key.
 
         Args:
             issuer: the issuer identifier
             alg: the signing alg to use
             default_lifetime: lifetime for generated tokens expiration date (`exp` claim)
@@ -162,15 +162,15 @@
         """
         jwk = Jwk.generate_for_alg(alg, kid=kid).with_kid_thumbprint()
         return cls(issuer, jwk, alg, default_lifetime, default_leeway)
 
     def verifier(
         self,
         audience: str,
-        verifiers: Optional[Iterable[Callable[[SignedJwt], None]]] = None,
+        verifiers: Iterable[Callable[[SignedJwt], None]] | None = None,
         **kwargs: Any,
     ) -> JwtVerifier:
         """Return the matching JwtVerifier, initialized with the public key."""
         return JwtVerifier(
             issuer=self.issuer,
             jwkset=self.jwk.public_jwk().as_jwks(),
             alg=self.alg,
```

### Comparing `jwskate-0.8.0/jwskate/jwt/verifier.py` & `jwskate-0.9.0/jwskate/jwt/verifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """High-Level facility to verify JWT tokens signature, validity dates, issuer, audiences, etc."""
-from typing import Any, Callable, Dict, Iterable, Optional, Union
+from __future__ import annotations
+
+from typing import Any, Callable, Iterable
 
 from jwskate import Jwk, JwkSet
 
 from .signed import ExpiredJwt, InvalidClaim, InvalidSignature, SignedJwt
 
 
 class JwtVerifier:
@@ -38,22 +40,22 @@
             print("token failed verification :(")
         ```
 
     """
 
     def __init__(
         self,
-        jwkset: Union[JwkSet, Jwk, Dict[str, Any]],
+        jwkset: JwkSet | Jwk | dict[str, Any],
         *,
-        issuer: Optional[str],
-        audience: Optional[str] = None,
-        alg: Optional[str] = None,
-        algs: Optional[Iterable[str]] = None,
+        issuer: str | None,
+        audience: str | None = None,
+        alg: str | None = None,
+        algs: Iterable[str] | None = None,
         leeway: int = 10,
-        verifiers: Optional[Iterable[Callable[[SignedJwt], None]]] = None,
+        verifiers: Iterable[Callable[[SignedJwt], None]] | None = None,
     ) -> None:
         if isinstance(jwkset, Jwk):
             jwkset = jwkset.as_jwks()
         elif isinstance(jwkset, dict):
             if "keys" in jwkset:
                 jwkset = JwkSet(jwkset)
             else:
@@ -69,15 +71,15 @@
         self.jwkset = jwkset
         self.audience = audience
         self.alg = alg
         self.algs = algs
         self.leeway = leeway
         self.verifiers = list(verifiers) if verifiers else []
 
-    def verify(self, jwt: Union[SignedJwt, str]) -> None:
+    def verify(self, jwt: SignedJwt | str) -> None:
         """Verify a given JWT token.
 
         This checks the token signature, issuer, audience and expiration date, plus any custom verification,
         as configured at init time.
 
         Args:
             jwt: the JWT token to verify
```

### Comparing `jwskate-0.8.0/jwskate/token.py` & `jwskate-0.9.0/jwskate/token.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 """This module contains base classes for all tokens types handled by `jwskate`."""
+from __future__ import annotations
+
 import json
 from functools import cached_property
-from typing import Any, Dict, Type, TypeVar, Union
+from typing import Any, Dict, TypeVar
 
 
 class BaseCompactToken:
     """Base class for all tokens in Compact representation.
 
     This includes JWS, JWE, and JWT tokens.
 
     Args:
         value: the string or bytes representation of this JWS/JWE/JWT
         max_size: if the JWT length is larger than this value, raise a `ValueError`.
             This is to avoid JSON deserialization vulnerabilities.
 
     """
 
-    def __init__(self, value: Union[bytes, str], max_size: int = 16 * 1024):
+    def __init__(self, value: bytes | str, max_size: int = 16 * 1024):
         if len(value) > max_size:
             raise ValueError(
                 f"This JWT size exceeds {max_size} bytes, which is abnormally big. "
                 "This size limit is made to avoid potential JSON deserialization vulnerabilities or issues. "
                 "You can increase this limit by passing a different `max_size` value as parameter."
             )
 
         if isinstance(value, str):
             value = value.encode("ascii")
 
         value = b"".join(value.split())
 
         self.value = value
-        self.headers: Dict[str, Any]
+        self.headers: dict[str, Any]
 
     def __eq__(self, other: Any) -> bool:
         """Check that a Jwt is equal to another.
 
         Works with other instances of `Jwt`, or with `str` or `bytes`.
 
         Args:
@@ -136,15 +138,15 @@
 D = TypeVar("D", bound="BaseJsonDict")
 
 
 class BaseJsonDict(Dict[str, Any]):
     """Base class Jwk and tokens in JSON representation."""
 
     @classmethod
-    def from_json(cls: Type[D], j: str) -> D:
+    def from_json(cls: type[D], j: str) -> D:
         """Initialize an object based on a string containing a JSON representation.
 
         Args:
           j: the JSON to parse, still serialized
 
         Returns:
             the resulting object
```

### Comparing `jwskate-0.8.0/pyproject.toml` & `jwskate-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,61 @@
 [tool]
 [tool.poetry]
 name = "jwskate"
-version = "0.8.0"
+version = "0.9.0"
 homepage = "https://github.com/guillp/jwskate"
 description = "A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
-    'Development Status :: 3 - Alpha',
+    'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
+    'Topic :: Security',
     'License :: OSI Approved :: MIT License',
-    'Natural Language :: English',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 packages = [
     { include = "jwskate" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.8"
 cryptography = ">=3.4"
 typing-extensions = ">=4.3.0"
-binapy = ">=0.6.1"
+binapy = ">=0.7.0"
 
 [tool.poetry.dev-dependencies]
-black  = ">=23.3"
+black  = ">=23.7"
 coverage = ">=7.2.3"
 freezegun = ">=1.2.2"
 isort  = ">=5.12"
 jwcrypto = ">=1.0"
 livereload = ">=2.6"
-mypy = ">=1.2"
+mypy = ">=1.4.1"
 mkdocs  = ">=1.4.2"
 mkdocstrings = { version = ">=0.21.2", extras = ["python"] }
 mkdocs-autorefs = ">=0.4"
-mkdocs-include-markdown-plugin  = ">=4.0.4"
-mkdocs-material  = ">=9.1.6"
+mkdocs-material  = ">=9.1.19"
 mkdocs-material-extensions  = ">=1.1"
-pip  = ">=22.0"
+pip  = ">=23.2.1"
 pre-commit = ">=3.2.2"
-pytest  = ">=7.3"
+pytest  = ">=7.4.0"
 pytest-cov  = ">=4.0"
 pytest-mypy = ">=0.10"
 toml = ">=0.10"
 tomli = ">=2.0.1"
-tox  = ">=4.5.1"
+tox  = ">=4.6.4"
 types-cryptography = ">=3.3"
-virtualenv  = ">=20.14.1"
+virtualenv  = ">=20.24.1"
 
 [tool.poetry.extras]
 test = ["pytest", "pytest-cov", "jwcrypto", "freezegun"]
 doc = ["mkdocs"]
 
 
 [build-system]
```

### Comparing `jwskate-0.8.0/tests/conftest.py` & `jwskate-0.9.0/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common fixtures for all tests."""
+from __future__ import annotations
 
 import pytest
 
 from jwskate import Jwk
 
 
 @pytest.fixture()
```

### Comparing `jwskate-0.8.0/tests/test_jwa/test_base.py` & `jwskate-0.9.0/tests/test_jwa/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type
+from __future__ import annotations
 
 import pytest
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from jwskate import (
     A128CBC_HS256,
     A128GCM,
@@ -102,13 +102,13 @@
         RsaEsOaep,
         RsaEsOaepSha256,
         RsaEsOaepSha384,
         RsaEsOaepSha512,
         RsaEsPcks1v1_5,
     ),
 )
-def test_init_with_random_key(alg_class: Type[BaseAlg]) -> None:
+def test_init_with_random_key(alg_class: type[BaseAlg]) -> None:
     alg = alg_class.with_random_key()
     assert isinstance(alg, alg_class)
     if issubclass(alg_class, BaseAsymmetricAlg):
         assert isinstance(alg, BaseAsymmetricAlg)
         assert isinstance(alg.public_key(), alg_class.public_key_class)
```

### Comparing `jwskate-0.8.0/tests/test_jwa/test_encryption.py` & `jwskate-0.9.0/tests/test_jwa/test_encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Tests for jwskate.jwa.encryption submodule."""
+from __future__ import annotations
 
 import pytest
 
 from jwskate import (
     A128CBC_HS256,
     A128GCM,
     A192CBC_HS384,
```

### Comparing `jwskate-0.8.0/tests/test_jwa/test_examples.py` & `jwskate-0.9.0/tests/test_jwa/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Tests for the jwkskate.jwa submodule."""
+from __future__ import annotations
+
 from binapy import BinaPy
 
 from jwskate import A128CBC_HS256, A192CBC_HS384, EcdhEs, Jwk
 
 
 def test_aes_128_hmac_sha256() -> None:
     """Test derived from [RFC7518](https://datatracker.ietf.org/doc/html/rfc7518#appendix-B.1)."""
```

### Comparing `jwskate-0.8.0/tests/test_jwa/test_key_mgmt.py` & `jwskate-0.9.0/tests/test_jwa/test_key_mgmt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Tests for jwskate.jwa.key_mgmt submodule."""
-from typing import Type, Union
+from __future__ import annotations
 
 import pytest
 from cryptography.hazmat.primitives.asymmetric import ec, x448, x25519
 
 from jwskate import BasePbes2, EcdhEs
 
 
@@ -14,19 +14,19 @@
         lambda: ec.generate_private_key(ec.SECP384R1()),
         lambda: ec.generate_private_key(ec.SECP521R1()),
         x25519.X25519PrivateKey.generate,
         x448.X448PrivateKey.generate,
     ],
 )
 def test_ecdhes(
-    key_gen: Union[
-        Type[ec.EllipticCurvePrivateKey],
-        Type[x25519.X25519PrivateKey],
-        Type[x448.X448PrivateKey],
-    ]
+    key_gen: (
+        type[ec.EllipticCurvePrivateKey]
+        | type[x25519.X25519PrivateKey]
+        | type[x448.X448PrivateKey]
+    ),
 ) -> None:
     private_key = key_gen()
     sender_ecdhes = EcdhEs(private_key.public_key())
     epk = sender_ecdhes.generate_ephemeral_key()
     assert isinstance(epk, private_key.__class__)
     sender_key = sender_ecdhes.sender_key(epk, alg="A128GCM", key_size=128)
```

### Comparing `jwskate-0.8.0/tests/test_jwe.py` & `jwskate-0.9.0/tests/test_jwe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import SupportsBytes, Union
+from __future__ import annotations
+
+from typing import SupportsBytes
 
 import pytest
 
 import jwskate.jwa
 from jwskate import (
     P_521,
     ECJwk,
@@ -422,15 +424,15 @@
         return alg
     pytest.skip(f"Encryption alg {alg} is not supported yet!")
 
 
 @pytest.fixture(
     scope="module",
     params=[
-        'pAvkcJv!$N8HtIuf3W@KaF&2Gv"EAD/BK[_FEoLIuvMS*aG0tm4,.?'.encode(),
+        b'pAvkcJv!$N8HtIuf3W@KaF&2Gv"EAD/BK[_FEoLIuvMS*aG0tm4,.?',
     ],
 )
 def password(request: pytest.FixtureRequest) -> bytes:
     return request.param  # type: ignore[no-any-return]
 
 
 @pytest.fixture(scope="module")
@@ -445,15 +447,15 @@
     okp_x448_private_jwk: Jwk,
     symmetric_128_encryption_jwk: Jwk,
     symmetric_192_encryption_jwk: Jwk,
     symmetric_256_encryption_jwk: Jwk,
     symmetric_384_encryption_jwk: Jwk,
     symmetric_512_encryption_jwk: Jwk,
     password: bytes,
-) -> Union[Jwk, bytes]:
+) -> Jwk | bytes:
     if key_management_alg == "dir":
         for key in (
             symmetric_128_encryption_jwk,
             symmetric_192_encryption_jwk,
             symmetric_256_encryption_jwk,
             symmetric_384_encryption_jwk,
             symmetric_512_encryption_jwk,
@@ -481,27 +483,27 @@
             if key_management_alg in key.supported_key_management_algorithms():
                 return key
 
     assert False, f"No key supports this Key Management alg: {key_management_alg}"
 
 
 @pytest.fixture(scope="module")
-def encryption_jwk(decryption_jwk: Union[Jwk, bytes]) -> Union[Jwk, bytes]:
+def encryption_jwk(decryption_jwk: Jwk | bytes) -> Jwk | bytes:
     if isinstance(decryption_jwk, SymmetricJwk):
         return decryption_jwk
     elif isinstance(decryption_jwk, bytes):
         return decryption_jwk
 
     return decryption_jwk.public_jwk()
 
 
 @pytest.fixture(scope="module")
 def encrypted_jwe(
     encryption_plaintext: SupportsBytes,
-    encryption_jwk: Union[Jwk, SupportsBytes],
+    encryption_jwk: Jwk | SupportsBytes,
     key_management_alg: str,
     encryption_alg: str,
 ) -> JweCompact:
     if isinstance(encryption_jwk, Jwk):
         jwe = JweCompact.encrypt(
             plaintext=encryption_plaintext,
             key=encryption_jwk,
@@ -529,15 +531,15 @@
 
     def __bytes__(self) -> bytes:  # noqa: D105
         return self.payload
 
 
 def test_supportsbytes(
     encryption_plaintext: bytes,
-    encryption_jwk: Union[Jwk, SupportsBytes],
+    encryption_jwk: Jwk | SupportsBytes,
     key_management_alg: str,
     encryption_alg: str,
     encrypted_jwe: JweCompact,
     decryption_jwk: Jwk,
 ) -> None:
     if isinstance(encryption_jwk, Jwk):
         jwe = JweCompact.encrypt(
@@ -571,15 +573,15 @@
             == encryption_plaintext
         )
 
 
 def test_decrypt(
     encryption_plaintext: bytes,
     encrypted_jwe: JweCompact,
-    decryption_jwk: Union[Jwk, bytes],
+    decryption_jwk: Jwk | bytes,
     key_management_alg: str,
     encryption_alg: str,
 ) -> None:
     assert encrypted_jwe.alg == key_management_alg
     assert encrypted_jwe.enc == encryption_alg
     if isinstance(decryption_jwk, Jwk):
         assert encrypted_jwe.decrypt(decryption_jwk) == encryption_plaintext
@@ -600,14 +602,15 @@
 
     Args:
         encryption_plaintext: the expected plaintext
         encrypted_jwe: the Jwe encrypted by jwskate to decrypt
         decryption_jwk: the Jwk containing the decryption key
         key_management_alg: the key management alg
         encryption_alg: the encryption alg
+
     """
     import jwcrypto.jwe  # type: ignore[import]
     import jwcrypto.jwk  # type: ignore[import]
     from jwcrypto.common import InvalidJWEOperation, json_encode  # type: ignore[import]
 
     if key_management_alg in JWCRYPTO_UNSUPPORTED_ALGS:
         pytest.skip(f"jwcrypto doesn't support key management alg {key_management_alg}")
@@ -639,14 +642,15 @@
         encryption_plaintext: the plaintext to encrypt
         encryption_jwk: the Jwk to use to for encryption
         key_management_alg: the key management alg
         encryption_alg: the encryption alg
 
     Returns:
         a JWE token
+
     """
     import jwcrypto.jwe
     import jwcrypto.jwk
     from jwcrypto.common import json_encode
 
     if key_management_alg in JWCRYPTO_UNSUPPORTED_ALGS:
         pytest.skip(f"jwcrypto doesn't support key management alg {key_management_alg}")
@@ -679,14 +683,15 @@
 
     Args:
         encryption_plaintext: the plaintext
         jwcrypto_encrypted_jwe: the JWE to validate
         decryption_jwk: the decryption key
         key_management_alg: the key management alg
         encryption_alg: the encryption alg
+
     """
     jwe = JweCompact(jwcrypto_encrypted_jwe)
     assert jwe.alg == key_management_alg
     assert jwe.enc == encryption_alg
     try:
         assert jwe.decrypt(decryption_jwk) == encryption_plaintext
     except Exception:
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_alg.py` & `jwskate-0.9.0/tests/test_jwk/test_alg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from jwskate import (
     ExpectedAlgRequired,
     MismatchingAlg,
     RSAJwk,
     UnsupportedAlg,
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_ec.py` & `jwskate-0.9.0/tests/test_jwk/test_ec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from cryptography.hazmat.primitives.asymmetric import ec
 
 from jwskate import (
     A128CBC_HS256,
     EcdhEs,
     ECJwk,
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_generate.py` & `jwskate-0.9.0/tests/test_jwk/test_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
+
 import secrets
 import warnings
-from typing import Dict
 
 import pytest
 
 from jwskate import (
     P_521,
     EncryptionAlgs,
     ExpectedAlgRequired,
@@ -94,15 +95,15 @@
     (
         (KeyTypes.EC, {"crv": "P-256"}),
         (KeyTypes.OCT, {}),
         (KeyTypes.RSA, {}),
         (KeyTypes.OKP, {"crv": "Ed25519"}),
     ),
 )
-def test_generate_for_kty(kty: str, kwargs: Dict[str, str]) -> None:
+def test_generate_for_kty(kty: str, kwargs: dict[str, str]) -> None:
     jwk = Jwk.generate_for_kty(kty, **kwargs)
     assert jwk.kty == kty
 
 
 def test_generate() -> None:
     for alg in SignatureAlgs.ALL | KeyManagementAlgs.ALL_KEY_BASED | EncryptionAlgs.ALL:
         assert Jwk.generate(alg=alg).alg == alg
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_jwk.py` & `jwskate-0.9.0/tests/test_jwk/test_jwk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
+
 import secrets
-from typing import Tuple
 
 import pytest
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from jwskate import (
     A128GCM,
     ES256,
@@ -176,15 +177,15 @@
         ("RSA", ("sign",), ("verify",)),
         ("RSA", ("unwrapKey",), ("wrapKey",)),
         ("oct", ("sign",), ("verify",)),
         ("oct", ("unwrapKey",), ("wrapKey",)),
     ],
 )
 def test_key_ops_without_alg(
-    kty: str, private_key_ops: Tuple[str], public_key_ops: Tuple[str]
+    kty: str, private_key_ops: tuple[str], public_key_ops: tuple[str]
 ) -> None:
     # with a key with no alg or use, we can only trust the key_ops from the key
     private_jwk = Jwk.generate_for_kty("RSA", key_ops=private_key_ops)
     assert private_jwk.key_ops == private_key_ops
 
     public_jwk = private_jwk.public_jwk()
     assert public_key_ops == public_jwk.key_ops
@@ -196,15 +197,15 @@
         ("RS256", "sig", ("sign",), ("verify",)),
         ("HS256", "sig", ("sign", "verify"), ("sign", "verify")),
         ("A128GCMKW", "enc", ("wrapKey", "unwrapKey"), ("wrapKey", "unwrapKey")),
         ("A128GCM", "enc", ("encrypt", "decrypt"), ("encrypt", "decrypt")),
     ],
 )
 def test_use_key_ops_with_alg(
-    alg: str, use: str, private_key_ops: Tuple[str], public_key_ops: Tuple[str]
+    alg: str, use: str, private_key_ops: tuple[str], public_key_ops: tuple[str]
 ) -> None:
     # if key has an 'alg' parameter, we can deduce the use and key ops
     private_jwk = Jwk.generate(alg=alg)
     assert "use" not in private_jwk
     assert "key_ops" not in private_jwk
     assert private_jwk.use == use
     assert private_jwk.key_ops == private_key_ops
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_jwks.py` & `jwskate-0.9.0/tests/test_jwk/test_jwks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from jwskate import Jwk, JwkSet
 
 
 def test_jwkset() -> None:
     keys = [
@@ -131,22 +133,22 @@
             ]
         }
     )
     assert not jwks.is_private
     sig_keys = jwks.verification_keys()
     enc_keys = jwks.encryption_keys()
 
-    sig_kids = set(jwk.kid for jwk in sig_keys)
+    sig_kids = {jwk.kid for jwk in sig_keys}
     assert sig_kids == {
         "7KJgpwNvHJp_zb6SybahlC7506kvAm2cvMG_EY6jmx8",
         "ojHE_6b7DXtOwLKYTmeao38CV_7P9F9rYTLGm8BuJnk",
         "m7XoZRBgXXjEFxGhWvb_urskl4rCLmOhhPRdC6278-E",
     }
 
-    enc_kids = set(jwk.kid for jwk in enc_keys)
+    enc_kids = {jwk.kid for jwk in enc_keys}
     assert enc_kids == {
         "xAgzqjWdBD8cRifXbpmcv-9vIgjKHTdjelI-Vvu0K9Q",
         "zjY2pjFnBc4rOHWEwfS5Cjyxsjo2aprsctM-4oS1r8I",
     }
 
 
 def test_contains() -> None:
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_okp.py` & `jwskate-0.9.0/tests/test_jwk/test_okp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Type
+from __future__ import annotations
+
+from typing import Any
 
 import pytest
 from cryptography.hazmat.primitives.asymmetric import ed448, ed25519, x448, x25519
 
 from jwskate import EcdhEs, Jwk, JwsCompact, OKPJwk, UnsupportedAlg, UnsupportedOKPCurve
 
 
@@ -73,15 +75,15 @@
         "kty": "OKP",
         "crv": "Ed25519",
         "x": "11qYAYKxCrfVS_7TyWQHOg7hcvPapiMlrwIaaPcHURo",
     }
 
     assert jwk.thumbprint() == "kPrK_qmxVWaYVA9wwBF6Iuo3vVzz7TxHCTwXBygrS4k"
 
-    payload = "Example of Ed25519 signing".encode()
+    payload = b"Example of Ed25519 signing"
 
     jws = JwsCompact.sign(payload, key=jwk, alg="EdDSA")
     assert jws.alg == "EdDSA"
     assert jws.headers == {"alg": "EdDSA"}
     assert jws.payload == payload
     assert (
         jws
@@ -197,15 +199,15 @@
         ("Ed25519", ed25519.Ed25519PrivateKey, ed25519.Ed25519PublicKey),
         ("Ed448", ed448.Ed448PrivateKey, ed448.Ed448PublicKey),
         ("X448", x448.X448PrivateKey, x448.X448PublicKey),
         ("X25519", x25519.X25519PrivateKey, x25519.X25519PublicKey),
     ],
 )
 def test_from_to_cryptography(
-    crv: str, private_key_class: Type[Any], public_key_class: Type[Any]
+    crv: str, private_key_class: type[Any], public_key_class: type[Any]
 ) -> None:
     private_key = private_key_class.generate()
     private_jwk = Jwk(private_key)
     assert private_jwk.kty == "OKP"
     assert private_jwk.crv == crv
     assert private_jwk.is_private
     cryptography_private_key = private_jwk.cryptography_key
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_rsa.py` & `jwskate-0.9.0/tests/test_jwk/test_rsa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from binapy import BinaPy
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
 
 from jwskate import InvalidJwk, Jwk, RSAJwk
 
@@ -274,7 +276,20 @@
     assert (
         RSAJwk.private(
             n=581831797455386813246870951403662981518383326752069653161687091636524692035451059751529725021086011080514203967660708556608959257136683803000557813582922515501119301935853624127976505824935448869826468131706070569668359596404981205792279503236861179392951933850882904023094726249984093827628367499618770791850493009057079861283617675352654479608886741353320834396999001730835389809792522074674926423574848886930305414558045770900140297959808424654188427939865950543997845926585244539391125171991462109738508535281696078079754639776388404249371981016081071173090762081340239686956968800991105578566346111467394123155368705170384874671213995798439801660150643317821796194534634539623517912121487166979460992727662035485372748743978318741443625556477516010319260697801487321709403354708068079666655387397610785011757642884740600491205859334144292473286583545157303315165369083473293364140160719840416370253970866863828629349218064758107924308170514622959068660450874641869639575158904877754690639489498702228444656531867394139988003690529623350593366263757107874332106588622856789604907077776522045603251761745089378722067223763671636152452517196746862763558368663695725296997471223967074489565627326864211540190399596977703215027386153,
             d=85949297177395419163926780265753883147303791478378234122275709231519670945698011386232161227404198311995180389122407719512191385143575691102722894437488267744864904433625019433128958405445112140790812740895668030312675379445133654249912353948332427376871323215799626387744111242621092029978899443912358282017830926712145115080824932778550836637525897809280823473853648862576103843570103213992807596292689714002685800306545624906953068642498059282288809649401517214765386665192996302805748364608424898147701844106320401542786892996859182425793559229319847876687747995788259997701331373187590840021597544770796791961753608335500384254575668205802108678935368959788532572209923733762974089615830955859212984854900615892385492715494509739485608524643951383522137859067675044581594438036770305206241596314622651284901799033288653371734958728107372492924563719905501036742373214649517151325589739354495952318548566281194488480574867154877315974865051892681619475151880069335808589395737746244034473578859620398996085842063243481448414748340235721934351390661126984464918157061419702651426151358486245314693313598808122996311605590254223890285038450643678929568822731288610336853609260717107560528285489877131565432193729078274074835073573,
         )
         == jwk
     )
+
+
+def test_init_from_prime_factors() -> None:
+    p = 398075086424064937397125500550386491199064362342526708406385189575946388957261768583317
+    q = 472772146107435302536223071973048224632914695302097116459852171130520711256363590397527
+    jwk = RSAJwk.from_prime_factors(p, q)
+    assert jwk.first_prime_factor == p
+    assert jwk.second_prime_factor == q
+    assert (
+        jwk.modulus
+        == 188198812920607963838697239461650439807163563379417382700763356422988859715234665485319060606504743045317388011303396716199692321205734031879550656996221305168759307650257059
+    )
+    assert jwk.exponent == 65537
```

### Comparing `jwskate-0.8.0/tests/test_jwk/test_symmetric.py` & `jwskate-0.9.0/tests/test_jwk/test_symmetric.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from jwskate import Jwk, SymmetricJwk
 
 
 @pytest.fixture(
     scope="module",
```

### Comparing `jwskate-0.8.0/tests/test_jws.py` & `jwskate-0.9.0/tests/test_jws.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 from binapy import BinaPy
 
 from jwskate import (
     P_521,
     ECJwk,
     InvalidJws,
@@ -478,14 +480,15 @@
 ) -> None:
     """This test verifies tokens generated by `jwskate` using another lib `jwcrypto`.
 
     Args:
         signed_jws_compact: the Jws signed by jwskate to verify
         verification_jwk: the Jwk containing the verification key
         signature_alg: the signature alg
+
     """
     import jwcrypto.jwk  # type: ignore[import]
     import jwcrypto.jws  # type: ignore[import]
 
     jwk = jwcrypto.jwk.JWK(**verification_jwk)
     jws = jwcrypto.jws.JWS()
     jws.deserialize(str(signed_jws_compact))
@@ -501,14 +504,15 @@
     Args:
         signature_payload: the payload to sign
         signature_jwk: the key to use
         signature_alg: the alg to use
 
     Returns:
         a JWS token
+
     """
     import jwcrypto.jwk
     import jwcrypto.jws
 
     jwk = jwcrypto.jwk.JWK(**signature_jwk)
     jws = jwcrypto.jws.JWS(signature_payload)
 
@@ -526,14 +530,15 @@
 ) -> None:
     """Check that `jwskate` verifies tokens signed by `jwcrypto`.
 
     Args:
         jwcrypto_signed_jws: the JWS to verify
         verification_jwk: the public key to verify the signature
         signature_alg: the alg to use
+
     """
     assert JwsCompact(jwcrypto_signed_jws).verify_signature(
         verification_jwk, alg=signature_alg
     )
 
 
 def test_invalid_jws_compact() -> None:
```

### Comparing `jwskate-0.8.0/tests/test_jwt.py` & `jwskate-0.9.0/tests/test_jwt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from builtins import ValueError
 from datetime import datetime, timezone
 
 import pytest
 from binapy import BinaPy
 from freezegun import freeze_time
 
@@ -85,15 +87,17 @@
             jwk.public_jwk(),
             audience="foo",
         )
 
 
 def test_unprotected() -> None:
     jwt = Jwt.unprotected({"foo": "bar"})
-    assert jwt == "eyJhbGciOiJub25lIn0.eyJmb28iOiJiYXIifQ."
+    assert jwt == "eyJhbGciOiJub25lIiwidHlwIjoiSldUIn0.eyJmb28iOiJiYXIifQ."
+    assert jwt.alg == "none"
+    assert jwt.signature == b""
 
 
 def test_jwt_signer_and_verifier(issuer: str) -> None:
     audience = "some_audience"
     signer = JwtSigner.with_random_key(issuer, alg="ES256")
     now = datetime.now(timezone.utc)
     jwt = signer.sign(subject="some_id", audience=audience, extra_claims={"foo": "bar"})
@@ -151,18 +155,21 @@
         jwt.foo
 
     with pytest.raises(KeyError):
         jwt["foo"]
 
     assert (
         str(jwt)
-        == "eyJhbGciOiJSUzI1NiIsImtpZCI6IkpXSy1BQkNEIn0.e30.iQ6eyP9QrNDQVfKYwHpIWvnTBb0SXNEItDxMQ0VmsB5CA5FaRYtGvj01VjoUAHEegGvwFI4YI35MDY_-DUR3UIXqxVMOe9Hk2hb9paTjJLpDIa7Ml6LKDh9-4xmAAPjZcra4IYrpDux8ohg0LUzgxHn0xnKDuxKmlh9shCyNWEOfN_i_JX4v8aSD-zDBteftrY9GzHU4Y0mlvlm4FaAwafPXovZilb_dTgTBkiFLmXY0y5ESurhQ4LrQqLzBz45lSONLElil5OQu0ySrrC72CBKp-HjdpCsLyG9F9p_X-1r9mmqlN38zIcgwkbhek04ieX-rumyzvHLO_UzttxDQOg"
+        == "eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6IkpXSy1BQkNEIn0.e30.c_3ppMzgxnhn4CkLBCNNJ5_zdoS6S9P79cruukiuixMHoHIPF0_nzaj5LBRUXt3O47JiJyUzroi1MXNe_Kod9dqLRM8RJ9t3dbWJRNbPrgnCkqpUhNZ6frrc8jVs9Qu9xmXLDYEa4aSwPSkQTufWN1fC04Vzm8JUMVXM0AFeKjyEyUijEuqeBBFztDbIc2apyXWc5bZW7HEkhDNgKK0pWAVnXLwt4OwGQjd6ZOC5Hgx1wDbiam_abNWaDvR53JSCLM0wMpkYrONY_RPjWRycyeb9K5tHOcGbfRvQqpZGsRG-slf-bqwSOt-8G6Phc_YDv9Lw4NN-vqOxbo2lw-3Crw"
     )
     assert bytes(jwt) == str(jwt).encode()
-    assert jwt.signed_part == b"eyJhbGciOiJSUzI1NiIsImtpZCI6IkpXSy1BQkNEIn0.e30"
+    assert (
+        jwt.signed_part
+        == b"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6IkpXSy1BQkNEIn0.e30"
+    )
 
     jwt.validate(key=private_jwk.public_jwk(), check_exp=False)
 
     with pytest.raises(InvalidClaim):
         jwt.validate(key=private_jwk.public_jwk())
```

### Comparing `jwskate-0.8.0/PKG-INFO` & `jwskate-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: jwskate
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module.
 Home-page: https://github.com/guillp/jwskate
 License: MIT
 Author: Guillaume Pujol
 Author-email: guill.p.linux@gmail.com
-Requires-Python: >=3.8,<3.12
-Classifier: Development Status :: 3 - Alpha
+Requires-Python: >=3.8
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Security
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: binapy (>=0.6.1)
+Requires-Dist: binapy (>=0.7.0)
 Requires-Dist: cryptography (>=3.4)
 Requires-Dist: typing-extensions (>=4.3.0)
 Description-Content-Type: text/markdown
 
 # JwSkate
 
 [![PyPi](https://img.shields.io/pypi/v/jwskate.svg)](https://pypi.python.org/pypi/jwskate)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 A Pythonic implementation of the JOSE set of IETF specifications: [Json Web Signature][rfc7515], [Keys][rfc7517],
 [Algorithms][rfc7518], [Tokens][rfc7519] and [Encryption][rfc7516] (RFC7515 to 7519), and their extensions
 [ECDH Signatures][rfc8037] (RFC8037), [JWK Thumbprints][rfc7638] (RFC7638), and [JWK Thumbprint URI][rfc9278] (RFC9278),
-and with respect to [JWT Best Current Practices][rfc8725].
+and with respects to [JWT Best Current Practices][rfc8725] (RFC8725).
 
 - Free software: MIT
 - Documentation: [https://guillp.github.io/jwskate/](https://guillp.github.io/jwskate/)
 
-A quick usage example, generating an RSA private key, signing some data, then validating that signature:
+Here is a quick usage example: generating a private RSA key, signing some data, then validating that signature with the matching public key:
 
 ```python
 from jwskate import Jwk
 
 # Let's generate a random private key, to use with alg 'RS256'.
 # Based on that alg, jwskate knows it must be an RSA key.
+# RSA keys can be of variable size, so let's pass the requested key size as parameter
 rsa_private_jwk = Jwk.generate(alg="RS256", key_size=2048)
 
-data = b"Signing is easy!"
-signature = rsa_private_jwk.sign(data)
+data = b"Signing is easy!"  # we will sign this
+signature = rsa_private_jwk.sign(data)  # done!
 
-# extract the public key, and verify the signature with it
+# now extract the public key, and verify the signature with it
 rsa_public_jwk = rsa_private_jwk.public_jwk()
 assert rsa_public_jwk.verify(data, signature)
 
 # let's see what a Jwk looks like:
 assert isinstance(rsa_private_jwk, dict)  # Jwk are dict
 
 print(rsa_private_jwk.with_usage_parameters())
@@ -72,49 +73,61 @@
  'qi': '...',
  'alg': 'RS256',
  'kid': '...',
  'use': 'sig',
  'key_ops': ['sign']}
 ```
 
-Now let's sign a JWT containing arbitrary claims, this time using an EC key:
+Now let's sign a JWT containing arbitrary claims, this time using an Elliptic Curve (`EC`) key:
 
 ```python
 from jwskate import Jwk, Jwt
 
 # This time let's try an EC key, based on `alg` parameter,
-# and let's specigy an arbitrary Key ID (kid).
+# and let's specify an arbitrary Key ID (kid).
+# additional args are either options (like 'key_size' above for RSA keys)
+# or additional parameters to include in the JWK
 private_jwk = Jwk.generate(alg="ES256", kid="my_key")
+# note that based only on the `alg` value, the appropriate key type and curve
+# are automatically deduced and included in the JWK
+print(private_jwk)
+# {'kty': 'EC', 'crv': 'P-256', 'x': 'Ppe...', 'y': '9Si...', 'd': 'g09...', 'alg': 'ES256'}
+assert private_jwk.kty == "EC"
+assert private_jwk.crv == "P-256"
+assert private_jwk.alg == "ES256"
+# this is a private key and 'ES256' is a signature alg, so 'use' and 'key_ops' can also be deduced:
+assert private_jwk.use == "sig"
+assert private_jwk.key_ops == ("sign",)
 
-# here are claims to sign in a JWT:
+# here are the claims to sign in a JWT:
 claims = {"sub": "some_sub", "claim1": "value1"}
 
 jwt = Jwt.sign(claims, private_jwk)
-# that's it! we have a signed JWT
+# that's it! we have a signed JWT.
+print(jwt)
+# eyJhbGciOiJFUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.SBQIlGlFdwoEMViWUFsBmCsXShtOq4lnp3Im5ZVh1PFCGJFdW-dTG9qJjlFSAA_BkM5PF9u38PL7Ai9cC2_DJw
 assert isinstance(jwt, Jwt)  # Jwt are objects
 assert jwt.claims == claims  # claims can be accessed as a dict
-assert jwt.headers == {"alg": "ES256", "kid": "my_key"}  # headers too
+assert jwt.headers == {"typ": "JWT", "alg": "ES256", "kid": "my_key"}  # headers too
 assert jwt.sub == "some_sub"  # individual claims can be accessed as attributes
 assert jwt["claim1"] == "value1"  # or as dict items (with "subscription")
 assert jwt.alg == "ES256"  # alg and kid headers are also accessible as attributes
 assert jwt.kid == private_jwk.kid
-# notice that alg and kid are automatically set with appropriate values
+# notice that alg and kid are automatically set with appropriate values taken from our private jwk
 assert isinstance(jwt.signature, bytes)  # signature is accessible too
 # verifying the jwt signature is as easy as:
 assert jwt.verify_signature(private_jwk.public_jwk())
 # since our jwk contains an 'alg' parameter (here 'ES256'), the signature is automatically verified using that alg
 # you could also specify an alg manually, useful for keys with no "alg" hint:
 assert jwt.verify_signature(private_jwk.public_jwk(), alg="ES256")
-
-print(jwt)
-# eyJhbGciOiJFUzI1NiIsImtpZCI6Im15a2V5In0.eyJzdWIiOiJzb21lX3N1YiIsImNsYWltMSI6InZhbHVlMSJ9.C1KcDyDT8qXwUqcWzPKkQD7f6xai-gCgaRFMdKPe80Vk7XeYNa8ovuLwvdXgGW4ZZ_lL73QIyncY7tHGXUthag
-# This will output the full JWT compact representation. You can inspect it for example at <https://jwt.io>
+# note that jwskate will only trust the alg(s) you provide as parameter, either part of the JWK
+# or with `alg` or `algs` params, and will ignore the 'alg' that is set in the JWT, for security reasons.
 ```
 
-Or let's sign a JWT with the standardised lifetime, subject, audience and ID claims, plus arbitrary custom claims:
+Now let's sign a JWT with the standardised lifetime, subject, audience and ID claims, plus arbitrary custom claims:
 
 ```python
 from jwskate import Jwk, JwtSigner
 
 private_jwk = Jwk.generate(alg="ES256")
 signer = JwtSigner(issuer="https://myissuer.com", jwk=private_jwk)
 jwt = signer.sign(
@@ -122,15 +135,16 @@
     audience="some_aud",
     extra_claims={"custom_claim1": "value1", "custom_claim2": "value2"},
 )
 
 print(jwt.claims)
 ```
 
-The generated JWT claims will include the standardised claims:
+The generated JWT will include the standardised claims (`iss`, `aud`, `sub`, `iat`, `exp` and `jti`),
+together with the `extra_claims` provided to `.sign()`:
 
 ```
 {'custom_claim1': 'value1',
  'custom_claim2': 'value2',
  'iss': 'https://myissuer.com',
  'aud': 'some_aud',
  'sub': 'some_sub',
@@ -162,107 +176,107 @@
 | Json Web Signature (JWS)  | ☑ Compact<br/> ☑ JSON Flat <br/> ☑ JSON General <br/> |
 | Json Web Encryption (JWE) | ☑ Compact<br/> ☐ JSON Flat <br/> ☐ JSON General <br/> |
 | Json Web Tokens (JWT)     | ☑ Signed<br/> ☑ Signed and Encrypted                   |
 
 ### Supported Signature algorithms
 
 
-| Signature Alg | Description                                    | Key Type | Reference                          | Note                           |
-| ------------- | ---------------------------------------------- | -------- | ---------------------------------- | ------------------------------ |
-| HS256         | HMAC using SHA-256                             | oct      | [RFC7518, Section 3.2]             |                                |
-| HS384         | HMAC using SHA-384                             | oct      | [RFC7518, Section 3.2]             |                                |
-| HS512         | HMAC using SHA-512                             | oct      | [RFC7518, Section 3.2]             |                                |
-| RS256         | RSASSA-PKCS1-v1_5 using SHA-256                | RSA      | [RFC7518, Section 3.3]             |                                |
-| RS384         | RSASSA-PKCS1-v1_5 using SHA-384                | RSA      | [RFC7518, Section 3.3]             |                                |
-| RS512         | RSASSA-PKCS1-v1_5 using SHA-512                | RSA      | [RFC7518, Section 3.3]             |                                |
-| ES256         | ECDSA using P-256 and SHA-256                  | EC       | [RFC7518, Section 3.4]             |                                |
-| ES384         | ECDSA using P-384 and SHA-384                  | EC       | [RFC7518, Section 3.4]             |                                |
-| ES512         | ECDSA using P-521 and SHA-512                  | EC       | [RFC7518, Section 3.4]             |                                |
-| PS256         | RSASSA-PSS using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 3.5]             |                                |
-| PS384         | RSASSA-PSS using SHA-384 and MGF1 with SHA-384 | RSA      | [RFC7518, Section 3.5]             |                                |
-| PS512         | RSASSA-PSS using SHA-512 and MGF1 with SHA-512 | RSA      | [RFC7518, Section 3.5]             |                                |
-| EdDSA         | EdDSA signature algorithms                     | OKP      | [RFC8037, Section 3.1]             | Ed2219 and Ed448 are supported |
-| ES256K        | ECDSA using secp256k1 curve and SHA-256        | EC       | [RFC8812, Section 3.2]             |                                |
-| HS1           | HMAC using SHA-1                               | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
-| RS1           | RSASSA-PKCS1-v1_5 with SHA-1                   | oct      | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
-| none          | No digital signature or MAC performed          |          | [RFC7518, Section 3.6]             | Not usable by mistake          |
+| Signature Alg   | Description                                      | Key Type | Reference                          | Note                           |
+|-----------------|--------------------------------------------------|----------| ---------------------------------- | ------------------------------ |
+| `HS256`         | HMAC using SHA-256                               | `oct`    | [RFC7518, Section 3.2]             |                                |
+| `HS384`         | HMAC using SHA-384                               | `oct`    | [RFC7518, Section 3.2]             |                                |
+| `HS512`         | HMAC using SHA-512                               | `oct`    | [RFC7518, Section 3.2]             |                                |
+| `RS256`         | RSASSA-PKCS1-v1_5 using SHA-256                  | `RSA`    | [RFC7518, Section 3.3]             |                                |
+| `RS384`         | RSASSA-PKCS1-v1_5 using SHA-384                  | `RSA`    | [RFC7518, Section 3.3]             |                                |
+| `RS512`         | RSASSA-PKCS1-v1_5 using SHA-512                  | `RSA`    | [RFC7518, Section 3.3]             |                                |
+| `ES256`         | ECDSA using P-256 and SHA-256                    | `EC`     | [RFC7518, Section 3.4]             |                                |
+| `ES384`         | ECDSA using P-384 and SHA-384                    | `EC`     | [RFC7518, Section 3.4]             |                                |
+| `ES512`         | ECDSA using P-521 and SHA-512                    | `EC`     | [RFC7518, Section 3.4]             |                                |
+| `PS256`         | RSASSA-PSS using SHA-256 and MGF1 with SHA-256   | `RSA`    | [RFC7518, Section 3.5]             |                                |
+| `PS384`         | RSASSA-PSS using SHA-384 and MGF1 with SHA-384   | `RSA`    | [RFC7518, Section 3.5]             |                                |
+| `PS512`         | RSASSA-PSS using SHA-512 and MGF1 with SHA-512   | `RSA`    | [RFC7518, Section 3.5]             |                                |
+| `EdDSA`         | EdDSA signature algorithms                       | `OKP`    | [RFC8037, Section 3.1]             | Ed2219 and Ed448 are supported |
+| `ES256K`        | ECDSA using secp256k1 curve and SHA-256          | `EC`     | [RFC8812, Section 3.2]             |                                |
+| `HS1`           | HMAC using SHA-1                                 | `oct`    | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
+| `RS1`           | RSASSA-PKCS1-v1_5 with SHA-1                     | `oct`    | https://www.w3.org/TR/WebCryptoAPI | Validation Only                |
+| `none`          | No digital signature or MAC performed            |          | [RFC7518, Section 3.6]             | Not usable by mistake          |
 
 ### Supported Key Management algorithms
 
 
-| Signature Alg      | Description                                    | Key Type | Reference                          | Note        |
-| ------------------ | ---------------------------------------------- | -------- | ---------------------------------- | ----------- |
-| RSA1_5             | RSAES-PKCS1-v1_5                               | RSA      | [RFC7518, Section 4.2]             | Unwrap Only |
-| RSA-OAEP           | RSAES OAEP using default parameters            | RSA      | [RFC7518, Section 4.3]             |             |
-| RSA-OAEP-256       | RSAES OAEP using SHA-256 and MGF1 with SHA-256 | RSA      | [RFC7518, Section 4.3]             |             |
-| RSA-OAEP-384       | RSA-OAEP using SHA-384 and MGF1 with SHA-384   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
-| RSA-OAEP-512       | RSA-OAEP using SHA-512 and MGF1 with SHA-512   | RSA      | https://www.w3.org/TR/WebCryptoAPI |             |
-| A128KW             | AES Key Wrap using 128-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
-| A192KW             | AES Key Wrap using 192-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
-| A256KW             | AES Key Wrap using 256-bit key                 | oct      | [RFC7518, Section 4.4]             |             |
-| dir                | Direct use of a shared symmetric key           | oct      | [RFC7518, Section 4.5]             |             |
-| ECDH-ES            | ECDH-ES using Concat KDF                       | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A128KW     | ECDH-ES using Concat KDF and "A128KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A192KW     | ECDH-ES using Concat KDF and "A192KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
-| ECDH-ES+A256KW     | ECDH-ES using Concat KDF and "A256KW" wrapping | EC       | [RFC7518, Section 4.6]             |             |
-| A128GCMKW          | Key wrapping with AES GCM using 128-bit key    | oct      | [RFC7518, Section 4.7]             |             |
-| A192GCMKW          | Key wrapping with AES GCM using 192-bit key    | oct      | [RFC7518, Section 4.7]             |             |
-| A256GCMKW          | Key wrapping with AES GCM using 256-bit key    | oct      | [RFC7518, Section 4.7]             |             |
-| PBES2-HS256+A128KW | PBES2 with HMAC SHA-256 and "A128KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
-| PBES2-HS384+A192KW | PBES2 with HMAC SHA-384 and "A192KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
-| PBES2-HS512+A256KW | PBES2 with HMAC SHA-512 and "A256KW" wrapping  | password | [RFC7518, Section 4.8]             |             |
+| Signature Alg      | Description                                    | Key Type      | Reference                          | Note        |
+| ------------------ | ---------------------------------------------- |---------------| ---------------------------------- | ----------- |
+| `RSA1_5`             | RSAES-PKCS1-v1_5                               | `RSA`       | [RFC7518, Section 4.2]             | Unwrap Only |
+| `RSA-OAEP`           | RSAES OAEP using default parameters            | `RSA`       | [RFC7518, Section 4.3]             |             |
+| `RSA-OAEP-256`       | RSAES OAEP using SHA-256 and MGF1 with SHA-256 | `RSA`       | [RFC7518, Section 4.3]             |             |
+| `RSA-OAEP-384`       | RSA-OAEP using SHA-384 and MGF1 with SHA-384   | `RSA`       | https://www.w3.org/TR/WebCryptoAPI |             |
+| `RSA-OAEP-512`       | RSA-OAEP using SHA-512 and MGF1 with SHA-512   | `RSA`       | https://www.w3.org/TR/WebCryptoAPI |             |
+| `A128KW`             | AES Key Wrap using 128-bit key                 | `oct`       | [RFC7518, Section 4.4]             |             |
+| `A192KW`             | AES Key Wrap using 192-bit key                 | `oct`       | [RFC7518, Section 4.4]             |             |
+| `A256KW`             | AES Key Wrap using 256-bit key                 | `oct`       | [RFC7518, Section 4.4]             |             |
+| `A128GCMKW`          | Key wrapping with AES GCM using 128-bit key    | `oct`       | [RFC7518, Section 4.7]             |             |
+| `A192GCMKW`          | Key wrapping with AES GCM using 192-bit key    | `oct`       | [RFC7518, Section 4.7]             |             |
+| `A256GCMKW`          | Key wrapping with AES GCM using 256-bit key    | `oct`       | [RFC7518, Section 4.7]             |             |
+| `dir`                | Direct use of a shared symmetric key           | `oct`       | [RFC7518, Section 4.5]             |             |
+| `ECDH-ES`            | ECDH-ES using Concat KDF                       | `EC`        | [RFC7518, Section 4.6]             |             |
+| `ECDH-ES+A128KW`     | ECDH-ES using Concat KDF and "A128KW" wrapping | `EC`        | [RFC7518, Section 4.6]             |             |
+| `ECDH-ES+A192KW`     | ECDH-ES using Concat KDF and "A192KW" wrapping | `EC`        | [RFC7518, Section 4.6]             |             |
+| `ECDH-ES+A256KW`     | ECDH-ES using Concat KDF and "A256KW" wrapping | `EC`        | [RFC7518, Section 4.6]             |             |
+| `PBES2-HS256+A128KW` | PBES2 with HMAC SHA-256 and "A128KW" wrapping  | `password`  | [RFC7518, Section 4.8]             |             |
+| `PBES2-HS384+A192KW` | PBES2 with HMAC SHA-384 and "A192KW" wrapping  | `password`  | [RFC7518, Section 4.8]             |             |
+| `PBES2-HS512+A256KW` | PBES2 with HMAC SHA-512 and "A256KW" wrapping  | `password`  | [RFC7518, Section 4.8]             |             |
 
 ### Supported Encryption algorithms
 
 
 | Signature Alg | Description                                                 | Reference                |
 | ------------- | ----------------------------------------------------------- | ------------------------ |
-| A128CBC-HS256 | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
-| A192CBC-HS384 | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
-| A256CBC-HS512 | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
-| A128GCM       | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
-| A192GCM       | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
-| A256GCM       | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
+| `A128CBC-HS256` | AES_128_CBC_HMAC_SHA_256 authenticated encryption algorithm | [RFC7518, Section 5.2.3] |
+| `A192CBC-HS384` | AES_192_CBC_HMAC_SHA_384 authenticated encryption algorithm | [RFC7518, Section 5.2.4] |
+| `A256CBC-HS512` | AES_256_CBC_HMAC_SHA_512 authenticated encryption algorithm | [RFC7518, Section 5.2.5] |
+| `A128GCM`       | AES GCM using 128-bit key                                   | [RFC7518, Section 5.3]   |
+| `A192GCM`       | AES GCM using 192-bit key                                   | [RFC7518, Section 5.3]   |
+| `A256GCM`       | AES GCM using 256-bit key                                   | [RFC7518, Section 5.3]   |
 
 ### Supported Elliptic Curves
 
 
-| Curve     | Description                           | Key Type | Usage                 | Reference                  |
-| --------- | ------------------------------------- | -------- | --------------------- | -------------------------- |
-| P-256     | P-256 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
-| P-384     | P-384 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
-| P-521     | P-521 Curve                           | EC       | signature, encryption | [RFC7518, Section 6.2.1.1] |
-| Ed25519   | Ed25519 signature algorithm key pairs | OKP      | signature             | [RFC8037, Section 3.1]     |
-| Ed448     | Ed448 signature algorithm key pairs   | OKP      | signature             | [RFC8037, Section 3.1]     |
-| X25519    | X25519 function key pairs             | OKP      | encryption            | [RFC8037, Section 3.2]     |
-| X448      | X448 function key pairs               | OKP      | encryption            | [RFC8037, Section 3.2]     |
-| secp256k1 | SECG secp256k1 curve                  | EC       | signature, encryption | [RFC8812, Section 3.1]     |
+| Curve       | Description                           | Key Type | Usage                 | Reference                  |
+|-------------|---------------------------------------|----------| --------------------- | -------------------------- |
+| `P-256`     | P-256 Curve                           | `EC`     | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| `P-384`     | P-384 Curve                           | `EC`     | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| `P-521`     | P-521 Curve                           | `EC`     | signature, encryption | [RFC7518, Section 6.2.1.1] |
+| `Ed25519`   | Ed25519 signature algorithm key pairs | `OKP`    | signature             | [RFC8037, Section 3.1]     |
+| `Ed448`     | Ed448 signature algorithm key pairs   | `OKP`    | signature             | [RFC8037, Section 3.1]     |
+| `X25519`    | X25519 function key pairs             | `OKP`    | encryption            | [RFC8037, Section 3.2]     |
+| `X448`      | X448 function key pairs               | `OKP`    | encryption            | [RFC8037, Section 3.2]     |
+| `secp256k1` | SECG secp256k1 curve                  | `EC`     | signature, encryption | [RFC8812, Section 3.1]     |
 
 ## Why a new lib ?
 
 There are already multiple modules implementing JOSE and Json Web Crypto related specifications in Python. However, I
 have been dissatisfied by all of them so far, so I decided to come up with my own module.
 
 - [PyJWT](https://pyjwt.readthedocs.io)
 - [JWCrypto](https://jwcrypto.readthedocs.io/)
 - [Python-JOSE](https://python-jose.readthedocs.io/)
 - [AuthLib](https://docs.authlib.org/en/latest/jose/)
 
 Not to say that those are _bad_ libs (I actually use `jwcrypto` myself for `jwskate` unit tests), but they either don't
-support some important features, lack documentation, or generally have APIs that don't feel easy-enough, Pythonic-enough
+support some important features, lack documentation, or more generally have APIs that don't feel easy-enough, Pythonic-enough
 to use.
 
 ## Design
 
 ### JWK are dicts
 
 JWK are specified as JSON objects, which are parsed as `dict` in Python. The `Jwk` class in `jwskate` is actually a
-`dict` subclass, so you can use it exactly like you would use a dict: you can access its members, dump it back as JSON,
-etc. The same is true for Signed or Encrypted Json Web tokens in JSON format. You cannot change the key cryptographic
-material, however, since that would lead to unusable keys.
+`dict` subclass, so you can use it exactly like you would use a `dict`: you can access its members, dump it back as JSON,
+etc. The same is true for Signed or Encrypted Json Web tokens in JSON format. However, you cannot change the key cryptographic
+materials, since that would lead to unusable keys.
 
 ### JWA Wrappers
 
 You can use `cryptography` to do the cryptographic operations that are described in
 [JWA](https://www.rfc-editor.org/info/rfc7518), but since `cryptography` is a general purpose library, its usage is not
 straightforward and gives you plenty of options to carefully select and combine, leaving room for mistakes, errors and
 confusion. It has also a quite inconsistent API to handle the different type of keys and algorithms. To work around
```

