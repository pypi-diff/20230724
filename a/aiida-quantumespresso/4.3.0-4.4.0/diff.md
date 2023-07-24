# Comparing `tmp/aiida-quantumespresso-4.3.0.tar.gz` & `tmp/aiida_quantumespresso-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-quantumespresso-4.3.0.tar", last modified: Thu Apr 27 14:24:01 2023, max compression
+gzip compressed data, was "aiida_quantumespresso-4.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-quantumespresso-4.3.0.tar` & `aiida_quantumespresso-4.4.0.tar`

### file list

```diff
@@ -1,206 +1,207 @@
--rw-r--r--   0        0        0      148 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/code-ph.yaml
--rw-r--r--   0        0        0      148 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/code-pw.yaml
--rw-r--r--   0        0        0       43 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/localhost-config.yaml
--rw-r--r--   0        0        0      234 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/localhost-setup.yaml
--rw-r--r--   0        0        0      215 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/profile.yaml
--rw-r--r--   0        0        0     1922 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/scripts/run_documentation_scripts.py
--rw-r--r--   0        0        0     3009 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4135 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2291 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/nightly.yml
--rw-r--r--   0        0        0     1520 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0     1303 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.gitignore
--rw-r--r--   0        0        0     1347 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      239 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.readthedocs.yml
--rw-r--r--   0        0        0    36108 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1273 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/LICENSE.txt
--rw-r--r--   0        0        0    30387 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/README.md
--rw-r--r--   0        0        0     8567 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/__init__.py
--rw-r--r--   0        0        0    39136 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/__init__.py
--rw-r--r--   0        0        0     2017 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/base.py
--rw-r--r--   0        0        0     6658 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/cp.py
--rw-r--r--   0        0        0     1539 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/dos.py
--rw-r--r--   0        0        0    14015 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/epw.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py
--rw-r--r--   0        0        0     1226 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py
--rw-r--r--   0        0        0     1436 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/__init__.py
--rw-r--r--   0        0        0     4593 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py
--rw-r--r--   0        0        0     4251 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py
--rw-r--r--   0        0        0     5358 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py
--rw-r--r--   0        0        0     2624 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py
--rw-r--r--   0        0        0    84796 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml
--rw-r--r--   0        0        0    87073 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml
--rw-r--r--   0        0        0    87073 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml
--rw-r--r--   0        0        0    83767 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml
--rw-r--r--   0        0        0    96224 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml
--rw-r--r--   0        0        0    96319 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml
--rw-r--r--   0        0        0    93230 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml
--rw-r--r--   0        0        0    96763 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml
--rw-r--r--   0        0        0    97862 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml
--rw-r--r--   0        0        0    97871 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml
--rw-r--r--   0        0        0    98698 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml
--rw-r--r--   0        0        0   109373 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml
--rw-r--r--   0        0        0   110988 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml
--rw-r--r--   0        0        0   112295 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml
--rw-r--r--   0        0        0   116180 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml
--rw-r--r--   0        0        0   118149 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml
--rw-r--r--   0        0        0    26623 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/__init__.py
--rw-r--r--   0        0        0     4732 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/matdyn.py
--rw-r--r--   0        0        0    10109 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/namelists.py
--rw-r--r--   0        0        0    17188 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/neb.py
--rw-r--r--   0        0        0     2058 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/open_grid.py
--rw-r--r--   0        0        0    16652 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/ph.py
--rw-r--r--   0        0        0    11374 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pp.py
--rw-r--r--   0        0        0     3843 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/projwfc.py
--rw-r--r--   0        0        0    14592 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw.py
--rw-r--r--   0        0        0     3578 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2gw.py
--rw-r--r--   0        0        0     3052 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2wannier90.py
--rw-r--r--   0        0        0    23331 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pwimmigrant.py
--rw-r--r--   0        0        0     1948 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/q2r.py
--rw-r--r--   0        0        0     6062 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/xspectra.py
--rw-r--r--   0        0        0      609 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/__init__.py
--rw-r--r--   0        0        0      874 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/__init__.py
--rw-r--r--   0        0        0     2130 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/cp.py
--rwxr-xr-x   0        0        0     1992 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/dos.py
--rw-r--r--   0        0        0     3530 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/epw.py
--rw-r--r--   0        0        0     1418 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/matdyn.py
--rw-r--r--   0        0        0     3622 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/neb.py
--rw-r--r--   0        0        0     2118 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/ph.py
--rw-r--r--   0        0        0     1981 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pp.py
--rwxr-xr-x   0        0        0     2012 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/projwfc.py
--rw-r--r--   0        0        0     4121 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw.py
--rwxr-xr-x   0        0        0     3060 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py
--rw-r--r--   0        0        0     1794 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/q2r.py
--rw-r--r--   0        0        0      361 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/data/__init__.py
--rw-r--r--   0        0        0     1062 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/data/structure.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/__init__.py
--rw-r--r--   0        0        0     1555 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/defaults.py
--rw-r--r--   0        0        0     1530 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/display.py
--rw-r--r--   0        0        0     1259 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/launch.py
--rw-r--r--   0        0        0     6820 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/options.py
--rw-r--r--   0        0        0     5435 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/validate.py
--rw-r--r--   0        0        0      675 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/matdyn/__init__.py
--rwxr-xr-x   0        0        0     1666 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/ph/__init__.py
--rwxr-xr-x   0        0        0     1568 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/ph/base.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/__init__.py
--rwxr-xr-x   0        0        0     3526 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py
--rwxr-xr-x   0        0        0     2720 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/base.py
--rwxr-xr-x   0        0        0     3408 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/q2r/__init__.py
--rwxr-xr-x   0        0        0     1720 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py
--rw-r--r--   0        0        0       84 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/__init__.py
--rw-r--r--   0        0        0     6183 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/hubbard.py
--rw-r--r--   0        0        0     1588 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/types.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/__init__.py
--rw-r--r--   0        0        0     9253 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/force_constants.py
--rw-r--r--   0        0        0     9221 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/hubbard_structure.py
--rw-r--r--   0        0        0      202 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/__init__.py
--rw-r--r--   0        0        0     2474 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/base.py
--rw-r--r--   0        0        0    16768 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/cp.py
--rw-r--r--   0        0        0     5575 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/dos.py
--rw-r--r--   0        0        0     4778 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/matdyn.py
--rw-r--r--   0        0        0    10493 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/neb.py
--rw-r--r--   0        0        0     3061 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/open_grid.py
--rw-r--r--   0        0        0       71 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/__init__.py
--rw-r--r--   0        0        0     6752 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/base.py
--rw-r--r--   0        0        0     8844 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py
--rw-r--r--   0        0        0    10943 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py
--rw-r--r--   0        0        0    20682 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py
--rw-r--r--   0        0        0    48436 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py
--rw-r--r--   0        0        0     1890 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw2gw.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/cp/__init__.py
--rw-r--r--   0        0        0    17305 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py
--rw-r--r--   0        0        0      291 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/exceptions.py
--rw-r--r--   0        0        0    21297 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py
--rw-r--r--   0        0        0    24260 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/__init__.py
--rw-r--r--   0        0        0    16555 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py
--rw-r--r--   0        0        0      906 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py
--rw-r--r--   0        0        0    39204 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd
--rw-r--r--   0        0        0    42964 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd
--rw-r--r--   0        0        0    41134 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd
--rw-r--r--   0        0        0    41234 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd
--rw-r--r--   0        0        0    42964 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd
--rw-r--r--   0        0        0    42964 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd
--rw-r--r--   0        0        0    49812 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd
--rw-r--r--   0        0        0    57907 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd
--rw-r--r--   0        0        0    58917 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd
--rw-r--r--   0        0        0     4627 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py
--rw-r--r--   0        0        0     3110 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/ph.py
--rw-r--r--   0        0        0    15908 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pp.py
--rw-r--r--   0        0        0    20459 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/projwfc.py
--rw-r--r--   0        0        0    29470 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw.py
--rw-r--r--   0        0        0     4210 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2gw.py
--rw-r--r--   0        0        0     1316 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2wannier90.py
--rw-r--r--   0        0        0     1250 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/q2r.py
--rw-r--r--   0        0        0    11344 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/xspectra.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/__init__.py
--rw-r--r--   0        0        0     2840 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/base.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/calculations/__init__.py
--rw-r--r--   0        0        0     2288 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/calculations/pw.py
--rw-r--r--   0        0        0     1035 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/cpinputparser.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/__init__.py
--rw-r--r--   0        0        0     2981 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py
--rw-r--r--   0        0        0     5427 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py
--rw-r--r--   0        0        0     6586 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/pwinputparser.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/__init__.py
--rw-r--r--   0        0        0     3972 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/bands.py
--rw-r--r--   0        0        0     8343 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/convert.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/defaults/__init__.py
--rw-r--r--   0        0        0      610 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py
--rw-r--r--   0        0        0    15021 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/hubbard.py
--rw-r--r--   0        0        0     1032 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/linalg.py
--rw-r--r--   0        0        0     3672 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/mapping.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/__init__.py
--rw-r--r--   0        0        0    10193 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/pw.py
--rw-r--r--   0        0        0    14855 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json
--rw-r--r--   0        0        0    15000 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json
--rw-r--r--   0        0        0    14831 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json
--rw-r--r--   0        0        0    15000 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json
--rw-r--r--   0        0        0     3050 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/resources.py
--rw-r--r--   0        0        0     2615 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/restart.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/validation/__init__.py
--rw-r--r--   0        0        0     5337 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/validation/trajectory.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/__init__.py
--rw-r--r--   0        0        0      671 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py
--rw-r--r--   0        0        0    15977 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py
--rw-r--r--   0        0        0      665 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/matdyn/__init__.py
--rw-r--r--   0        0        0     2682 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/matdyn/base.py
--rw-r--r--   0        0        0    26001 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pdos.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/ph/__init__.py
--rw-r--r--   0        0        0    13101 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/ph/base.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/__init__.py
--rw-r--r--   0        0        0     1125 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml
--rw-r--r--   0        0        0     1469 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml
--rw-r--r--   0        0        0     1983 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/ph/__init__.py
--rw-r--r--   0        0        0     1064 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/__init__.py
--rw-r--r--   0        0        0     1045 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml
--rw-r--r--   0        0        0     1804 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml
--rw-r--r--   0        0        0      840 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml
--rw-r--r--   0        0        0     5838 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/utils.py
--rw-r--r--   0        0        0      538 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml
--rw-r--r--   0        0        0     1892 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml
--rw-r--r--   0        0        0      657 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml
--rw-r--r--   0        0        0      599 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/__init__.py
--rw-r--r--   0        0        0    16503 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/bands.py
--rw-r--r--   0        0        0    30947 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/base.py
--rw-r--r--   0        0        0    18141 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/relax.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/q2r/__init__.py
--rw-r--r--   0        0        0     2649 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/q2r/base.py
--rw-r--r--   0        0        0    30756 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xps.py
--rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/__init__.py
--rw-r--r--   0        0        0    12841 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/base.py
--rw-r--r--   0        0        0    34623 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/core.py
--rw-r--r--   0        0        0    30297 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py
--rw-r--r--   0        0        0    32371 1970-01-01 00:00:00.000000 aiida-quantumespresso-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/config/code-ph.yaml
+-rw-r--r--   0        0        0      148 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/config/code-pw.yaml
+-rw-r--r--   0        0        0       43 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/config/localhost-config.yaml
+-rw-r--r--   0        0        0      234 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/config/localhost-setup.yaml
+-rw-r--r--   0        0        0      215 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/config/profile.yaml
+-rw-r--r--   0        0        0     1922 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/scripts/run_documentation_scripts.py
+-rw-r--r--   0        0        0     3009 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4135 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2284 2023-07-24 13:39:30.078890 aiida_quantumespresso-4.4.0/.github/workflows/nightly.yml
+-rw-r--r--   0        0        0     2479 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/.github/workflows/update_changelog.py
+-rw-r--r--   0        0        0     1520 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0     1286 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/.gitignore
+-rw-r--r--   0        0        0     1347 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      277 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/.readthedocs.yml
+-rw-r--r--   0        0        0    41943 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1273 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/LICENSE.txt
+-rw-r--r--   0        0        0    30387 2023-07-24 13:39:30.082890 aiida_quantumespresso-4.4.0/README.md
+-rw-r--r--   0        0        0     8543 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/__init__.py
+-rw-r--r--   0        0        0    38896 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/base.py
+-rw-r--r--   0        0        0     6243 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/cp.py
+-rw-r--r--   0        0        0     1245 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/dos.py
+-rw-r--r--   0        0        0    14015 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/epw.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/__init__.py
+-rw-r--r--   0        0        0     1595 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0     5461 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/create_magnetic_configuration.py
+-rw-r--r--   0        0        0     1226 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py
+-rw-r--r--   0        0        0     1436 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/__init__.py
+-rw-r--r--   0        0        0     4593 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py
+-rw-r--r--   0        0        0     4251 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py
+-rw-r--r--   0        0        0     5358 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py
+-rw-r--r--   0        0        0     2624 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py
+-rw-r--r--   0        0        0    84796 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml
+-rw-r--r--   0        0        0    87073 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml
+-rw-r--r--   0        0        0    87073 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml
+-rw-r--r--   0        0        0    83767 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml
+-rw-r--r--   0        0        0    96224 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml
+-rw-r--r--   0        0        0    96319 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml
+-rw-r--r--   0        0        0    93230 2023-07-24 13:39:30.094890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml
+-rw-r--r--   0        0        0    96763 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml
+-rw-r--r--   0        0        0    97862 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml
+-rw-r--r--   0        0        0    97871 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml
+-rw-r--r--   0        0        0    98698 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml
+-rw-r--r--   0        0        0   109373 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml
+-rw-r--r--   0        0        0   110988 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml
+-rw-r--r--   0        0        0   112295 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml
+-rw-r--r--   0        0        0   116180 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml
+-rw-r--r--   0        0        0   118149 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml
+-rw-r--r--   0        0        0    26623 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/__init__.py
+-rw-r--r--   0        0        0     4438 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/matdyn.py
+-rw-r--r--   0        0        0    10731 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/namelists.py
+-rw-r--r--   0        0        0    16773 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/neb.py
+-rw-r--r--   0        0        0     1650 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/open_grid.py
+-rw-r--r--   0        0        0    16652 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/ph.py
+-rw-r--r--   0        0        0    11511 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pp.py
+-rw-r--r--   0        0        0     3549 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/projwfc.py
+-rw-r--r--   0        0        0    13364 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pw.py
+-rw-r--r--   0        0        0     3008 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pw2gw.py
+-rw-r--r--   0        0        0     2758 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pw2wannier90.py
+-rw-r--r--   0        0        0    23331 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pwimmigrant.py
+-rw-r--r--   0        0        0     1654 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/q2r.py
+-rw-r--r--   0        0        0     5746 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/xspectra.py
+-rw-r--r--   0        0        0      609 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/__init__.py
+-rw-r--r--   0        0        0      874 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/__init__.py
+-rw-r--r--   0        0        0     2130 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/cp.py
+-rwxr-xr-x   0        0        0     1992 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/dos.py
+-rw-r--r--   0        0        0     3530 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/epw.py
+-rw-r--r--   0        0        0     1418 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/matdyn.py
+-rw-r--r--   0        0        0     3622 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/neb.py
+-rw-r--r--   0        0        0     2118 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/ph.py
+-rw-r--r--   0        0        0     1981 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/pp.py
+-rwxr-xr-x   0        0        0     2012 2023-07-24 13:39:30.098890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/projwfc.py
+-rw-r--r--   0        0        0     4121 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/pw.py
+-rwxr-xr-x   0        0        0     3060 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py
+-rw-r--r--   0        0        0     1794 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/q2r.py
+-rw-r--r--   0        0        0      361 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/data/__init__.py
+-rw-r--r--   0        0        0     1062 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/data/structure.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1555 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/defaults.py
+-rw-r--r--   0        0        0     1530 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/display.py
+-rw-r--r--   0        0        0     1259 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/launch.py
+-rw-r--r--   0        0        0     6820 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/options.py
+-rw-r--r--   0        0        0     5435 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/validate.py
+-rw-r--r--   0        0        0      675 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/matdyn/__init__.py
+-rwxr-xr-x   0        0        0     1666 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/ph/__init__.py
+-rwxr-xr-x   0        0        0     1568 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/ph/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/__init__.py
+-rwxr-xr-x   0        0        0     3526 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py
+-rwxr-xr-x   0        0        0     2720 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/base.py
+-rwxr-xr-x   0        0        0     3408 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/q2r/__init__.py
+-rwxr-xr-x   0        0        0     1720 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py
+-rw-r--r--   0        0        0       84 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/common/__init__.py
+-rw-r--r--   0        0        0     6143 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/common/hubbard.py
+-rw-r--r--   0        0        0     1588 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/common/types.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/data/__init__.py
+-rw-r--r--   0        0        0     9253 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/data/force_constants.py
+-rw-r--r--   0        0        0     9294 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/data/hubbard_structure.py
+-rw-r--r--   0        0        0      202 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/__init__.py
+-rw-r--r--   0        0        0     8636 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/base.py
+-rw-r--r--   0        0        0    17005 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/cp.py
+-rw-r--r--   0        0        0     5089 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/dos.py
+-rw-r--r--   0        0        0     4749 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/matdyn.py
+-rw-r--r--   0        0        0     9541 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/neb.py
+-rw-r--r--   0        0        0     2749 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/open_grid.py
+-rw-r--r--   0        0        0       71 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/__init__.py
+-rw-r--r--   0        0        0     2686 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/base.py
+-rw-r--r--   0        0        0     8576 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py
+-rw-r--r--   0        0        0     6773 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py
+-rw-r--r--   0        0        0    18957 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py
+-rw-r--r--   0        0        0    48436 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/cp/__init__.py
+-rw-r--r--   0        0        0    17305 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py
+-rw-r--r--   0        0        0      291 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/exceptions.py
+-rw-r--r--   0        0        0    21297 2023-07-24 13:39:30.102890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py
+-rw-r--r--   0        0        0    24260 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/pw/__init__.py
+-rw-r--r--   0        0        0    16555 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py
+-rw-r--r--   0        0        0      906 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py
+-rw-r--r--   0        0        0    39204 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd
+-rw-r--r--   0        0        0    42964 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd
+-rw-r--r--   0        0        0    41134 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd
+-rw-r--r--   0        0        0    41234 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd
+-rw-r--r--   0        0        0    42964 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd
+-rw-r--r--   0        0        0    42964 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd
+-rw-r--r--   0        0        0    49812 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd
+-rw-r--r--   0        0        0    57907 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd
+-rw-r--r--   0        0        0    58917 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd
+-rw-r--r--   0        0        0     4627 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py
+-rw-r--r--   0        0        0     2684 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/ph.py
+-rw-r--r--   0        0        0    13750 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pp.py
+-rw-r--r--   0        0        0    19897 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/projwfc.py
+-rw-r--r--   0        0        0    29518 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pw.py
+-rw-r--r--   0        0        0     2882 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pw2gw.py
+-rw-r--r--   0        0        0     1067 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pw2wannier90.py
+-rw-r--r--   0        0        0     1369 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/q2r.py
+-rw-r--r--   0        0        0    10164 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/xspectra.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/__init__.py
+-rw-r--r--   0        0        0     2840 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/calculations/__init__.py
+-rw-r--r--   0        0        0     4288 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/calculations/pw.py
+-rw-r--r--   0        0        0     1035 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/cpinputparser.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/data/orbital/__init__.py
+-rw-r--r--   0        0        0     2981 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py
+-rw-r--r--   0        0        0     5427 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py
+-rw-r--r--   0        0        0     6586 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/pwinputparser.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/__init__.py
+-rw-r--r--   0        0        0     3972 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/bands.py
+-rw-r--r--   0        0        0     8343 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/convert.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/defaults/__init__.py
+-rw-r--r--   0        0        0      610 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py
+-rw-r--r--   0        0        0    15043 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/hubbard.py
+-rw-r--r--   0        0        0     1032 2023-07-24 13:39:30.106890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/linalg.py
+-rw-r--r--   0        0        0     3672 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/mapping.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/__init__.py
+-rw-r--r--   0        0        0    10193 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/pw.py
+-rw-r--r--   0        0        0    14855 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json
+-rw-r--r--   0        0        0    15000 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json
+-rw-r--r--   0        0        0    14831 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json
+-rw-r--r--   0        0        0    15000 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json
+-rw-r--r--   0        0        0     3050 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/resources.py
+-rw-r--r--   0        0        0     2615 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/restart.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/validation/__init__.py
+-rw-r--r--   0        0        0     5337 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/validation/trajectory.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/__init__.py
+-rw-r--r--   0        0        0      671 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0    15977 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py
+-rw-r--r--   0        0        0      665 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/matdyn/__init__.py
+-rw-r--r--   0        0        0     2682 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/matdyn/base.py
+-rw-r--r--   0        0        0    25876 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pdos.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/ph/__init__.py
+-rw-r--r--   0        0        0    13101 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/ph/base.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/__init__.py
+-rw-r--r--   0        0        0     1125 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml
+-rw-r--r--   0        0        0     1469 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml
+-rw-r--r--   0        0        0     1983 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/ph/__init__.py
+-rw-r--r--   0        0        0     1064 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/__init__.py
+-rw-r--r--   0        0        0     1045 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml
+-rw-r--r--   0        0        0     1804 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml
+-rw-r--r--   0        0        0      840 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml
+-rw-r--r--   0        0        0     5782 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/utils.py
+-rw-r--r--   0        0        0      538 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml
+-rw-r--r--   0        0        0     1892 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml
+-rw-r--r--   0        0        0      657 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml
+-rw-r--r--   0        0        0      599 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/__init__.py
+-rw-r--r--   0        0        0    16378 2023-07-24 13:39:30.110890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/bands.py
+-rw-r--r--   0        0        0    30947 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/base.py
+-rw-r--r--   0        0        0    18141 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/relax.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/q2r/__init__.py
+-rw-r--r--   0        0        0     2649 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/q2r/base.py
+-rw-r--r--   0        0        0    30756 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xps.py
+-rw-r--r--   0        0        0        0 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/__init__.py
+-rw-r--r--   0        0        0    12841 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/base.py
+-rw-r--r--   0        0        0    34623 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/core.py
+-rw-r--r--   0        0        0    30297 2023-07-24 13:39:30.114890 aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py
+-rw-r--r--   0        0        0    32448 1970-01-01 00:00:00.000000 aiida_quantumespresso-4.4.0/PKG-INFO
```

### Comparing `aiida-quantumespresso-4.3.0/.github/scripts/run_documentation_scripts.py` & `aiida_quantumespresso-4.4.0/.github/scripts/run_documentation_scripts.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/.github/workflows/cd.yml` & `aiida_quantumespresso-4.4.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/.github/workflows/ci.yml` & `aiida_quantumespresso-4.4.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/.github/workflows/nightly.yml` & `aiida_quantumespresso-4.4.0/.github/workflows/nightly.yml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     tests:
 
         if: github.repository == 'aiidateam/aiida-quantumespresso'  # Prevent running the builds on forks as well
         runs-on: ubuntu-latest
 
         strategy:
             matrix:
-                python-version: ['3.8', '3.9', '3.10', '3.11']
+                python-version: ['3.9', '3.10', '3.11']
 
         services:
             postgres:
                 image: postgres:12
             rabbitmq:
                 image: rabbitmq:latest
                 ports:
```

### Comparing `aiida-quantumespresso-4.3.0/.github/workflows/validate_release_tag.py` & `aiida_quantumespresso-4.4.0/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/.gitignore` & `aiida_quantumespresso-4.4.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -107,8 +107,8 @@
 
 *~
 .DS_Store
 .idea
 submit_test/
 
 # Autogenerated API docs
-docs/source/reference/api/aiida_quantumespresso
+docs/source/reference/api/auto
```

### Comparing `aiida-quantumespresso-4.3.0/.pre-commit-config.yaml` & `aiida_quantumespresso-4.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/CHANGELOG.md` & `aiida_quantumespresso-4.4.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,132 @@
+## v4.4.0
+
+This minor release mainly includes documentation changes, but also a small breaking change in [[a389629](https://github.com/aiidateam/aiida-quantumespresso/commit/a389629387b74805ffe2f4d6515ac05b8f62b4d5)].
+Work chains that wrap the `PwBaseWorkChain` for an `nscf` or `bands` calculation and add the `parent_folder` during runtime would have to adapt the `validator` for the `pw` name space as follows to avoid warnings:
+
+```python
+    spec.inputs['nscf']['pw'].validator = PwCalculation.validate_inputs_base
+```
+
+Now, the validator that checks for the presence of the `parent_folder` in the inputs is adapted so it checks if the  `parent_folder` port is in the name space.
+If not, the validation is skipped.
+So work chains that wrap the `PwBaseWorkChain` to run an `nscf` or `bands` calculation can simply exclude the `parent_folder` port in the `pw` name space:
+
+```python
+    spec.expose_inputs(
+        PwBaseWorkChain,
+        namespace='nscf',
+        exclude=('clean_workdir', 'pw.structure', 'pw.parent_folder'),
+        namespace_options={
+            'help': 'Inputs for the `PwBaseWorkChain` of the `nscf` calculation.',
+            'validator': validate_nscf
+        }
+    )
+```
+
+A new calculation function `create_magnetic_configuration` is added, which can be used to create a new `StructureData` with the required kinds for a specific magnetic configuration.
+For example, for an HCP structure with two Co sites:
+
+```python
+In [1]: from aiida import orm
+
+In [2]: from ase.build import bulk
+   ...: structure = orm.StructureData(ase=bulk('Co', 'hcp', 2.5, 4.06))
+```
+
+The `create_magnetic_configuration` can be used to quickly create a new `StructureData` with two different kinds:
+
+```python
+In [3]: from aiida_quantumespresso.calculations.functions.create_magnetic_configuration import create_magnetic_configuration
+   ...:
+   ...: results = create_magnetic_configuration(structure, [-2, 2])
+
+In [4]: results['structure'].sites
+Out[4]:
+[<Site: kind name 'Co0' @ -2.7755575615629e-17,1.4433756729741,2.03>,
+ <Site: kind name 'Co1' @ 0.0,0.0,0.0>]
+
+In [5]: results['magnetic_moments'].get_dict()
+Out[5]: {'Co0': 2, 'Co1': -2}
+```
+
+For more information, see the tutorial on how to work with magnetic systems:
+
+https://aiida-quantumespresso.readthedocs.io/en/latest/tutorials/magnetism.html
+
+The release also makes an important change in the dependencies related to a bug introduced in `pydantic`, see:
+
+https://github.com/pydantic/pydantic/issues/5821
+
+Hence the version of `pydantic` is adapted to `1.10.8`, where this bug is fixed.
+
+### ‼️ Breaking changes
+
+* `PwCalculation`: refactor `parent_folder` validation [[a389629](https://github.com/aiidateam/aiida-quantumespresso/commit/a389629387b74805ffe2f4d6515ac05b8f62b4d5)]
+
+### ✨ New features
+
+* Add the `create_magnetic_configuration` function [[d9b18a7](https://github.com/aiidateam/aiida-quantumespresso/commit/d9b18a7c20ce023018755c202f8d06cbf8bd27c5)]
+
+### 👌 Improvements
+
+* `PpParser`: Include exception in `ERROR_OUTPUT_DATAFILE_PARSE` message [[72f114e](https://github.com/aiidateam/aiida-quantumespresso/commit/72f114e4b05b45297abf0954b6334f5a461ed17e)]
+
+### 🐛 Bug Fixes
+
+* `PwParser`: Fix case when `settings` are not provided [[5d4a7d9](https://github.com/aiidateam/aiida-quantumespresso/commit/5d4a7d9405b757e2ecf65a72c1ee92aa2fb36a39)]
+
+### 📚 Documentation
+
+* Small improvements to "Installation" page [[90ad1d6](https://github.com/aiidateam/aiida-quantumespresso/commit/90ad1d6026d3c4b557970d6cc7626e85195ca4dc)]
+* Switch to `sphinx-book-theme` from `pydata_sphinx_theme` [[3578a9d](https://github.com/aiidateam/aiida-quantumespresso/commit/3578a9d08af5e8cdd0851f852185bce2f2c7bd51)]
+* Switch to using MyST Markdown [[37d2a14](https://github.com/aiidateam/aiida-quantumespresso/commit/37d2a14256480785491429c4ca424ebdc258ae34)]
+* Add how-to for `PwCalculationTools.get_scf_accuracy` [[29b4db9](https://github.com/aiidateam/aiida-quantumespresso/commit/29b4db9e5c0d225331aba58981663ad4af641640)]
+* Bump Python version for RTD build [[483d99b](https://github.com/aiidateam/aiida-quantumespresso/commit/483d99b77ca26ce4c607440922b432e39c16d1cf)]
+* Fix breaking changes `CHANGELOG.md` [[7f4c4a1](https://github.com/aiidateam/aiida-quantumespresso/commit/7f4c4a108b09c31cfc9ee252d7e8fbe574ea477f)]
+
+### 🔧 Maintenance
+
+* Catch warning in `restart_mode` test for `PwBaseWorkChain` [[45e1907](https://github.com/aiidateam/aiida-quantumespresso/commit/45e19072f28d30fb4d6df1bbc489f38ce94cd1be)]
+* Update `tox` configuration [[0702152](https://github.com/aiidateam/aiida-quantumespresso/commit/0702152c1dc18fd8d04cbf44f99a15761be955fe)]
+* Add script to update `CHANGELOG.md` [[b21076c](https://github.com/aiidateam/aiida-quantumespresso/commit/b21076cdd1773fe3b7de18bc83e89ec7b367d837)]
+* Remove Python 3.8 from the nightly workflow matrix [[0859d0a](https://github.com/aiidateam/aiida-quantumespresso/commit/0859d0a05c495c8a92208d118da6066f385600a7)]
+
+### ⬆️ Update dependencies
+
+* Restrict `pydantic` to at least `1.10.8` [[f430139](https://github.com/aiidateam/aiida-quantumespresso/commit/f430139e36723f73253efa66a6444018123760d2)]
+
+### ♻️ Refactor
+
+* `BasePwCpInputGenerator`: Remove superfluous validation [[0b6476c](https://github.com/aiidateam/aiida-quantumespresso/commit/0b6476c6c8379a0ea6575f4323979d136f7220aa)]
+*  Move basic parsing into `BaseParser` class [[1c223c7](https://github.com/aiidateam/aiida-quantumespresso/commit/1c223c78f0a2eda38089a08d9f21626f49d2fd6b)]
+
 ## v4.3.0
 
 Release version `4.3.0` comes with a lot of new features, improvements and bug fixes.
 Although this is technically a minor release, this new version does come with some _minor_ breaking changes:
 
 * The default value of `clean_workdir` was changed from `True` to `False`.
 * The `automatic_parallelization` feature of the `PwBaseWorkChain` was removed, as this was badly broken with no clear path to fixing it. Moreover, [v7.1 of Quantum ESPRESSO](https://gitlab.com/QEF/q-e/-/releases/qe-7.1) has implemented some basic automated parallelization for `pw.x` when no parallelization flags are specified.
+* Work chains no longer set/override static inputs inside the steps of their outline. All defaults are moved to the protocol files instead, and it is recommended to always use the `get_builder_from_protocol()` method to run a work chain. For more details, [see the corresponding PR](https://github.com/aiidateam/aiida-quantumespresso/pull/902).
 
 Support for Quantum ESPRESSO v7.2 `pw.x` parsing was added, as well as the `HubbardStructureData` data plugin and corresponding implementation in the `PwCalculation` plugin to support the [new input syntax for using Hubbard corrections](https://gitlab.com/QEF/q-e/-/releases/qe-7.1#incompatible-changes-in-71-version) in the `pw.x` code.
 
 For `ph.x`, the symmetry labels printed in the `stdout` after the mode frequencies are now parsed for each q-point.
 In the case of restarts in the `PhBaseWorkChain`, care has been taken to properly parse these symmetry labels from the separate output files and merge them, so the `output_parameters` are the same with or without restarts.
 
 The `XpsWorkChain` has been added to compute the XPS spectra using core-hole pseudo potentials and the `pw.x` code. The work chain can handle both molecules and crystals. The chemical shifts, as well as the cole-level binding energy can be obtained.
 
 Finally, improved error handling for the `PwBaseWorkChain` was implemented for several typical failure modes of the `pw.x` code, and the `CRASH` file is now also retrieved, as this will be the default location of error messages from Quantum ESPRESSO v7.2 onwards.
 
 ### ‼️ Breaking changes
 
 * Protocols: Set `clean_workdir` default to `False` [[f8e512f](https://github.com/aiidateam/aiida-quantumespresso/commit/f8e512f9cb5404d702aa1d721e2369c7257f977f)]
 * `PwBaseWorkChain`: Remove `automatic_parallelization` input [[5cae75f](https://github.com/aiidateam/aiida-quantumespresso/commit/5cae75ff671268dc1e5684e1c84f801a10839e0b)]
+* Protocols: Move all static work chain inputs to protocol [[01f1470](https://github.com/aiidateam/aiida-quantumespresso/commit/01f14701e6846338f84db25bf7e654fcdfb6f927)]
 
 ### ✨ New features
 
 * `PwBaseWorkChain`: Add `ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY` handler [[9291f84](https://github.com/aiidateam/aiida-quantumespresso/commit/9291f841445800fa2b38d97b6957e98a2818b624)]
 * `PwCalculation`: Add exit code and handler for `scale_h` error [[d350d7e](https://github.com/aiidateam/aiida-quantumespresso/commit/d350d7eb5b7bfcf4682ee8f635c721708be1d1d7)]
 * `PwParser`: Add retrieval and parsing of `CRASH` file [[7f53c96](https://github.com/aiidateam/aiida-quantumespresso/commit/7f53c96bf744ed622fe7b1d13b0f7e9198ed5656)]
 * Add the `HubbardStructureData` data plugin [[355020c](https://github.com/aiidateam/aiida-quantumespresso/commit/355020ca9ea63db0803ecc5746f93a879f488696)]
@@ -63,15 +167,14 @@
 
 ### ⬆️ Update dependencies
 * Symlink `CRASH` and `data-file.xml` files, and reduce fixture file contents [[0a48533](https://github.com/aiidateam/aiida-quantumespresso/commit/0a48533f40e276e5423428e0ca9745bd0b789121)]
 * Devops: Update `pylint` version [[9f4142d](https://github.com/aiidateam/aiida-quantumespresso/commit/9f4142d4713b0d1c32042b3ca35905d725954bf4)]
 
 ### ♻️ Refactor
 * Update `pylint` version [[9f4142d](https://github.com/aiidateam/aiida-quantumespresso/commit/9f4142d4713b0d1c32042b3ca35905d725954bf4)]
-* Protocols: Move all static work chain inputs to protocol [[01f1470](https://github.com/aiidateam/aiida-quantumespresso/commit/01f14701e6846338f84db25bf7e654fcdfb6f927)]
 
 
 ## v4.2.0
 
 ### Features
 - Add the `XspectraBaseWorkChain` [[#854]](https://github.com/aiidateam/aiida-quantumespresso/pull/854)
 - Add the `XspectraCoreWorkChain` [[#872]](https://github.com/aiidateam/aiida-quantumespresso/pull/872)
```

### Comparing `aiida-quantumespresso-4.3.0/LICENSE.txt` & `aiida_quantumespresso-4.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/README.md` & `aiida_quantumespresso-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/pyproject.toml` & `aiida_quantumespresso-4.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,34 +24,35 @@
 dependencies = [
     'aiida_core[atomic_tools]~=2.3',
     'aiida-pseudo~=1.0',
     'click~=8.0',
     'importlib_resources',
     'jsonschema',
     'numpy',
-    'pydantic',
+    'pydantic~=1.10,>=1.10.8',
     'packaging',
     'qe-tools~=2.0',
     'xmlschema~=1.2,>=1.2.5'
 ]
 
 [project.urls]
 Home = 'https://github.com/aiidateam/aiida-quantumespresso'
 Source = 'https://github.com/aiidateam/aiida-quantumespresso'
 Documentation = 'https://aiida-quantumespresso.readthedocs.io'
 
 [project.optional-dependencies]
 docs = [
-    'sphinx~=4.1',
-    'sphinx-copybutton~=0.5.0',
-    'sphinx-book-theme~=0.3.2',
-    'sphinx-click~=4.0',
-    'sphinx-design~=0.0.13',
+    'sphinx~=6.2.1',
+    'sphinx-copybutton~=0.5.2',
+    'sphinx-book-theme~=1.0.1',
+    'sphinx-click~=4.4.0',
+    'sphinx-design~=0.4.1',
     'sphinxcontrib-details-directive~=0.1.0',
-    'sphinx-autoapi',
+    'sphinx-autoapi~=2.0.1',
+    'myst_parser~=1.0.0',
 ]
 pre-commit = [
     'pre-commit~=2.17',
     'pylint~=2.17.2',
     'pylint-aiida~=0.1.1',
     'toml',
 ]
@@ -63,14 +64,15 @@
 
 [project.scripts]
 aiida-quantumespresso = 'aiida_quantumespresso.cli:cmd_root'
 
 [project.entry-points.'aiida.calculations']
 'quantumespresso.cp' = 'aiida_quantumespresso.calculations.cp:CpCalculation'
 'quantumespresso.create_kpoints_from_distance' = 'aiida_quantumespresso.calculations.functions.create_kpoints_from_distance:create_kpoints_from_distance'
+'quantumespresso.create_magnetic_configuration' = 'aiida_quantumespresso.calculations.functions.create_magnetic_configuration:create_magnetic_configuration'
 'quantumespresso.merge_ph_outputs' = 'aiida_quantumespresso.calculations.functions.merge_ph_outputs:merge_ph_outputs'
 'quantumespresso.dos' = 'aiida_quantumespresso.calculations.dos:DosCalculation'
 'quantumespresso.epw' = 'aiida_quantumespresso.calculations.epw:EpwCalculation'
 'quantumespresso.matdyn' = 'aiida_quantumespresso.calculations.matdyn:MatdynCalculation'
 'quantumespresso.namelists' = 'aiida_quantumespresso.calculations.namelists:NamelistsCalculation'
 'quantumespresso.neb' = 'aiida_quantumespresso.calculations.neb:NebCalculation'
 'quantumespresso.ph' = 'aiida_quantumespresso.calculations.ph:PhCalculation'
@@ -209,34 +211,24 @@
 dedent_closing_brackets = true
 indent_dictionary_value = false
 split_arguments_when_comma_terminated = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py37
+envlist =
+    py{38,39,310,311}
+    py38-pre-commit
 
 [testenv]
+description = Run the pytest tests
 usedevelop=True
-
-[testenv:py{36,37,38,39}]
 extras = tests
 commands = pytest {posargs}
 
 [testenv:py38-pre-commit]
 description = Run the pre-commit checks
 extras =
     tests
     pre-commit
 commands = pre-commit run {posargs}
-
-[testenv:py38-docs-{clean,update}]
-description =
-    clean: Build the documentation (remove any existing build)
-    update: Build the documentation (modify any existing build)
-extras = docs
-changedir = docs
-whitelist_externals = make
-commands =
-    clean: make clean
-    make
 """
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/__init__.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,30 @@
                     for flag_name in cls._ENABLED_PARALLELIZATION_FLAGS
                 )
             ),
             validator=cls.validate_parallelization
         )
         spec.inputs.validator = cls.validate_inputs
 
+        spec.exit_code(
+            302,
+            'ERROR_OUTPUT_STDOUT_MISSING',
+            message='The retrieved folder did not contain the required stdout output file.'
+        )
+        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ', message='The stdout output file could not be read.')
+        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE', message='The stdout output file could not be parsed.')
+        spec.exit_code(
+            312,
+            'ERROR_OUTPUT_STDOUT_INCOMPLETE',
+            message='The stdout output file was incomplete probably because the calculation got interrupted.'
+        )
+        spec.exit_code(
+            400, 'ERROR_OUT_OF_WALLTIME', message='The calculation stopped prematurely because it ran out of walltime.'
+        )
+
     @classmethod
     def validate_inputs(cls, value, port_namespace):
         """Validate the entire inputs namespace."""
 
         # Wrapping processes may choose to exclude certain input ports in which case we can't validate. If the ports
         # have been excluded, and so are no longer part of the ``port_namespace``, skip the validation.
         if any(key not in port_namespace for key in ('pseudos', 'structure')):
@@ -209,24 +225,14 @@
         """
         # pylint: disable=too-many-branches,too-many-statements
         if 'settings' in self.inputs:
             settings = _uppercase_dict(self.inputs.settings.get_dict(), dict_name='settings')
         else:
             settings = {}
 
-        # Check that a pseudo potential was specified for each kind present in the `StructureData`
-        kinds = [kind.name for kind in self.inputs.structure.kinds]
-        if set(kinds) != set(self.inputs.pseudos.keys()):
-            formatted_pseudos = ', '.join(list(self.inputs.pseudos.keys()))
-            formatted_kinds = ', '.join(list(kinds))
-            raise exceptions.InputValidationError(
-                'Mismatch between the defined pseudos and the list of kinds of the structure.\n'
-                f'Pseudos: {formatted_pseudos};\nKinds: {formatted_kinds}'
-            )
-
         local_copy_list = []
         remote_copy_list = []
         remote_symlink_list = []
 
         # Create the subfolder that will contain the pseudopotentials
         folder.get_subfolder(self._PSEUDO_SUBFOLDER, create=True)
         # Create the subfolder for the output data (sometimes Quantum ESPRESSO codes crash if the folder does not exist)
@@ -536,20 +542,14 @@
             '{0} {1:18.10f} {2:18.10f} {3:18.10f}'.format(site.kind_name.ljust(6), *site_coords)  # pylint: disable=consider-using-f-string
             for site, site_coords in zip(structure.sites, coordinates)
         ]
 
         fixed_coords = settings.pop('FIXED_COORDS', None)
 
         if fixed_coords is not None:
-            # Note that this check is also in the validation of the top-level namespace, but this is only checked in
-            # in case the structure is provided
-            if len(fixed_coords) != len(structure.sites):
-                raise exceptions.InputValidationError(
-                    f'Input structure has {len(structure.sites)} sites, but fixed_coords has length {len(fixed_coords)}'
-                )
             fixed_coords_strings = [
                 ' {:d} {:d} {:d}'.format(*row) for row in numpy.int32(numpy.invert(fixed_coords)).tolist()  # pylint: disable=consider-using-f-string
             ]
             atomic_positions_card_list = [
                 atomic_pos_str + fixed_coords_str
                 for atomic_pos_str, fixed_coords_str in zip(atomic_positions_card_list, fixed_coords_strings)
             ]
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/cp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/cp.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,20 +127,14 @@
 
         spec.exit_code(301, 'ERROR_NO_RETRIEVED_TEMPORARY_FOLDER',
             message='The retrieved temporary folder could not be accessed.')
         spec.exit_code(303, 'ERROR_MISSING_XML_FILE',
             message='The required XML file is not present in the retrieved folder.')
         spec.exit_code(304, 'ERROR_OUTPUT_XML_MULTIPLE',
             message='The retrieved folder contains multiple XML files.')
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
-            message='The output file contains invalid output.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(320, 'ERROR_OUTPUT_XML_READ',
             message='The required XML file could not be read.')
         spec.exit_code(330, 'ERROR_READING_POS_FILE',
             message='The required POS file could not be read.')
         spec.exit_code(340, 'ERROR_READING_TRAJECTORY_DATA',
             message='The required trajectory data could not be read.')
         # yapf: enable
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/dos.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/dos.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,14 +23,10 @@
         """Define the process specification."""
         # yapf: disable
         super().define(spec)
         spec.input('parent_folder', valid_type=(orm.RemoteData, orm.FolderData), required=True)
         spec.output('output_parameters', valid_type=orm.Dict)
         spec.output('output_dos', valid_type=orm.XyData)
         spec.default_output_node = 'output_parameters'
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(330, 'ERROR_READING_DOS_FILE',
             message='The dos file could not be read from the retrieved folder.')
         # yapf: enable
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/epw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/epw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/__init__.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/matdyn.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/matdyn.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,18 +33,14 @@
         spec.input('kpoints', valid_type=orm.KpointsData, help='Kpoints on which to calculate the phonon frequencies.')
         spec.inputs.validator = cls._validate_inputs
 
         spec.output('output_parameters', valid_type=orm.Dict)
         spec.output('output_phonon_bands', valid_type=orm.BandsData)
         spec.default_output_node = 'output_parameters'
 
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(330, 'ERROR_OUTPUT_FREQUENCIES',
             message='The output frequencies file could not be read from the retrieved folder.')
         spec.exit_code(410, 'ERROR_OUTPUT_KPOINTS_MISSING',
             message='Number of kpoints not found in the output data')
         spec.exit_code(411, 'ERROR_OUTPUT_KPOINTS_INCOMMENSURATE',
             message='Number of kpoints in the inputs is not commensurate with those in the output')
         # yapf: enable
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/namelists.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/namelists.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,22 @@
             spec.input('metadata.options.parser_name', valid_type=str, default=cls._default_parser)
         spec.input('parameters', valid_type=Dict, required=False,
             help='Parameters for the namelists in the input file.')
         spec.input('settings', valid_type=Dict, required=False,
             help='Use an additional node for special settings')
         spec.input('parent_folder', valid_type=(RemoteData, FolderData, SinglefileData), required=False,
             help='Use a local or remote folder as parent folder (for restarts and similar)')
+        spec.exit_code(302, 'ERROR_OUTPUT_STDOUT_MISSING',
+            message='The retrieved folder did not contain the required stdout output file.')
+        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
+            message='An exception was raised while reading the `stdout` file: {exception}')
+        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
+            message='An exception was raised while parsing the `stdout` file: {exception}')
+        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
+            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         # yapf: enable
 
     @classmethod
     def set_blocked_keywords(cls, parameters):
         """Force default values for blocked keywords. NOTE: this is different from PW/CP."""
         for blocked in cls._blocked_keywords:
             namelist = blocked[0].upper()
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/neb.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/neb.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,20 +74,14 @@
         spec.output('output_trajectory', valid_type=orm.TrajectoryData)
         spec.output('iteration_array', valid_type=orm.ArrayData, required=False)
         spec.output('output_mep', valid_type=orm.ArrayData,
             help='The original and interpolated energy profiles along the minimum-energy path (mep)')
         spec.default_output_node = 'output_parameters'
         spec.exit_code(303, 'ERROR_MISSING_XML_FILE',
             message='The required XML file is not present in the retrieved folder.')
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
-            message='The output file contains invalid output.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(320, 'ERROR_OUTPUT_XML_READ',
             message='The XML output file could not be read.')
         spec.exit_code(321, 'ERROR_OUTPUT_XML_PARSE',
             message='The XML output file could not be parsed.')
         spec.exit_code(322, 'ERROR_OUTPUT_XML_FORMAT',
             message='The XML output file has an unsupported format.')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/open_grid.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/open_grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,11 @@
         spec.input('parent_folder', valid_type=(RemoteData, FolderData),
             help='The output folder of a completed `PwCalculation` on an irreducible Brillouin zone')
         spec.output('kpoints_mesh', valid_type=KpointsData, help='The dimensions of the unfolded kmesh')
         spec.output('kpoints', valid_type=KpointsData, help='The explicit list of kpoints of the unfolded kmesh')
 
         spec.exit_code(300, 'ERROR_NO_RETRIEVED_FOLDER',
             message='The retrieved folder data node could not be accessed.')
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(312, 'ERROR_INCOMPATIBLE_FFT_GRID',
             message='Found rotation or fractional translation not compatible with FFT grid.')
-        spec.exit_code(340, 'ERROR_GENERIC_QE_ERROR',
-            message='Encountered a generic error message.')
         spec.exit_code(350, 'ERROR_OUTPUT_KPOINTS_MISMATCH',
             message='Mismatch between kmesh dimensions and number of kpoints.')
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/ph.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/ph.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pp.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
             message='The retrieved temporary folder could not be accessed.')
         spec.exit_code(302, 'ERROR_OUTPUT_STDOUT_MISSING',
             message='The retrieved folder did not contain the required stdout output file.')
         spec.exit_code(303, 'ERROR_OUTPUT_XML_MISSING',
             message='The parent folder did not contain the required XML output file.')
         spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
             message='The stdout output file could not be read.')
+        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
+            message='The stdout output file could not be parsed.')
         spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
             message='The stdout output file was incomplete.')
         spec.exit_code(340, 'ERROR_OUT_OF_WALLTIME_INTERRUPTED',
             message='The calculation stopped prematurely because it ran out of walltime but the job was killed by the '
                     'scheduler before the files were safely written to disk for a potential restart.')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
             message='The parser raised an unexpected exception: {exception}')
@@ -110,15 +112,15 @@
         spec.exit_code(330, 'ERROR_OUTPUT_DATAFILE_MISSING',
             message='The formatted data output file `{filename}` was not present in the retrieved (temporary) folder.')
         spec.exit_code(331, 'ERROR_OUTPUT_DATAFILE_READ',
             message='The formatted data output file `{filename}` could not be read.')
         spec.exit_code(332, 'ERROR_UNSUPPORTED_DATAFILE_FORMAT',
             message='The data file format is not supported by the parser')
         spec.exit_code(333, 'ERROR_OUTPUT_DATAFILE_PARSE',
-            message='The formatted data output file `{filename}` could not be parsed')
+            message='The formatted data output file `{filename}` could not be parsed: {exception}')
         # yapf: enable
 
     def prepare_for_submission(self, folder):  # pylint: disable=too-many-branches,too-many-statements
         """Prepare the calculation job for submission by transforming input nodes into input files.
 
         In addition to the input files being written to the sandbox folder, a `CalcInfo` instance will be returned that
         contains lists of files that need to be copied to the remote machine before job submission, as well as file
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/projwfc.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/projwfc.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,18 +58,14 @@
         spec.output('projections', valid_type=ProjectionData, required=False)
         spec.output('bands', valid_type=BandsData, required=False)
         spec.default_output_node = 'output_parameters'
         spec.exit_code(301, 'ERROR_NO_RETRIEVED_TEMPORARY_FOLDER',
             message='The retrieved temporary folder could not be accessed.')
         spec.exit_code(303, 'ERROR_OUTPUT_XML_MISSING',
             message='The retrieved folder did not contain the required XML file.')
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(320, 'ERROR_OUTPUT_XML_READ',
             message='The XML output file could not be read.')
         spec.exit_code(321, 'ERROR_OUTPUT_XML_PARSE',
             message='The XML output file could not be parsed.')
         spec.exit_code(322, 'ERROR_OUTPUT_XML_FORMAT',
             message='The XML output file has an unsupported format.')
         spec.exit_code(330, 'ERROR_READING_PDOSTOT_FILE',
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pw.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,28 +83,20 @@
         spec.output('output_kpoints', valid_type=orm.KpointsData, required=False)
         spec.output('output_atomic_occupations', valid_type=orm.Dict, required=False)
         spec.default_output_node = 'output_parameters'
 
         # Unrecoverable errors: required retrieved files could not be read, parsed or are otherwise incomplete
         spec.exit_code(301, 'ERROR_NO_RETRIEVED_TEMPORARY_FOLDER',
             message='The retrieved temporary folder could not be accessed.')
-        spec.exit_code(302, 'ERROR_OUTPUT_STDOUT_MISSING',
-            message='The retrieved folder did not contain the required stdout output file.')
         spec.exit_code(303, 'ERROR_OUTPUT_XML_MISSING',
             message='The retrieved folder did not contain the required XML file.')
         spec.exit_code(304, 'ERROR_OUTPUT_XML_MULTIPLE',
             message='The retrieved folder contained multiple XML files.')
         spec.exit_code(305, 'ERROR_OUTPUT_FILES',
             message='Both the stdout and XML output files could not be read or parsed.')
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
-            message='The stdout output file could not be parsed.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(320, 'ERROR_OUTPUT_XML_READ',
             message='The XML output file could not be read.')
         spec.exit_code(321, 'ERROR_OUTPUT_XML_PARSE',
             message='The XML output file could not be parsed.')
         spec.exit_code(322, 'ERROR_OUTPUT_XML_FORMAT',
             message='The XML output file has an unsupported format.')
         spec.exit_code(340, 'ERROR_OUT_OF_WALLTIME_INTERRUPTED',
@@ -112,16 +104,14 @@
                     'scheduler before the files were safely written to disk for a potential restart.')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
             message='The parser raised an unexpected exception: {exception}')
         spec.exit_code(360, 'ERROR_G_PAR',
             message='The code failed in finding a valid reciprocal lattice vector.')
 
         # Significant errors but calculation can be used to restart
-        spec.exit_code(400, 'ERROR_OUT_OF_WALLTIME',
-            message='The calculation stopped prematurely because it ran out of walltime.')
         spec.exit_code(410, 'ERROR_ELECTRONIC_CONVERGENCE_NOT_REACHED',
             message='The electronic minimization cycle did not reach self-consistency.')
 
         spec.exit_code(461, 'ERROR_DEXX_IS_NEGATIVE',
             message='The code failed with negative dexx in the exchange calculation.')
         spec.exit_code(462, 'ERROR_COMPUTING_CHOLESKY',
             message='The code failed during the cholesky factorization.')
@@ -172,69 +162,62 @@
 
         # Strong warnings about calculation results, but something tells us that you're ok with that
         spec.exit_code(710, 'WARNING_ELECTRONIC_CONVERGENCE_NOT_REACHED',
             message='The electronic minimization cycle did not reach self-consistency, but `scf_must_converge` '
                     'is `False` and/or `electron_maxstep` is 0.')
         # yapf: enable
 
-    @staticmethod
-    def validate_inputs_base(value, _):
-        """Validate the top level namespace."""
+    @classmethod
+    def validate_inputs(cls, value, port_namespace):
+        """Validate the top level namespace.
+
+        Check that the restart input parameters are set correctly. In case of 'nscf' and 'bands' calculations, this
+        means ``parent_folder`` is provided. For other calculations, if the ``parent_folder`` is provided, the restart
+        settings must be set to use some of the outputs.
+
+        Note that the validator will only check the logic in case the ``parent_folder`` is a port in the
+        ``port_namespace``. This is because the ``PwCalculation`` can be wrapped inside a work chain that only provides
+        the ``parent_folder`` input at a later step in the outline. To avoid raising any warnings, such a work chain
+        must exclude the ``parent_folder`` port when exposing the inputs of the ``PwCalculation``.
+        """
+        result = super().validate_inputs(value, port_namespace)
+
+        if result is not None:
+            return result
+
         parameters = value['parameters'].get_dict()
         calculation_type = parameters.get('CONTROL', {}).get('calculation', 'scf')
 
+        if 'parent_folder' not in port_namespace:
+            return
+
         # If a `parent_folder` input is provided, make sure the inputs are set to restart
         if 'parent_folder' in value and calculation_type not in ('nscf', 'bands'):
             if not any([
                 parameters.get('CONTROL', {}).get('restart_mode', None) == 'restart',
                 parameters.get('ELECTRONS', {}).get('startingpot', None) == 'file',
                 parameters.get('ELECTRONS', {}).get('startingwfc', None) == 'file'
             ]):
                 warnings.warn(
-                    f'`parent_folder` input was provided for the `{calculation_type}` `PwCalculation`, but no input'
+                    f'`parent_folder` input was provided for the `{calculation_type}` `PwCalculation`, but no input '
                     'parameters were provided to restart from this folder.\n\n'
                     'Please set one of the following in the input parameters:\n'
                     "    parameters['CONTROL']['restart_mode'] = 'restart'\n"
                     "    parameters['ELECTRONS']['startingpot'] = 'file'\n"
                     "    parameters['ELECTRONS']['startingwfc'] = 'file'\n"
                 )
 
-    @classmethod
-    def validate_inputs(cls, value, port_namespace):
-        """Validate the top level namespace.
-
-        Check that the restart input parameters are set correctly. In case of 'nscf' and 'bands' calculations, this
-        means ``parent_folder`` is provided. For other calculations, if the ``parent_folder`` is provided, the restart
-        settings must be set to use some of the outputs.
-
-        Note that the validator is split in two methods: ``validate_inputs`` and ``validate_inputs_base``. This is to
-        facilitate work chains that wrap this calculation that will provide the ``parent_folder`` themselves and so do
-        not require the user to provide it at launch of the work chain. This will fail because of the validation in this
-        validator, however, which is why the rest of the logic is moved to ``validate_inputs_base``. The wrapping work
-        chain can change the ``validate_input`` validator for ``validate_inputs_base`` thereby allowing the parent
-        folder to be defined during the work chains runtime, while still keep the rest of the namespace validation.
-        """
-        result = super().validate_inputs(value, port_namespace)
-
-        if result is not None:
-            return result
-
-        parameters = value['parameters'].get_dict()
-        calculation_type = parameters.get('CONTROL', {}).get('calculation', 'scf')
-
         if calculation_type in ('nscf', 'bands'):
             if 'parent_folder' not in value:
                 warnings.warn(
                     f'`parent_folder` not provided for `{calculation_type}` calculation. For work chains wrapping this '
-                    'calculation, you can disable this warning by setting the validator of the `PwCalculation` port to '
-                    '`PwCalculation.validate_inputs_base`.'
+                    'calculation, you can disable this warning by excluding the `parent_folder` when exposing the '
+                    'inputs of the `PwCalculation`.'
                 )
 
-        return cls.validate_inputs_base(value, port_namespace)
-
     @classproperty
     def filename_input_hubbard_parameters(cls):
         """Return the relative file name of the file containing the Hubbard parameters.
 
         .. note:: This only applies if they should be read from file instead of specified in the input file cards.
         .. warning:: Requires the aiida-quantumespresso-hp plugin to be installed
         """
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2gw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pw2gw.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,24 +34,16 @@
             help='Output folder of a completed `PwCalculation`')
 
         spec.output('output_parameters', valid_type=orm.Dict,
             help='The `output_parameters` output node of the successful calculation.`')
         spec.output('eps', valid_type=orm.ArrayData,
             help='The `eps` output node containing 5 arrays `energy`, `epsX`, `epsY`, `epsZ`, `epsTOT`')
 
-        spec.exit_code(302, 'ERROR_OUTPUT_STDOUT_MISSING',
-            message='The retrieved folder did not contain the required stdout output file.')
         spec.exit_code(305, 'ERROR_OUTPUT_FILES',
             message='The eps*.dat output files could not be read or parsed.')
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
-            message='The stdout output file could not be parsed.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(330, 'ERROR_OUTPUT_FILES_INVALID_FORMAT',
             message='The eps*.dat output files do not have the expected shape (N, 2).')
         spec.exit_code(331, 'ERROR_OUTPUT_FILES_ENERGY_MISMATCH',
             message='The eps*.dat output files contains different values of energies.')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
             message='The parser raised an unexpected exception: {exception}')
         # yapf: enable
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2wannier90.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pw2wannier90.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,18 +27,14 @@
         super().define(spec)
         spec.input('nnkp_file', valid_type=SinglefileData,
                    help='A SinglefileData containing the .nnkp file generated by wannier90.x -pp')
         spec.input('parent_folder', valid_type=(RemoteData, FolderData),
                    help='The output folder of a pw.x calculation')
         spec.output('output_parameters', valid_type=Dict)
         spec.default_output_node = 'output_parameters'
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(340, 'ERROR_GENERIC_QE_ERROR',
             message='Encountered a generic error message')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
             message='The parser raised an unexpected exception: {exception}')
         # yapf: enable
 
     def prepare_for_submission(self, folder):
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pwimmigrant.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/pwimmigrant.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/q2r.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/q2r.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,14 +28,10 @@
     @classmethod
     def define(cls, spec):
         """Define the process specification."""
         # yapf: disable
         super().define(spec)
         spec.input('parent_folder', valid_type=(orm.RemoteData, orm.FolderData), required=True)
         spec.output('force_constants', valid_type=ForceConstantsData)
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ',
-            message='The stdout output file could not be read.')
-        spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(330, 'ERROR_READING_FORCE_CONSTANTS_FILE',
             message='The force constants file could not be read.')
         # yapf: enable
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/xspectra.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/calculations/xspectra.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,20 +57,14 @@
             ' `gamma_mode=file`'
         )
 
         spec.output('output_parameters', valid_type=Dict)
         spec.output('spectra', valid_type=XyData)
         spec.default_output_node = 'output_parameters'
 
-        spec.exit_code(310, 'ERROR_OUTPUT_STDOUT_READ', message='The stdout output file could not be read.')
-        spec.exit_code(
-            312,
-            'ERROR_OUTPUT_STDOUT_INCOMPLETE',
-            message='The stdout output file was incomplete probably because the calculation got interrupted.'
-        )
         spec.exit_code(
             313,
             'ERROR_OUTPUT_ABSORBING_SPECIES_WRONG',
             message='xiabs was set incorrectly, check and ensure that the index value correctly refers '
             'to the atomic species containing the core-hole (where the index starts from 1).'
         )
         spec.exit_code(
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/__init__.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/__init__.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/cp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/cp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/dos.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/dos.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/epw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/epw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/matdyn.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/matdyn.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/neb.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/neb.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/ph.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/ph.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/pp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/projwfc.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/pw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/q2r.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/calculations/q2r.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/data/structure.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/data/structure.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/defaults.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/display.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/display.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/launch.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/launch.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/options.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/options.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/validate.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/utils/validate.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/__init__.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/ph/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/ph/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/hubbard.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/common/hubbard.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return (
             self.atom_index, self.atom_manifold, self.neighbour_index, self.neighbour_manifold, self.value,
             self.translation, self.hubbard_type
         )
 
     @staticmethod
     def from_tuple(hubbard_parameters: Tuple[int, str, int, str, float, Tuple[int, int, int], str]):
-        """Return a :meth:`~aiida_quantumespresso.common.hubbard.HubbardParameters`  instance from a list.
+        """Return a ``HubbardParameters``  instance from a list.
 
         The parameters within the list must have the following order:
             * atom_index
             * atom_manifold
             * neighbour_index
             * neighbour_manifold
             * value
@@ -108,15 +108,15 @@
         return HubbardParameters(**dict(zip(keys, hubbard_parameters)))
 
 
 class Hubbard(BaseModel):
     """Class for complete description of Hubbard interactions."""
 
     parameters: List[HubbardParameters]
-    """List of :meth:`~aiida_quantumespress.common.hubbard.HubbardParameters`."""
+    """List of :class:`~aiida_quantumespresso.common.hubbard.HubbardParameters`."""
 
     projectors: Literal['atomic',
                         'ortho-atomic',
                         'norm-atomic',
                         'wannier-functions',
                         'pseudo-potentials',
                         ] = 'ortho-atomic'
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/types.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/common/types.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/force_constants.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/data/force_constants.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/hubbard_structure.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/data/hubbard_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,41 +26,41 @@
     ):
         """Set a ``HubbardStructureData`` instance.
 
         :param cell: (3,3) shape list of floats
         :param pbc: (3,) shape list in bools
         :param sites: list of lists, each of the shape [symbol, name, position],
             where position is a (3,) shape list of floats
-        :param hubbard: a :py:meth:`~aiida_quantumespresso.common.hubbrd.Hubbard` istance
+        :param hubbard: a :class:`~aiida_quantumespresso.common.hubbard.Hubbard` istance
         """
         super().__init__(cell=cell, **kwargs)
         self.sites = sites
         self.pbc = pbc
         self.hubbard = Hubbard(parameters=[]) if hubbard is None else hubbard
 
     @property
     def sites(self):
-        """Return the :meth:`aiida.core.Sites`."""
+        """Return the :attr:`~aiida.orm.nodes.data.structure.StructureData.sites`."""
         return super().sites
 
     @sites.setter
     def sites(self, values: List[Tuple[str, str, Tuple[float, float, float]]]):
-        """Set the :meth:`aiida.core.Sites`.
+        """Set the :attr:`~aiida.orm.nodes.data.structure.StructureData.sites`.
 
         :param values: list of sites, each as [symbol, name, (3,) shape list of positions]
         """
         self.clear_sites()
         for simbols, kind_name, position in values:
             self.append_atom(symbols=simbols, name=kind_name, position=position)
 
     @property
     def hubbard(self) -> Hubbard:
         """Get the `Hubbard` instance.
 
-        :returns: a :py:meth:`~aiida_quantumespresso.common.hubbard.Hubbard` instance.
+        :returns: a :class:`~aiida_quantumespresso.common.hubbard.Hubbard` instance.
         """
         with self.base.repository.open(self._hubbard_filename, mode='rb') as handle:
             return Hubbard.parse_raw(json.load(handle))
 
     @hubbard.setter
     def hubbard(self, hubbard: Hubbard):
         """Set the full Hubbard information."""
@@ -73,16 +73,16 @@
     @staticmethod
     def from_structure(
         structure: StructureData,
         hubbard: Union[Hubbard, None] = None,
     ):
         """Return an instance of ``HubbardStructureData`` from a ``StructureData`` node.
 
-        :param structure: :meth:`aiida.orm.StructureData` instance
-        :param hubbad: :meth:`~aiida_quantumespresso.common.hubbard.Hubbard` instance
+        :param structure: :class:`aiida.orm.StructureData` instance
+        :param hubbard: :class:`~aiida_quantumespresso.common.hubbard.Hubbard` instance
         :returns: ``HubbardStructureData`` instance
         """
         sites = [[structure.get_kind(site.kind_name).symbol, site.kind_name, site.position] for site in structure.sites]
         cell = structure.cell
         pbc = structure.pbc
 
         return HubbardStructureData(cell=cell, pbc=pbc, sites=sites, hubbard=hubbard)
@@ -93,25 +93,25 @@
         atom_manifold: str,
         neighbour_index: int,
         neighbour_manifold: str,
         value: float,
         translation: Tuple[int, int, int] = None,
         hubbard_type: str = 'Ueff',
     ):
-        """Append a :meth:`~aiida_quantumespresso.common.hubbard.HubbardParameters``.
+        """Append a :class:`~aiida_quantumespresso.common.hubbard.HubbardParameters`.
 
         :param atom_index: atom index in unitcell
         :param atom_manifold: atomic manifold (e.g. 3d, 3d-2p)
         :param neighbour_index: neighbouring atom index in unitcell
         :param neighbour_manifold: neighbour manifold (e.g. 3d, 3d-2p)
         :param value: value of the Hubbard parameter, in eV
         :param translation: (3,) list of ints, describing the translation vector
             associated with the neighbour atom, defaults to None
         :param hubbard_type: hubbard type (U, V, J, ...), defaults to 'Ueff'
-            (see :meth:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
+            (see :class:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
         """
         pymat = self.get_pymatgen_structure()
         sites = pymat.sites
 
         if translation is None:
             _, translation = sites[atom_index].distance_and_image(sites[neighbour_index])
             translation = np.array(translation, dtype=np.int64).tolist()
@@ -157,15 +157,15 @@
 
         :param atom_name: atom name in unitcell
         :param atom_manifold: atomic manifold (e.g. 3d, 3d-2p)
         :param neighbour_index: neighbouring atom name in unitcell
         :param neighbour_manifold: neighbour manifold (e.g. 3d, 3d-2p)
         :param value: value of the Hubbard parameter, in eV
         :param hubbard_type: hubbard type (U, V, J, ...), defaults to 'V'
-            (see :meth:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
+            (see :class:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
         :param use_kinds: whether to use kinds for initializing the parameters; when False, it
             initializes all the ``Kinds`` matching the ``atom_name``
         """
         sites = self.get_pymatgen_structure().sites
 
         function = self._get_one_kind_index if use_kinds else self._get_symbol_indices
         atom_indices = function(atom_name)
@@ -193,15 +193,15 @@
     ):
         """Initialize and append onsite Hubbard values of atoms with specific name.
 
         :param atom_name: atom name in unitcell
         :param atom_manifold: atomic manifold (e.g. 3d, 3d-2p)
         :param value: value of the Hubbard parameter, in eV
         :param hubbard_type: hubbard type (U, J, ...), defaults to 'Ueff'
-            (see :meth:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
+            (see :class:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
         :param use_kinds: whether to use kinds for initializing the parameters; when False, it
             initializes all the ``Kinds`` matching the ``atom_name``
         """
         function = self._get_one_kind_index if use_kinds else self._get_symbol_indices
         atom_indices = function(atom_name)
 
         if atom_indices is None:
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/cp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/cp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 # -*- coding: utf-8 -*-
 from aiida.orm import Dict, TrajectoryData
 import numpy
 from packaging.version import Version
 from qe_tools import CONSTANTS
 
-from .base import Parser
+from aiida_quantumespresso.utils.mapping import get_logging_container
+
+from .base import BaseParser
 from .parse_raw.cp import parse_cp_raw_output, parse_cp_traj_stanzas
 
 
-class CpParser(Parser):
+class CpParser(BaseParser):
     """This class is the implementation of the Parser class for Cp."""
 
     def parse(self, **kwargs):
         """Receives in input a dictionary of retrieved nodes.
 
         Does all the logic here.
         """
+        logs = get_logging_container()
+
+        stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
+
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
+
         retrieved = self.retrieved
 
         # check what is inside the folder
         list_of_files = retrieved.base.repository.list_object_names()
 
-        # options.metadata become attributes like this:
-        stdout_filename = self.node.base.attributes.get('output_filename')
-        # at least the stdout should exist
-        if stdout_filename not in list_of_files:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
-
         # This should match 1 file
         xml_files = [xml_file for xml_file in self.node.process_class.xml_filenames if xml_file in list_of_files]
         if not xml_files:
-            return self.exit(self.exit_codes.ERROR_MISSING_XML_FILE)
+            return self.exit(self.exit_codes.ERROR_MISSING_XML_FILE, logs)
         elif len(xml_files) > 1:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_XML_MULTIPLE)
+            return self.exit(self.exit_codes.ERROR_OUTPUT_XML_MULTIPLE, logs)
 
         # cp.x can produce, depending on the particular version of the code, a file called `print_counter.xml` or
         # `print_counter`, which is a plain text file with the number of the last timestep written in the trajectory
         # output. Note that if no trajectory is produced (for example because a single conjugate gradient step was
         # performed to calculate the ground state and the wavefunctions velocities) no printer_counter* file is written.
 
         print_counter_xml = True
@@ -59,19 +63,18 @@
                 print_counter_xml = False
                 filename_counter = filename_counter_txt
             else:  # xml format
                 print_counter_xml = True
                 self.logger.info('print counter in xml format')
                 filename_counter = filename_counter_xml
 
-        output_stdout = retrieved.base.repository.get_object_content(stdout_filename)
         output_xml = retrieved.base.repository.get_object_content(xml_files[0])
         output_xml_counter = None if no_trajectory_output else retrieved.base.repository.get_object_content(filename_counter)
         out_dict, _raw_successful = parse_cp_raw_output(
-            output_stdout, output_xml, output_xml_counter, print_counter_xml
+            stdout, output_xml, output_xml_counter, print_counter_xml
         )
 
         if not no_trajectory_output:
             # parse the trajectory. Units in Angstrom, picoseconds and eV.
             # append everthing in the temporary dictionary raw_trajectory
             raw_trajectory = {}
             evp_keys = [
@@ -251,17 +254,24 @@
         for key in [
             'atoms', 'cell', 'ions_positions_stau', 'ions_positions_svel', 'ions_positions_taui', 'atoms_index_list',
             'atoms_if_pos_list', 'ions_positions_force', 'bands', 'structure'
         ]:
             out_dict.pop(key, None)
 
         # convert the dictionary into an AiiDA object
+        out_dict.update(parsed_data)
         output_params = Dict(out_dict)
         self.out('output_parameters', output_params)
 
+        for exit_code in list(self.get_error_map().values()) + ['ERROR_OUTPUT_STDOUT_INCOMPLETE']:
+            if exit_code in logs.error:
+                return self.exit(self.exit_codes.get(exit_code), logs)
+
+        return self.exit(logs=logs)
+
     def get_linkname_trajectory(self):
         """Returns the name of the link to the output_structure (None if not present)"""
         return 'output_trajectory'
 
     def _generate_sites_ordering(self, raw_species, raw_atoms):
         """take the positions of xml and from file.pos of the LAST step and compare them."""
         # Examples in the comments are for species [Ba, O, Ti]
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/dos.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/dos.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 # -*- coding: utf-8 -*-
 from aiida.orm import Dict, XyData
 import numpy as np
 
 from aiida_quantumespresso.parsers import QEOutputParsingError
-from aiida_quantumespresso.parsers.parse_raw.base import parse_output_base
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
-class DosParser(Parser):
-    """This class is the implementation of the Parser class for Dos."""
+class DosParser(BaseParser):
+    """``Parser`` implementation for the ``DosCalculation`` calculation job class."""
 
     def parse(self, **kwargs):
-        """Parses the datafolder, stores results.
+        """Parse the retrieved files of a ``DosCalculation`` into output nodes."""
+        logs = get_logging_container()
 
-        Retrieves dos output, and some basic information from the out_file, such as warnings and wall_time
-        """
-        retrieved = self.retrieved
+        _, parsed_stdout, logs = self.parse_stdout_from_retrieved(logs)
 
-        # Read standard out
-        try:
-            filename_stdout = self.node.get_option('output_filename')  # or get_attribute(), but this is clearer
-            with retrieved.base.repository.open(filename_stdout, 'r') as fil:
-                out_file = fil.readlines()
-        except OSError:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
+
+        self.out('output_parameters', Dict(parsed_stdout))
 
-        job_done = False
-        for i in range(len(out_file)):
-            line = out_file[-i]
-            if 'JOB DONE' in line:
-                job_done = True
-                break
-        if not job_done:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE)
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
 
-        # check that the dos file is present, if it is, read it
+        # Parse the DOS
         try:
-            with retrieved.base.repository.open(self.node.process_class._DOS_FILENAME, 'r') as fil:
-                dos_file = fil.readlines()
+            with self.retrieved.base.repository.open(self.node.process_class._DOS_FILENAME, 'r') as handle:
+                dos_file = handle.readlines()
         except OSError:
-            return self.exit(self.exit_codes.ERROR_READING_DOS_FILE)
-
-        # end of initial checks
+            return self.exit(self.exit_codes.ERROR_READING_DOS_FILE, logs)
 
         array_names = [[], []]
         array_units = [[], []]
         array_names[0] = ['dos_energy', 'dos', 'integrated_dos']  # When spin is not displayed
         array_names[1] = ['dos_energy', 'dos_spin_up', 'dos_spin_down', 'integrated_dos']  # When spin is displayed
         array_units[0] = ['eV', 'states/eV', 'states']  # When spin is not displayed
         array_units[1] = ['eV', 'states/eV', 'states/eV', 'states']  # When spin is displayed
@@ -75,19 +64,17 @@
             y_units += ['states/eV'] * 2
         else:
             y_arrays += [array_data['dos']]
             y_names += ['dos']
             y_units += ['states/eV']
         xy_data.set_y(y_arrays, y_names, y_units)
 
-        parsed_data, logs = parse_output_base(out_file, 'DOS')
-        self.emit_logs(logs)
-
         self.out('output_dos', xy_data)
-        self.out('output_parameters', Dict(parsed_data))
+
+        return self.exit(logs=logs)
 
 
 def parse_raw_dos(dos_file, array_names, array_units):
     """This function takes as input the dos_file as a list of filelines along with information on how to give labels and
     units to the parsed data.
 
     :param dos_file: dos file lines in the form of a list
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/matdyn.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/matdyn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 # -*- coding: utf-8 -*-
 from aiida import orm
 from qe_tools import CONSTANTS
 
 from aiida_quantumespresso.calculations.matdyn import MatdynCalculation
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
-class MatdynParser(Parser):
-    """Parser implementation for the MatdynCalculation."""
+class MatdynParser(BaseParser):
+    """``Parser`` implementation for the ``MatDynCalculation`` calculation job class."""
 
     def parse(self, **kwargs):
-        """Parse the retrieved files from a `MatdynCalculation`."""
-        retrieved = self.retrieved
-        filename_stdout = self.node.get_option('output_filename')
-        filename_frequencies = MatdynCalculation._PHONON_FREQUENCIES_NAME
+        """Parse the retrieved files from a ``MatdynCalculation`` into output nodes."""
+        logs = get_logging_container()
+
+        _, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
+
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
 
-        if filename_stdout not in retrieved.base.repository.list_object_names():
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
+        self.out('output_parameters', orm.Dict(parsed_data))
 
-        if 'JOB DONE' not in retrieved.base.repository.get_object_content(filename_stdout):
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE)
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
 
-        if filename_frequencies not in retrieved.base.repository.list_object_names():
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
+        filename_frequencies = MatdynCalculation._PHONON_FREQUENCIES_NAME
 
         # Extract the kpoints from the input data and create the `KpointsData` for the `BandsData`
         try:
             kpoints = self.node.inputs.kpoints.get_kpoints()
             kpoints_for_bands = self.node.inputs.kpoints.clone()
         except AttributeError:
             kpoints = self.node.inputs.kpoints.get_kpoints_mesh(print_list=True)
             kpoints_for_bands = orm.KpointsData()
             kpoints_for_bands.set_kpoints(kpoints)
 
-        parsed_data = parse_raw_matdyn_phonon_file(retrieved.base.repository.get_object_content(filename_frequencies))
+        parsed_data = parse_raw_matdyn_phonon_file(self.retrieved.base.repository.get_object_content(filename_frequencies))
 
         try:
             num_kpoints = parsed_data.pop('num_kpoints')
         except KeyError:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_KPOINTS_MISSING)
+            return self.exit(self.exit_codes.ERROR_OUTPUT_KPOINTS_MISSING, logs)
 
         if num_kpoints != kpoints.shape[0]:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_KPOINTS_INCOMMENSURATE)
+            return self.exit(self.exit_codes.ERROR_OUTPUT_KPOINTS_INCOMMENSURATE, logs)
 
         output_bands = orm.BandsData()
         output_bands.set_kpointsdata(kpoints_for_bands)
         output_bands.set_bands(parsed_data.pop('phonon_bands'), units='THz')
 
         for message in parsed_data['warnings']:
             self.logger.error(message)
 
-        self.out('output_parameters', orm.Dict(parsed_data))
         self.out('output_phonon_bands', output_bands)
 
-        return
+        return self.exit(logs=logs)
 
 
 def parse_raw_matdyn_phonon_file(phonon_frequencies):
     """Parses the phonon frequencies file.
 
     :param phonon_frequencies: phonon frequencies file from the matdyn calculation
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/neb.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/neb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,127 +1,110 @@
 # -*- coding: utf-8 -*-
-from aiida.common import NotExistent
-from aiida.orm import Dict
+import os
+
+from aiida.common import AttributeDict, NotExistent
+from aiida.orm import ArrayData, Dict, TrajectoryData
+import numpy
 
 from aiida_quantumespresso.calculations.pw import PwCalculation
-from aiida_quantumespresso.parsers import QEOutputParsingError
 from aiida_quantumespresso.parsers.parse_raw import convert_qe_to_aiida_structure
 from aiida_quantumespresso.parsers.parse_raw.neb import parse_raw_output_neb
 from aiida_quantumespresso.parsers.parse_raw.pw import parse_stdout as parse_pw_stdout
 from aiida_quantumespresso.parsers.parse_raw.pw import reduce_symmetries
 from aiida_quantumespresso.parsers.parse_xml.exceptions import XMLParseError, XMLUnsupportedFormatError
 from aiida_quantumespresso.parsers.parse_xml.pw.parse import parse_xml as parse_pw_xml
 from aiida_quantumespresso.parsers.pw import PwParser
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
-class NebParser(Parser):
+class NebParser(BaseParser):
     """`Parser` implementation for the `NebCalculation` calculation job class."""
 
+    # Key that contains the optional parser options in the `settings` input node.
+    parser_settings_key = 'parser_options'
+
+    class_warning_map = {
+        'scf convergence NOT achieved on image': 'SCF did not converge for a given image',
+        'Maximum CPU time exceeded': 'Maximum CPU time exceeded',
+        'reached the maximum number of steps': 'Maximum number of iterations reached in the image optimization',
+    }
+
     def parse(self, **kwargs):
-        """Parse the retrieved files of a completed `NebCalculation` into output nodes.
+        """Parse the retrieved files of a completed ``NebCalculation`` into output nodes.
 
-        Two nodes that are expected are the default 'retrieved' `FolderData` node which will store the retrieved files
+        Two nodes that are expected are the default 'retrieved' ``FolderData`` node which will store the retrieved files
         permanently in the repository. The second required node is a filepath under the key `retrieved_temporary_files`
         which should contain the temporary retrieved files.
         """
-        import os
-
-        from aiida.orm import ArrayData, TrajectoryData
-        import numpy
-
-        PREFIX = self.node.process_class._PREFIX
-
-        retrieved = self.retrieved
-        list_of_files = retrieved.base.repository.list_object_names()  # Note: this includes folders, but not the files they contain.
+        logs = get_logging_container()
 
-        # The stdout is required for parsing
-        filename_stdout = self.node.base.attributes.get('output_filename')
-
-        if filename_stdout not in list_of_files:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
+        prefix = self.node.process_class._PREFIX
 
         # Look for optional settings input node and potential 'parser_options' dictionary within it
         # Note that we look for both NEB and PW parser options under "inputs.settings.parser_options";
         # we don't even have a namespace "inputs.pw.settings".
         try:
             settings = self.node.inputs.settings.get_dict()
-            parser_options = settings[self.get_parser_settings_key()]
+            parser_options = settings[self.parser_settings_key]
         except (AttributeError, KeyError, NotExistent):
             settings = {}
             parser_options = {}
 
         # load the pw input parameters dictionary
         pw_input_dict = self.node.inputs.pw.parameters.get_dict()
 
-        # load the neb input parameters dictionary
-        neb_input_dict = self.node.inputs.parameters.get_dict()
+        stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
 
-        # First parse the Neb output
-        try:
-            stdout = retrieved.base.repository.get_object_content(filename_stdout)
-            neb_out_dict, iteration_data, raw_successful = parse_raw_output_neb(stdout, neb_input_dict)
-            # TODO: why do we ignore raw_successful ?
-        except (OSError, QEOutputParsingError):
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
-
-        for warn_type in ['warnings', 'parser_warnings']:
-            for message in neb_out_dict[warn_type]:
-                self.logger.warning(f'parsing NEB output: {message}')
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
 
-        if 'QE neb run did not reach the end of the execution.' in neb_out_dict['parser_warnings']:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE)
+        neb_out_dict, iteration_data = parse_raw_output_neb(stdout)
+        parsed_data.update(neb_out_dict)
 
-        # Retrieve the number of images
-        try:
-            num_images = neb_input_dict['num_of_images']
-        except KeyError:
-            try:
-                num_images = neb_out_dict['num_of_images']
-            except KeyError:
-                return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_PARSE)
-        if num_images < 2:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_PARSE)
+        num_images = parsed_data['num_of_images']
 
         # Now parse the information from the individual pw calculations for the different images
         image_data = {}
         positions = []
         cells = []
-        # for each image...
+
         for i in range(num_images):
             # check if any of the known XML output file names are present, and parse the first that we find
-            relative_output_folder = os.path.join(f'{PREFIX}_{i + 1}', f'{PREFIX}.save')
+            relative_output_folder = os.path.join(f'{prefix}_{i + 1}', f'{prefix}.save')
             retrieved_files = self.retrieved.base.repository.list_object_names(relative_output_folder)
+
             for xml_filename in PwCalculation.xml_filenames:
                 if xml_filename in retrieved_files:
                     xml_file_path = os.path.join(relative_output_folder, xml_filename)
                     try:
-                        with retrieved.base.repository.open(xml_file_path) as xml_file:
+                        with self.retrieved.base.repository.open(xml_file_path) as xml_file:
                             parsed_data_xml, logs_xml = parse_pw_xml(xml_file, None)
                     except IOError:
                         return self.exit(self.exit_codes.ERROR_OUTPUT_XML_READ)
                     except XMLParseError:
                         return self.exit(self.exit_codes.ERROR_OUTPUT_XML_PARSE)
                     except XMLUnsupportedFormatError:
                         return self.exit(self.exit_codes.ERROR_OUTPUT_XML_FORMAT)
-                    except Exception as exc:
+                    except Exception:
                         import traceback
                         traceback.print_exc()
-                        return self.exit(self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION.format(exception=exc))
+                        return self.exit(self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION)
                     # this image is dealt with, so break the inner loop and go to the next image
                     break
             # otherwise, if none of the filenames we tried exists, exit with an error
             else:
                 return self.exit(self.exit_codes.ERROR_MISSING_XML_FILE)
 
             # look for pw output and parse it
-            pw_out_file = os.path.join(f'{PREFIX}_{i + 1}', 'PW.out')
+            pw_out_file = os.path.join(f'{prefix}_{i + 1}', 'PW.out')
             try:
-                with retrieved.base.repository.open(pw_out_file, 'r') as f:
+                with self.retrieved.base.repository.open(pw_out_file, 'r') as f:
                     pw_out_text = f.read()  # Note: read() and not readlines()
             except IOError:
                 return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
 
             try:
                 parsed_data_stdout, logs_stdout = parse_pw_stdout(
                     pw_out_text, pw_input_dict, parser_options, parsed_data_xml
@@ -154,24 +137,24 @@
             key = f'pw_output_image_{i + 1}'
             image_data[key] = parsed_parameters
 
             positions.append([site.position for site in structure_data.sites])
             cells.append(structure_data.cell)
 
             # Add also PW warnings and errors to the neb output data, avoiding repetitions.
-            for log_type in ['warning', 'error']:
-                for message in logs_stdout[log_type]:
-                    formatted_message = f'{log_type}: {message}'
-                    if formatted_message not in neb_out_dict['warnings']:
-                        neb_out_dict['warnings'].append(formatted_message)
+            for log_level in ['warning', 'error']:
+                for message in logs_stdout[log_level]:
+                    formatted_message = f'{log_level}: {message}'
+                    if formatted_message not in parsed_data['warnings']:
+                        parsed_data['warnings'].append(formatted_message)
 
         # Symbols can be obtained simply from the last image
         symbols = [str(site.kind_name) for site in structure_data.sites]
 
-        output_params = Dict(dict(list(neb_out_dict.items()) + list(image_data.items())))
+        output_params = Dict(dict(list(parsed_data.items()) + list(image_data.items())))
         self.out('output_parameters', output_params)
 
         trajectory = TrajectoryData()
         trajectory.set_trajectory(
             stepids=numpy.arange(1, num_images + 1),
             cells=numpy.array(cells),
             symbols=symbols,
@@ -184,34 +167,32 @@
                 arraydata = ArrayData()
                 for k, v in iteration_data.items():
                     arraydata.set_array(k, numpy.array(v))
                 self.out('iteration_array', arraydata)
 
         # Load the original and interpolated energy profile along the minimum-energy path (mep)
         try:
-            filename = PREFIX + '.dat'
-            with retrieved.base.repository.open(filename, 'r') as handle:
+            filename = prefix + '.dat'
+            with self.retrieved.base.repository.open(filename, 'r') as handle:
                 mep = numpy.loadtxt(handle)
         except Exception:
             self.logger.warning(f'could not open expected output file `{filename}`.')
             mep = numpy.array([[]])
 
         try:
-            filename = PREFIX + '.int'
-            with retrieved.base.repository.open(filename, 'r') as handle:
+            filename = prefix + '.int'
+            with self.retrieved.base.repository.open(filename, 'r') as handle:
                 interp_mep = numpy.loadtxt(handle)
         except Exception:
             self.logger.warning(f'could not open expected output file `{filename}`.')
             interp_mep = numpy.array([[]])
 
         # Create an ArrayData with the energy profiles
         mep_arraydata = ArrayData()
         mep_arraydata.set_array('mep', mep)
         mep_arraydata.set_array('interpolated_mep', interp_mep)
         self.out('output_mep', mep_arraydata)
 
-        return
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
 
-    @staticmethod
-    def get_parser_settings_key():
-        """Return the key that contains the optional parser options in the `settings` input node."""
-        return 'parser_options'
+        return self.exit(logs=logs)
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/open_grid.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/open_grid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # -*- coding: utf-8 -*-
-from aiida.common import NotExistent
+from typing import Tuple
+
+from aiida.common import AttributeDict
 from aiida.orm import Dict, KpointsData
 
-from aiida_quantumespresso.parsers.base import Parser
-from aiida_quantumespresso.parsers.parse_raw.base import parse_output_base
+from aiida_quantumespresso.parsers.base import BaseParser
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
 
-class OpenGridParser(Parser):
+class OpenGridParser(BaseParser):
     """``Parser`` implementation for the ``OpenGridCalculation`` calculation job class."""
 
+    class_error_map = {
+        'incompatible FFT grid': 'ERROR_INCOMPATIBLE_FFT_GRID'
+    }
+
     def parse(self, **kwargs):
         """Parse the retrieved files of a completed ``OpenGridCalculation`` into output nodes."""
-        try:
-            out_folder = self.retrieved
-        except NotExistent:
-            return self.exit(self.exit_codes.ERROR_NO_RETRIEVED_FOLDER)
-
-        try:
-            filename_stdout = self.node.get_option('output_filename')
-            with out_folder.open(filename_stdout, 'r') as handle:
-                out_file = handle.read()
-        except OSError:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
+        logs = get_logging_container()
+
+        stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
+
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
 
-        parsed_data, logs = parse_output_base(out_file, codename='OPEN_GRID')
-        self.emit_logs(logs)
         self.out('output_parameters', Dict(parsed_data))
 
-        lines = out_file.split('\n')
-        for line in lines:
-            if 'incompatible FFT grid' in line:
-                return self.exit(self.exit_codes.ERROR_INCOMPATIBLE_FFT_GRID)
+        for exit_code in self.get_error_map().values():
+            if exit_code in logs.error:
+                return self.exit(self.exit_codes.get(exit_code), logs)
 
-        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE' in logs.error:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE)
-        elif logs.error:
-            return self.exit(self.exit_codes.ERROR_GENERIC_QE_ERROR)
-
-        try:
-            kpoints_mesh, kpoints = self.parse_kpoints(out_file)
-        except ValueError:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_KPOINTS_MISMATCH)
+        kpoints_mesh, kpoints, logs = self.parse_kpoints(stdout, logs)
 
-        # Output both the dimensions and the explict list of kpoints
         self.out('kpoints_mesh', kpoints_mesh)
         self.out('kpoints', kpoints)
 
+        for exit_code in ['ERROR_OUTPUT_KPOINTS_MISMATCH', 'ERROR_OUTPUT_STDOUT_INCOMPLETE']:
+            if exit_code in logs.error:
+                return self.exit(self.exit_codes.get(exit_code), logs)
+
+        return self.exit(logs=logs)
+
     @staticmethod
-    def parse_kpoints(out_file):
-        """Parse and output the dimensions and the explicit list of kpoints."""
-        lines = out_file.split('\n')
+    def parse_kpoints(stdout: str, logs: AttributeDict) -> Tuple[KpointsData, KpointsData, AttributeDict]:
+        """Parse the ``stdout`` for the mesh and explicit list of kpoints."""
+        lines = stdout.split('\n')
 
         kpoints = []
         weights = []
         found_kpoints = False
 
         for line in lines:
             if 'EXX: q-point mesh:' in line:
@@ -72,10 +68,10 @@
 
         kpoints_mesh = KpointsData()
         kpoints_mesh.set_kpoints_mesh(kmesh)
         kpoints_list = KpointsData()
         kpoints_list.set_kpoints(kpoints, cartesian=False, weights=weights)
 
         if kmesh[0] * kmesh[1] * kmesh[2] != len(kpoints):
-            raise ValueError('Mismatch between kmesh dimensions and number of kpoints')
+            logs.error.append('ERROR_OUTPUT_KPOINTS_MISMATCH')
 
-        return kpoints_mesh, kpoints_list
+        return kpoints_mesh, kpoints_list, logs
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,15 @@
         if 'conjugate gradient' in line.lower():
             conjugate_gradient = True
             parsed_data['conjugate_gradient'] = True
         if 'warning' in line.lower():
             parsed_data['warnings'].append(line)
         elif 'bananas' in line:
             parsed_data['warnings'].append('Bananas from the ortho.')
-        elif 'CP' in line and 'WALL' in line:
-            try:
-                time = line.split('CPU')[1].split('WALL')[0]
-                parsed_data['wall_time'] = time
-            except:
-                raise QEOutputParsingError('Error while parsing wall time.')
+
     #when the cp does a cg, the output is different and the parser below does not work
     #TODO: understand what the cg prints out and parse it (it is undocumented)
     if not conjugate_gradient:
         for count, line in enumerate(reversed(data)):
             if 'nfi' in line and 'ekinc' in line and 'econs' in line:
                 this_line = data[len(data) - count]
                 try:
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/xspectra.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,236 +1,237 @@
 # -*- coding: utf-8 -*-
-"""A collection of function that are used to parse the output of Quantum Espresso Neb.
+import re
+from typing import Tuple
 
-The function that needs to be called from outside is parse_raw_output_neb(). The functions mostly work without aiida
-specific functionalities. The parsing will try to convert whatever it can in some dictionary, which by operative
-decision doesn't have much structure encoded, [the values are simple ]
-"""
-from qe_tools import CONSTANTS
+from aiida.common import AttributeDict
+from aiida.orm import Dict, XyData
+import numpy as np
 
 from aiida_quantumespresso.parsers import QEOutputParsingError
-from aiida_quantumespresso.parsers.parse_raw import convert_qe_time_to_sec
+from aiida_quantumespresso.parsers.base import BaseParser
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
 
-def parse_raw_output_neb(stdout, input_dict, parser_opts=None):
-    """Parses the output of a neb calculation Receives in input the paths to the output file.
+class XspectraParser(BaseParser):
+    """Parser for the ``XSpectraCalculation`` calcjob plugin."""
 
-    :param stdout: the stdout content as a string
-    :param input_dict: dictionary with the neb input parameters
-    :param parser_opts: not used
-
-    :return parameter_data: a dictionary with parsed parameters
-    :return iteration_data: a dictionary with arrays (for relax & md calcs.)
-    :return job_successful: a boolean that is False in case of failed calculations
-
-    :raises QEOutputParsingError: for errors in the parsing,
-
-    2 different keys to check in output: parser_warnings and warnings.
-    On an upper level, these flags MUST be checked.
-    The first is expected to be empty unless QE failures or unfinished jobs.
-    """
-    import copy
-
-    job_successful = True
-    parser_warnings = []
-
-    if not stdout:  # there is an output file, but it's empty -> crash
-        job_successful = False
-
-    # check if the job has finished (that doesn't mean without errors)
-    finished_run = False
-    for line in stdout.split('\n')[::-1]:
-        if 'JOB DONE' in line:
-            finished_run = True
-            break
-    if not finished_run:  # error if the job has not finished
-        warning = 'QE neb run did not reach the end of the execution.'
-        parser_warnings.append(warning)
-        job_successful = False
-
-    # parse the text output of the neb calculation
-    try:
-        out_data, iteration_data, critical_messages = parse_neb_text_output(stdout, input_dict)
-    except QEOutputParsingError as exc:
-        if not finished_run:  # I try to parse it as much as possible
-            parser_warnings.append('Error while parsing the output file')
-            out_data = {'warnings': []}
-            iteration_data = {}
-            critical_messages = []
-        else:  # if it was finished and I got an error, it's a mistake of the parser
-            raise QEOutputParsingError(f'Error while parsing NEB text output: {exc}')
-
-    # I add in the out_data all the last elements of iteration_data values.
-    # I leave the possibility to skip some large arrays (None for the time being).
-    skip_keys = []
-    tmp_iteration_data = copy.copy(iteration_data)
-    for k, v in tmp_iteration_data.items():
-        if k in skip_keys:
-            continue
-        out_data[k] = v[-1]
-
-    # if there is a severe error, the calculation is FAILED
-    if any([x in out_data['warnings'] for x in critical_messages]):
-        job_successful = False
-
-    parameter_data = dict(list(out_data.items()) + [('parser_warnings', parser_warnings)])
-
-    # return various data.
-    # parameter data will be mapped in Dict
-    # iteration_data in ArrayData
-    return parameter_data, iteration_data, job_successful
-
-
-def parse_neb_text_output(data, input_dict={}):
-    """Parses the text output of QE Neb.
-
-    :param data: a string, the file as read by read()
-    :param input_dict: dictionary with the input parameters
-
-    :return parsed_data: dictionary with key values, referring to quantities
-                         at the last step.
-    :return iteration_data: key,values referring to intermediate iterations.
-                             Empty dictionary if no value is present.
-    :return critical_messages: a list with critical messages. If any is found in
-                               parsed_data['warnings'], the calculation is FAILED!
-    """
-    from collections import defaultdict
-
-    from aiida_quantumespresso.parsers.parse_raw import parse_output_error
-    from aiida_quantumespresso.utils.mapping import get_logging_container
-
-    # TODO: find a more exhaustive list of the common errors of neb
-    # critical warnings: if any is found, the calculation status is FAILED
-    critical_warnings = {
-        'scf convergence NOT achieved on image': 'SCF did not converge for a given image',
-        'Maximum CPU time exceeded': 'Maximum CPU time exceeded',
-        'reached the maximum number of steps': 'Maximum number of iterations reached in the image optimization',
+    class_error_map = {
+        'Wrong xiabs!!!': 'ERROR_OUTPUT_ABSORBING_SPECIES_WRONG',
+        'xiabs < 1 or xiabs > ntyp': 'ERROR_OUTPUT_ABSORBING_SPECIES_ZERO',
+        'Calculation not finished': 'ERROR_OUT_OF_WALLTIME',
     }
+    success_string='END JOB'
 
-    minor_warnings = {
-        'Warning:': None,
-    }
+    def parse(self, **kwargs):
+        """Parse the contents of the output files stored in the `retrieved` output node."""
+        logs = get_logging_container()
+
+        stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
+
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
+
+        parsed_xspectra, logs = self.parse_stdout(stdout, logs)
+        parsed_data.update(parsed_xspectra)
+
+        # Parse some additional info which the stdout does not reliably report
+        parameters = self.node.inputs.parameters.base.attributes.get('INPUT_XSPECTRA', {})
 
-    all_warnings = dict(list(critical_warnings.items()) + list(minor_warnings.items()))
+        xepsilon_defaults = {
+            '1': 0,
+            '2': 0,
+            '3': 1,
+        }
+        raw_xepsilon = [parameters.get(f'xepsilon({n})', xepsilon_defaults[n]) for n in ['1', '2', '3']]
+        parsed_data['xepsilon'] = [float(n) for n in raw_xepsilon]
+        parsed_data['xcoordcrys'] = parameters.get('xcoordcrys', True)
+        parsed_data['xonly_plot'] = parameters.get('xonly_plot', False)
 
-    parsed_data = {}
-    parsed_data['warnings'] = []
-    iteration_data = defaultdict(list)
-
-    # parse time, starting from the end
-    # apparently, the time is written multiple times
-    for line in reversed(data.split('\n')):
-        if 'NEB' in line and 'WALL' in line:
-            try:
-                time = line.split('CPU')[1].split('WALL')[0].strip()
-                parsed_data['wall_time'] = time
-            except Exception:
-                parsed_data['warnings'].append('Error while parsing wall time.')
-
-            try:
-                parsed_data['wall_time_seconds'] = \
-                    convert_qe_time_to_sec(parsed_data['wall_time'])
-            except ValueError:
-                raise QEOutputParsingError('Unable to convert wall_time in seconds.')
-            break
-
-    # set by default the calculation as not converged.
-    parsed_data['converged'] = [False, 0]
-    logs = get_logging_container()
-    lines = data.split('\n')
-
-    for count, line in enumerate(lines):
-        if 'initial path length' in line:
-            initial_path_length = float(line.split('=')[1].split('bohr')[0])
-            parsed_data['initial_path_length'] = initial_path_length * CONSTANTS.bohr_to_ang
-        elif 'initial inter-image distance' in line:
-            initial_image_dist = float(line.split('=')[1].split('bohr')[0])
-            parsed_data['initial_image_dist'] = initial_image_dist * CONSTANTS.bohr_to_ang
-        elif 'string_method' in line:
-            parsed_data['string_method'] = line.split('=')[1].strip()
-        elif 'restart_mode' in line:
-            parsed_data['restart_mode'] = line.split('=')[1].strip()
-        elif 'opt_scheme' in line:
-            parsed_data['opt_scheme'] = line.split('=')[1].strip()
-        elif 'num_of_images' in line:
-            parsed_data['num_of_images'] = int(line.split('=')[1])
-        elif 'nstep_path' in line:
-            parsed_data['nstep_path'] = int(line.split('=')[1])
-        elif 'CI_scheme' in line:
-            parsed_data['ci_scheme'] = line.split('=')[1].strip()
-        elif 'first_last_opt' in line:
-            parsed_data['first_last_opt'] = True if line.split('=')[1] == 'T' else False
-        elif 'use_freezing' in line:
-            parsed_data['use_freezing'] = True if line.split('=')[1] == 'T' else False
-        elif ' ds ' in line:
-            parsed_data['ds_au'] = float(line.split('=')[1].split('a.u.')[0])
-        elif '   k_max' in line:
-            parsed_data['k_max'] = float(line.split('=')[1].split('a.u.')[0])
-        elif '   k_min_au' in line:
-            parsed_data['k_min_au'] = float(line.split('=')[1].split('a.u.')[0])
-        elif 'suggested k_max' in line:
-            parsed_data['suggested_k_max_au'] = float(line.split('=')[1].split('a.u.')[0])
-        elif 'suggested k_min' in line:
-            parsed_data['suggested_k_min_au'] = float(line.split('=')[1].split('a.u.')[0])
-        elif 'path_thr' in line:
-            parsed_data['path_thr'] = float(line.split('=')[1].split('eV')[0])
-        elif 'list of climbing images' in line:
-            parsed_data['climbing_images_manual'] = [int(_) for _ in line.split(':')[1].split(',')[:-1]]
-        elif 'neb: convergence achieved in' in line:
-            parsed_data['converged'] = [True, int(line.split('iteration')[0].split()[-1])]
-        elif '%%%%%%%%%%%%%%' in line:
-            parse_output_error(lines, count, logs)
-        elif any(i in line for i in all_warnings):
-            message = [all_warnings[i] for i in all_warnings.keys() if i in line][0]
-
-            if message is not None:
-                parsed_data['warnings'].append(message)
-
-    parsed_data['warnings'].extend(logs.error)
-
-    try:
-        num_images = parsed_data['num_of_images']
-    except KeyError:
+        self.out('output_parameters', Dict(parsed_data))
+
+        for exit_code in list(self.class_error_map.values()) + ['ERROR_OUTPUT_STDOUT_INCOMPLETE']:
+            if exit_code in logs.error:
+                return self.exit(self.exit_codes.get(exit_code), logs)
+
+        # Check that the spectra data file exists and is readable
         try:
-            num_images = input_dict['PATH']['num_of_images']
-        except KeyError:
-            raise QEOutputParsingError(
-                'No information on the number '
-                'of images available (neither in input nor in output'
-            )
-
-    iteration_lines = data.split('-- iteration')[1:]
-    iteration_lines = [i.split('\n') for i in iteration_lines]
-
-    for iteration in iteration_lines:
-        for count, line in enumerate(iteration):
-            if 'activation energy (->)' in line:
-                activ_energy = float(line.split('=')[1].split('eV')[0])
-                iteration_data['forward_activation_energy'].append(activ_energy)
-            elif 'activation energy (<-)' in line:
-                activ_energy = float(line.split('=')[1].split('eV')[0])
-                iteration_data['backward_activation_energy'].append(activ_energy)
-            elif 'image        energy (eV)        error (eV/A)        frozen' in line:
-                energies = []
-                forces = []
-                frozen = []
+            with self.retrieved.base.repository.open(self.node.process_class._Spectrum_FILENAME, 'r') as fil:
+                xspectra_file = fil.readlines()
+        except OSError:
+            return self.exit(self.exit_codes.ERROR_READING_SPECTRUM_FILE, logs)
+
+        # Check that the data in the spectra file can be read by NumPy
+        try:
+            _ = np.genfromtxt(xspectra_file)
+        except ValueError:
+            return self.exit(self.exit_codes.ERROR_READING_SPECTRUM_FILE_DATA, logs)
+
+        array_names = [[], []]
+        array_units = [[], []]
+
+        array_names[0] = ['energy', 'sigma'] # for non-spin-polarised calculations
+        array_units[0] = ['eV', 'n/a']
+
+        array_names[1] = ['energy', 'sigma_tot', 'sigma_up', 'sigma_down'] # for spin-polarised calculations
+        array_units[1] = ['eV', 'n/a', 'n/a', 'n/a']
+
+        array_data, spin = self.parse_raw_xspectra(xspectra_file, array_names, array_units)
+
+        energy_units = 'eV'
+        xy_data = XyData()
+        xy_data.set_x(array_data['energy'], 'energy', energy_units)
+
+        y_arrays = []
+        y_names = []
+        y_units = []
+        if spin:
+            y_arrays += [array_data['sigma_tot']]
+            y_names += ['sigma_tot']
+            y_arrays += [array_data['sigma_up']]
+            y_arrays += [array_data['sigma_down']]
+            y_names += ['sigma_up']
+            y_names += ['sigma_down']
+            y_units += ['n/a'] * 3
+        else:
+            y_arrays += [array_data['sigma']]
+            y_names += ['sigma']
+            y_units += ['n/a']
+
+        xy_data.set_y(y_arrays, y_names, y_units)
+
+        self.out('spectra', xy_data)
+
+        return self.exit(logs=logs)
+
+    @staticmethod
+    def parse_stdout(stdout: str, logs: AttributeDict) -> Tuple[dict, AttributeDict]:
+        """Parse the ``stdout`` of XSpectra for the core level energy and energy zero of the spectrum."""
+        from .parse_raw.base import convert_qe_time_to_sec
+
+        parsed_data = {}
+
+        # Parse the necessary information for data plotting: core level energy of the
+        # absorbing atom and the energy zero of the spectrum (typically the Fermi level)
+        for line in stdout.split('\n'):
+            if 'From SCF save directory' in line:
+                if '(spin polarized work)' in line:
+                    spin = True
+                else:
+                    spin = False
+                parsed_data['lsda'] = spin
+            if 'ehomo [eV]' in line:
+                if spin:
+                    homo_energy = line.split(':')[-2].split('(')[0].strip()
+                else:
+                    homo_energy = line.split(':')[-1].split('(')[0].strip()
+                homo_energy_units = line.split('[')[1].split(':')[0].replace(']', '')
+                parsed_data['highest_occupied_level'] = homo_energy
+                parsed_data['highest_occupied_level_units'] = homo_energy_units
+            if 'elumo [eV]' in line:
+                if spin:
+                    lumo_energy = line.split(':')[-2].split('(')[0].strip()
+                else:
+                    lumo_energy = line.split(':')[-1].split('(')[0].strip()
+                lumo_energy_units = line.split('[')[1].split(':')[0].replace(']', '')
+                parsed_data['lowest_unoccupied_level'] = lumo_energy
+                parsed_data['lowest_unoccupied_level_units'] = lumo_energy_units
+                parsed_data['lumo_found'] = True
+            elif 'No LUMO value' in line:
+                parsed_data['lumo_found'] = False
+            if 'ef    [eV]' in line:
+                ef_energy = line.split(':')[-1].split('(')[0].strip()
+                ef_energy_units = line.split('[')[1].split(':')[0].replace(']', '')
+                parsed_data['fermi_energy'] = ef_energy
+                parsed_data['fermi_energy_units'] = ef_energy_units
+
+            # parse per-process dynamical RAM estimates
+            if 'Estimated max dynamical RAM per process' in line:
+                value = line.split('>')[-1]
+                match = re.match(r'\s+([+-]?\d+(\.\d*)?|\.\d+([eE][+-]?\d+)?)\s*(Mb|MB|GB)', value)
+                if match:
+                    try:
+                        parsed_data['estimated_ram_per_process'] = float(match.group(1))
+                        parsed_data['estimated_ram_per_process_units'] = match.group(4)
+                    except (IndexError, ValueError):
+                        pass
+
+            # parse total dynamical RAM estimates
+            if 'Estimated total dynamical RAM' in line:
+                value = line.split('>')[-1]
+                match = re.match(r'\s+([+-]?\d+(\.\d*)?|\.\d+([eE][+-]?\d+)?)\s*(Mb|MB|GB)', value)
+                if match:
+                    try:
+                        parsed_data['estimated_ram_total'] = float(match.group(1))
+                        parsed_data['estimated_ram_total_units'] = match.group(4)
+                    except (IndexError, ValueError):
+                        pass
+
+            if 'Core level energy' in line:
+                core_energy_line = line
+                parsed_data['core_level_energy'] = core_energy_line.split('[')[1].split(':')[1].strip()
+                parsed_data['core_level_energy_units'] = core_energy_line.split('[')[1].split(':')[0].replace(']', '')
+            if 'energy-zero' in line:
+                energy_zero_line = line
+                parsed_data['energy_zero'] = energy_zero_line.split('[')[1].split(':')[1].strip()
+                parsed_data['energy_zero_units'] = energy_zero_line.split('[')[1].split(':')[0].replace(']', '')
+
+            # Parse the walltime
+            # XSpectra does not appear next to the timing data, so we must find 'xanes' instead.
+            if 'xanes' in line and 'WALL' in line:
+                try:
+                    time = line.split('CPU')[1].split('WALL')[0].strip()
+                    parsed_data['wall_time'] = time
+                except (ValueError, IndexError):
+                    break
                 try:
-                    for i in range(num_images):
-                        split_line = iteration[count + 2 + i].split()[1:]
-                        energies.append(float(split_line[0]))
-                        forces.append(float(split_line[1]))
-                        frozen.append(True if split_line[2] == 'T' else False)
-                    iteration_data['image_energies'].append(energies)
-                    iteration_data['image_forces'].append(forces)
-                    iteration_data['image_frozen'].append(frozen)
-                except Exception:
-                    parsed_data['warnings'].append('Error while parsing the image energies and forces.')
-            elif 'climbing image' in line:
-                iteration_data['climbing_image_auto'].append([int(_) for _ in line.split('=')[1].split(',')])
-            elif 'path length' in line:
-                path_length = float(line.split('=')[1].split('bohr')[0])
-                iteration_data['path_length'].append(path_length * CONSTANTS.bohr_to_ang)
-            elif 'inter-image distance' in line:
-                image_dist = float(line.split('=')[1].split('bohr')[0])
-                iteration_data['image_dist'].append(image_dist * CONSTANTS.bohr_to_ang)
+                    parsed_data['wall_time_seconds'] = convert_qe_time_to_sec(time)
+                except ValueError:
+                    logs.warnings.append('Unable to convert wall time from `stdout` to seconds.')
+
+        return parsed_data, logs
+
+    @staticmethod
+    def parse_raw_xspectra(xspectra_file, array_names, array_units):
+        """Parse the content of the output spectrum.
+
+        This function takes as input the xspectra_file as a list of filelines along with information on how to give
+        labels and units to the parsed data.
+
+        :param xspectra_file: xspectra file lines in the form of a list
+        :type xspectra_file: list
+        :param array_names: list of all array names.
+        :type array_names: list
+        :param array_units: list of all array units.
+        :type array_units: list
+
+        :return array_data: narray, a dictionary for ArrayData type, which
+            contains all parsed xspectra output along with labels and units
+        """
+        xspectra_header = xspectra_file[:4]
+        xspectra_data = np.genfromtxt(xspectra_file)
+
+        if len(xspectra_data) == 0:
+            raise QEOutputParsingError('XSpectra file is empty.')
+        if np.isnan(xspectra_data).any():
+            raise QEOutputParsingError('XSpectra file contains non-numeric elements.')
+
+        if len(xspectra_data[0]) == 2:
+            array_names = array_names[0]
+            array_units = array_units[0]
+            spin = False
+        elif len(xspectra_data[0]) == 4:
+            array_names = array_names[1]
+            array_units = array_units[1]
+            spin = True
+        else:
+            raise QEOutputParsingError('XSpectra data file in unsuitable format for the parser')
+
+        i = 0
+        array_data = {}
+        array_data['header'] = np.array(xspectra_header)
+        while i < len(array_names):
+            array_data[array_names[i]] = xspectra_data[:, i]
+            array_data[array_names[i] + '_units'] = np.array(array_units[i])
+            i += 1
 
-    return parsed_data, dict(iteration_data), list(critical_warnings.values())
+        return array_data, spin
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,35 +6,26 @@
 """
 import numpy
 from qe_tools import CONSTANTS
 
 from aiida_quantumespresso.parsers import QEOutputParsingError
 from aiida_quantumespresso.parsers.parse_raw.base import convert_qe_time_to_sec
 from aiida_quantumespresso.parsers.parse_xml.pw.legacy import parse_xml_child_bool, read_xml_card
-from aiida_quantumespresso.utils.mapping import get_logging_container
 
 
-def parse_raw_ph_output(stdout, tensors=None, dynamical_matrices=None):
+def parse_raw_ph_output(stdout, logs, tensors=None, dynamical_matrices=None):
     """Parses the raw output of a Quantum ESPRESSO `ph.x` calculation.
 
     :param stdout: the content of the stdout file as a string
     :param tensors: the content of the tensors.xml file as a string
     :param dynamical_matrices: a list of the content of the dynamical matrix files as a string
     :returns: tuple of two dictionaries, with the parsed data and log messages, respectively
     """
-    logs = get_logging_container()
     data_lines = stdout.split('\n')
 
-    # First check whether the `JOB DONE` message was written, otherwise the job was interrupted
-    for line in data_lines:
-        if 'JOB DONE' in line:
-            break
-    else:
-        logs.error.append('ERROR_OUTPUT_STDOUT_INCOMPLETE')
-
     # Parse tensors, if present
     tensor_data = {}
     if tensors:
         try:
             tensor_data = parse_ph_tensor(tensors)
         except QEOutputParsingError:
             logs.warning.append('Error while parsing the tensor files')
@@ -143,47 +134,20 @@
     # convert to float, then into a list of tuples, then into a list of lists
     flat_array = [float(i) for i in flat_array]
     list_tuple = list(zip(*[iter(flat_array)] * 3))
     return [list(i) for i in list_tuple]
 
 
 def parse_ph_text_output(lines, logs):
-    """Parses the stdout of Quantum ESPRESSO ph.x.
+    """Parses the stdout of Quantum ESPRESSO ``ph.x``.
 
     :param lines: list of strings, the file as read by readlines()
     :return: dictionary with parsed values
     """
 
-    def detect_important_message(logs, line):
-
-        message_map = {
-            'error': {
-                'Maximum CPU time exceeded': 'ERROR_OUT_OF_WALLTIME',
-                'No convergence has been achieved': 'ERROR_CONVERGENCE_NOT_REACHED',
-                'problems computing cholesky': 'ERROR_COMPUTING_CHOLESKY',
-            },
-            'warning': {
-                'Warning:': None,
-                'DEPRECATED:': None,
-            }
-        }
-
-        # Match any known error and warning messages
-        for marker, message in message_map['error'].items():
-            if marker in line:
-                if message is None:
-                    message = line
-                logs.error.append(message)
-
-        for marker, message in message_map['warning'].items():
-            if marker in line:
-                if message is None:
-                    message = line
-                logs.warning.append(message)
-
     def parse_qpoints(lines):
         """Parse the q-points from the corresponding lines in the stdout."""
 
         return {int(line.split()[0]): [float(coord) for coord in line.split()[1:4]] for line in lines}
 
     def parse_mode_symmetries(lines, num_atoms):
         """Parse the mode symmetries from the block after diagonalization of the dynamical matrix."""
@@ -214,30 +178,19 @@
             q_data['point_group'] = 'C_1'
             q_data['mode_symmetry'] = ['A'] * (3 * num_atoms)
 
         return symlabel_q_point, q_data
 
     parsed_data = {}
 
-    # Parse time, starting from the end because the time is written multiple times
-    for line in reversed(lines):
-        if 'PHONON' in line and 'WALL' in line:
-            try:
-                parsed_data['wall_time_seconds'] = \
-                    convert_qe_time_to_sec(line.split('CPU')[1].split('WALL')[0])
-            except (ValueError, IndexError):
-                raise QEOutputParsingError('Error during parsing of walltime.')
-            break
-
     parsed_data['num_q_found'] = 0
 
+    # Parse number of q-points and number of atoms
     for count, line in enumerate(lines):
 
-        detect_important_message(logs, line)
-
         if 'q-points for this run' in line:
             try:
                 parsed_data['number_of_qpoints'] = int(line.split('/')[1].split('q-points')[0])
                 parsed_data['q_points'] = parse_qpoints(lines[count + 2:count + parsed_data['number_of_qpoints'] + 2])
 
             except Exception as exc:
                 logs.warning.append(f'Error while parsing number of q points: {exc}')
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pp.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 # -*- coding: utf-8 -*-
 """`Parser` implementation for the `PpCalculation` calculation job class."""
 import os
 import re
-import traceback
+from typing import Tuple
 
 from aiida import orm
-from aiida.common import exceptions
+from aiida.common import AttributeDict
 import numpy as np
 
 from aiida_quantumespresso.calculations.pp import PpCalculation
 from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
-class PpParser(Parser):
-    """`Parser` implementation for the `PpCalculation` calculation job class."""
+class PpParser(BaseParser):
+    """``Parser`` implementation for the ``PpCalculation`` calculation job class."""
+
+    class_error_map = {
+        'xml data file not found': 'ERROR_PARENT_XML_MISSING',
+    }
 
     # Lookup: plot_num --> units
     units_dict = {
         0: 'e/bohr^3',  # Electrons, electronic charge density
         1: 'Ry',  # Total potential
         2: 'Ry',  # Ionic potential
         3: 'states/bohr^3',  # Density of states over an energy range
@@ -39,37 +43,40 @@
         20:
         'e/bohr^5',  # Product of the electron density and the second eigenvalue of the electron-density Hessian matrix, see: dx.doi.org/10.1021/ct100641a, with sign of second eigenvalue
         21: 'e/bohr^3',  # All electron charge density, PAW case
         22: 'Ry/bohr^3',  # Kinetic energy density
     }
 
     def parse(self, **kwargs):
-        """
-        Parse raw files retrieved from remote dir
-        """
-        retrieved = self.retrieved
+        """Parse the retrieved files of a ``PpCalculation`` into output nodes."""
+        logs = get_logging_container()
+
+        stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
+
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
+
+        parsed_pp, logs = self.parse_stdout(stdout, logs)
+        parsed_data.update(parsed_pp)
+
+        self.out('output_parameters', orm.Dict(parsed_data))
+
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
+
         retrieve_temporary_list = self.node.base.attributes.get('retrieve_temporary_list', None)
-        filename_stdout = self.node.get_option('output_filename')
 
         # If temporary files were specified, check that we have them
         if retrieve_temporary_list:
             try:
                 retrieved_temporary_folder = kwargs['retrieved_temporary_folder']
             except KeyError:
                 return self.exit(self.exit_codes.ERROR_NO_RETRIEVED_TEMPORARY_FOLDER)
 
-        # The stdout is required for parsing
-        if filename_stdout not in retrieved.base.repository.list_object_names():
-            return self.exit_codes.ERROR_OUTPUT_STDOUT_MISSING
-
-        try:
-            stdout_raw = retrieved.base.repository.get_object_content(filename_stdout)
-        except (IOError, OSError):
-            return self.exit_codes.ERROR_OUTPUT_STDOUT_READ
-
         # Currently all plot output files should start with the `filplot` as prefix. If only one file was produced the
         # prefix is the entire filename, but in the case of multiple files, there will be pairs of two files where the
         # first has the format '{filename_prefix}.{some_random_suffix' and the second has the same name but with the
         # `filename_suffix` appended.
         filename_prefix = PpCalculation._FILPLOT
         filename_suffix = PpCalculation._FILEOUT
 
@@ -79,30 +86,16 @@
         # that will open a handle to the output file given a certain filename. This works since it is guaranteed that
         # these output files (excluding the standard output) will all either be in the retrieved, or in the retrieved
         # temporary folder.
         if retrieve_temporary_list:
             filenames = os.listdir(retrieved_temporary_folder)
             file_opener = lambda filename: open(os.path.join(retrieved_temporary_folder, filename))
         else:
-            filenames = retrieved.base.repository.list_object_names()
-            file_opener = retrieved.base.repository.open
-
-        try:
-            logs, self.output_parameters = self.parse_stdout(stdout_raw)
-        except Exception as exc:
-            self.logger.error(traceback.format_exc())
-            return self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION.format(exception=exc)
-
-        self.emit_logs(logs)
-
-        # Scan logs for known errors
-        if 'ERROR_PARENT_XML_MISSING' in logs['error']:
-            return self.exit_codes.ERROR_PARENT_XML_MISSING
-        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE' in logs['error']:
-            return self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
+            filenames = self.retrieved.base.repository.list_object_names()
+            file_opener = self.retrieved.base.repository.open
 
         # The following check should in principle always succeed since the iflag should in principle be set by the
         # `PpCalculation` plugin which only ever sets 0 - 4, but we check in order for the code not to except.
         iflag = self.node.inputs.parameters.base.attributes.get('PLOT')['iflag']
         if iflag not in range(5):
             return self.exit_codes.ERROR_UNSUPPORTED_DATAFILE_FORMAT
 
@@ -133,108 +126,61 @@
                     with file_opener(filename) as handle:
                         data_raw = handle.read()
                 except OSError:
                     return self.exit_codes.ERROR_OUTPUT_DATAFILE_READ.format(filename=filename)
                 # Parse the file
                 try:
                     key = get_key_from_filename(filename)
-                    data_parsed.append((key, parsers[iflag](data_raw)))
+                    data_parsed.append((key, parsers[iflag](data_raw, self.units_dict[parsed_data['plot_num']])))
                     del data_raw
-                except Exception:  # pylint: disable=broad-except
-                    return self.exit_codes.ERROR_OUTPUT_DATAFILE_PARSE.format(filename=filename)
+                except Exception as exception:  # pylint: disable=broad-except
+                    return self.exit_codes.ERROR_OUTPUT_DATAFILE_PARSE.format(filename=filename, exception=exception)
 
         # If we don't have any parsed files, we exit. Note that this will not catch the case where there should be more
         # than one file, but the engine did not retrieve all of them. Since often we anyway don't know how many files
         # should be retrieved there really is no way to check this explicitly.
         if not data_parsed:
             return self.exit_codes.ERROR_OUTPUT_DATAFILE_MISSING.format(filename=filename_prefix)
 
         # Create output nodes
         if len(data_parsed) == 1:
             self.out('output_data', data_parsed[0][1])
         else:
             self.out('output_data_multiple', dict(data_parsed))
 
-        self.out('output_parameters', orm.Dict(self.output_parameters))
-
-    def parse_stdout(self, stdout_str):
-        """
-        Parses the output written to StdOut to retrieve basic information about the post processing
-
-        :param stdout_str: the stdout file read in as a single string
-        """
+        return self.exit(logs=logs)
 
-        def detect_important_message(logs, line):
-            """
-            Detect know errors and warnings printed in the stdout
-
-            :param logs:
-            :param line: a line from the stdout as a string
-            """
-            message_map = {
-                'error': {
-                    'xml data file not found': 'ERROR_PARENT_XML_MISSING'
-                },
-                'warning': {
-                    'Warning:': None,
-                    'DEPRECATED:': None,
-                }
-            }
-
-            # Match any known error and warning messages
-            for marker, message in message_map['error'].items():
-                if marker in line:
-                    if message is None:
-                        message = line
-                    logs.error.append(message)
-
-            for marker, message in message_map['warning'].items():
-                if marker in line:
-                    if message is None:
-                        message = line
-                    logs.warning.append(message)
-
-        stdout_lines = stdout_str.splitlines()
-        logs = get_logging_container()
-        output_dict = {}
-
-        # Check for job completion, indicating that pp.x exited without interruption, even if there was an error.
-        for line in stdout_lines:
-            if 'JOB DONE' in line:
-                break
-        else:
-            logs.error.append('ERROR_OUTPUT_STDOUT_INCOMPLETE')
-
-        # Detect any issues and detect job completion
-        for line in stdout_lines:
-            detect_important_message(logs, line)
+    def parse_stdout(self, stdout: str, logs: AttributeDict) -> Tuple[dict, AttributeDict]:
+        """Parse the ``stdout`` content of a Quantum ESPRESSO ``pp.x`` calculation."""
+        parsed_data = {}
 
         # Parse useful data from stdout
-        for line in stdout_lines:
+        for line in stdout.splitlines():
             if 'Check:' in line:  # QE < 6.5
                 split_line = line.split('=')
                 if 'negative/imaginary' in line:  # QE6.1-6.3
-                    output_dict['negative_core_charge'] = float(split_line[-1].split()[0])
-                    output_dict['imaginary_core_charge'] = float(split_line[-1].split()[-1])
+                    parsed_data['negative_core_charge'] = float(split_line[-1].split()[0])
+                    parsed_data['imaginary_core_charge'] = float(split_line[-1].split()[-1])
                 else:  # QE6.4
-                    output_dict['negative_core_charge'] = float(split_line[1])
+                    parsed_data['negative_core_charge'] = float(split_line[1])
             if 'Min, Max, imaginary charge:' in line:
                 split_line = line.split()
-                output_dict['charge_min'] = float(split_line[-3])
-                output_dict['charge_max'] = float(split_line[-2])
-                output_dict['charge_img'] = float(split_line[-1])
+                parsed_data['charge_min'] = float(split_line[-3])
+                parsed_data['charge_max'] = float(split_line[-2])
+                parsed_data['charge_img'] = float(split_line[-1])
             if 'plot_num = ' in line:
-                output_dict['plot_num'] = int(line.split('=')[1])
+                parsed_data['plot_num'] = int(line.split('=')[1])
             if 'Plot Type:' in line:
-                output_dict['plot_type'] = line.split('Output format')[0].split(':')[-1].strip()
-                output_dict['output_format'] = line.split(':')[-1].strip()
+                parsed_data['plot_type'] = line.split('Output format')[0].split(':')[-1].strip()
+                parsed_data['output_format'] = line.split(':')[-1].strip()
 
-        return logs, output_dict
+        return parsed_data, logs
 
-    def parse_gnuplot1D(self, data_file_str):
+    @staticmethod
+    def parse_gnuplot1D(data_file_str, data_units):
         """Parse 1D GNUPlot formatted output.
 
         :param data_file_str: the data file read in as a single string
         """
         data_lines = data_file_str.splitlines()
 
         n_col = len(data_lines[0].split())
@@ -246,61 +192,61 @@
             data_integral = []
             for line in data_lines:
                 split_line = line.split()
                 coords.append(float(split_line[0]))
                 data.append(float(split_line[1]))
             y_data = [data]
             y_names = ['data']
-            y_units = [self.units_dict[self.output_parameters['plot_num']]]
+            y_units = [data_units]
 
         # 1D case with spherical averaging
         if n_col == 3:
             coords = []
             data = []
             data_integral = []
             for line in data_lines:
                 split_line = line.split()
                 coords.append(float(split_line[0]))
                 data.append(float(split_line[1]))
                 data_integral.append(float(split_line[2]))
             y_data = [data, data_integral]
             y_names = ['data', 'integrated_data']
-            unit = self.units_dict[self.output_parameters['plot_num']]
-            y_units = [unit, unit.replace('bohr^3', 'bohr')]
+            y_units = [data_units, data_units.replace('bohr^3', 'bohr')]
 
         x_units = 'bohr'
         arraydata = orm.ArrayData()
         arraydata.set_array('x_coordinates', np.array(coords))
         arraydata.set_array('x_coordinates_units', np.array(x_units))
         for name, data, units in zip(y_names, y_data, y_units):
             arraydata.set_array(name, np.array(data))
             arraydata.set_array(name + '_units', np.array(units))
 
         return arraydata
 
-    def parse_gnuplot_polar(self, data_file_str):
+    @staticmethod
+    def parse_gnuplot_polar(data_file_str, data_units):
         """Parse 2D Polar GNUPlot formatted, single column output.
 
         :param data_file_str: the data file read in as a single string
         """
         data_lines = data_file_str.splitlines()
         data_lines.pop(0)  # First line is a header
 
         data = []
         for line in data_lines:
             data.append(float(line))
-        data_units = [self.units_dict[self.output_parameters['plot_num']]]
 
         arraydata = orm.ArrayData()
         arraydata.set_array('data', np.array(data))
-        arraydata.set_array('data_units', np.array(data_units))
+        arraydata.set_array('data_units', np.array([data_units]))
 
         return arraydata
 
-    def parse_gnuplot2D(self, data_file_str):
+    @staticmethod
+    def parse_gnuplot2D(data_file_str, data_units):
         """Parse 2D GNUPlot formatted output.
 
         :param data_file_str: the data file read in as a single string
         """
         data_lines = data_file_str.splitlines()
 
         coords = []
@@ -312,24 +258,24 @@
                 continue
             else:
                 split_line = stripped.split()
                 coords.append([float(split_line[0]), float(split_line[1])])
                 data.append(float(split_line[2]))
 
         coords_units = 'bohr'
-        data_units = self.units_dict[self.output_parameters['plot_num']]
         arraydata = orm.ArrayData()
         arraydata.set_array('xy_coordinates', np.array(coords))
         arraydata.set_array('data', np.array(data))
         arraydata.set_array('xy_coordinates_units', np.array(coords_units))
         arraydata.set_array('data_units', np.array(data_units))
 
         return arraydata
 
-    def parse_gaussian(self, data_file_str):
+    @staticmethod
+    def parse_gaussian(data_file_str, data_units):
         """Parse Gaussian Cube formatted output.
 
         :param data_file_str: the data file read in as a single string
         """
         lines = data_file_str.splitlines()
 
         atoms_line = lines[2].split()
@@ -358,15 +304,14 @@
         for line in data_lines:
             ls = line.split()
             data_array[cursor:cursor + len(ls)] = ls
             cursor += len(ls)
         data_array = data_array.reshape((xdim, ydim, zdim))
 
         coordinates_units = 'bohr'
-        data_units = self.units_dict[self.output_parameters['plot_num']]
 
         arraydata = orm.ArrayData()
         arraydata.set_array('voxel', voxel_array)
         arraydata.set_array('data', data_array)
         arraydata.set_array('data_units', np.array(data_units))
         arraydata.set_array('coordinates_units', np.array(coordinates_units))
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/projwfc.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/projwfc.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,22 +4,18 @@
 import re
 
 from aiida.orm import BandsData, Dict, ProjectionData, XyData
 from aiida.plugins import OrbitalFactory
 import numpy as np
 
 from aiida_quantumespresso.parsers import QEOutputParsingError
-from aiida_quantumespresso.parsers.parse_raw.base import (
-    convert_qe_to_aiida_structure,
-    convert_qe_to_kpoints,
-    parse_output_base,
-)
+from aiida_quantumespresso.parsers.parse_raw.base import convert_qe_to_aiida_structure, convert_qe_to_kpoints
 from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
 def find_orbitals_from_statelines(out_info_dict):
     """This function reads in all the state_lines, that is, the lines describing which atomic states, taken from the
     pseudopotential, are used for the projection. Then it converts these state_lines into a set of orbitals.
 
     :param out_info_dict: contains various technical internals useful in parsing
@@ -268,109 +264,97 @@
         else:
             for i in range(fa, np.shape(this_array)[1], mf):
                 out_arrays.append(this_array[:, i])
 
     return out_arrays
 
 
-class ProjwfcParser(Parser):
-    """This class is the implementation of the Parser class for projwfc.x in Quantum Espresso.
+class ProjwfcParser(BaseParser):
+    """``Parser`` implementation for the ``ProjwfcCalculation`` calculation job class.
 
     Parses projection arrays that map the projection onto each point in the bands structure, as well as pdos arrays,
     which map the projected density of states onto an energy axis.
     """
 
     def parse(self, **kwargs):
-        """Parses the datafolder, stores results.
+        """Parse the retrieved files from a ``ProjwfcCalculation`` into output nodes."""
+        # we create a dictionary the progressively accumulates more info
+        out_info_dict = {}
+
+        logs = get_logging_container()
+
+        stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
+        out_info_dict['out_file'] = stdout.split('\n')
+
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
+
+        self.out('output_parameters', Dict(parsed_data))
+
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
 
-        Retrieves projwfc output, and some basic information from the out_file, such as warnings and wall_time
-        """
-        retrieved = self.retrieved
-        # Get the temporary retrieved folder
         try:
             retrieved_temporary_folder = kwargs['retrieved_temporary_folder']
         except KeyError:
-            return self.exit(self.exit_codes.ERROR_NO_RETRIEVED_TEMPORARY_FOLDER)
-
-        # Read standard out
-        try:
-            filename_stdout = self.node.get_option('output_filename')  # or get_attribute(), but this is clearer
-            with retrieved.base.repository.open(filename_stdout, 'r') as fil:
-                out_file = fil.readlines()
-        except OSError:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
-
-        job_done = False
-        for i in range(len(out_file)):
-            line = out_file[-i]
-            if 'JOB DONE' in line:
-                job_done = True
-                break
-        if not job_done:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE)
-
-        # Parse basic info and warnings, and output them as output_parmeters
-        parsed_data, logs = parse_output_base(out_file, 'PROJWFC')
-        self.emit_logs(logs)
-        self.out('output_parameters', Dict(parsed_data))
+            return self.exit(self.exit_codes.ERROR_NO_RETRIEVED_TEMPORARY_FOLDER, logs)
 
         # Parse the XML to obtain the `structure`, `kpoints` and spin-related settings from the parent calculation
         self.exit_code_xml = None
         parsed_xml, logs_xml = self._parse_xml(retrieved_temporary_folder)
         self.emit_logs(logs_xml)
 
         if self.exit_code_xml:
             return self.exit(self.exit_code_xml)
 
-        # we create a dictionary the progressively accumulates more info
-        out_info_dict = {}
-
         out_info_dict['structure'] = convert_qe_to_aiida_structure(parsed_xml['structure'])
         out_info_dict['kpoints'] = convert_qe_to_kpoints(parsed_xml, out_info_dict['structure'])
         out_info_dict['nspin'] = parsed_xml.get('number_of_spin_components')
         out_info_dict['collinear'] = not parsed_xml.get('non_colinear_calculation')
         out_info_dict['spinorbit'] = parsed_xml.get('spin_orbit_calculation')
         out_info_dict['spin'] = out_info_dict['nspin'] == 2
 
         # check and read pdos_tot file
-        out_filenames = retrieved.base.repository.list_object_names()
+        out_filenames = self.retrieved.base.repository.list_object_names()
         try:
             pdostot_filename = fnmatch.filter(out_filenames, '*pdos_tot*')[0]
-            with retrieved.base.repository.open(pdostot_filename, 'r') as pdostot_file:
+            with self.retrieved.base.repository.open(pdostot_filename, 'r') as pdostot_file:
                 # Columns: Energy(eV), Ldos, Pdos
                 pdostot_array = np.atleast_2d(np.genfromtxt(pdostot_file))
                 energy = pdostot_array[:, 0]
                 dos = pdostot_array[:, 1]
         except (OSError, KeyError):
-            return self.exit(self.exit_codes.ERROR_READING_PDOSTOT_FILE)
+            return self.exit(self.exit_codes.ERROR_READING_PDOSTOT_FILE, logs)
 
         # check and read all of the individual pdos_atm files
         pdos_atm_filenames = fnmatch.filter(out_filenames, '*pdos_atm*')
         pdos_atm_array_dict = {}
         for name in pdos_atm_filenames:
-            with retrieved.base.repository.open(name, 'r') as pdosatm_file:
+            with self.retrieved.base.repository.open(name, 'r') as pdosatm_file:
                 pdos_atm_array_dict[name] = np.atleast_2d(np.genfromtxt(pdosatm_file))
 
         # finding the bands and projections
-        out_info_dict['out_file'] = out_file
         out_info_dict['energy'] = energy
         out_info_dict['pdos_atm_array_dict'] = pdos_atm_array_dict
         try:
             new_nodes_list = self._parse_bands_and_projections(out_info_dict)
         except QEOutputParsingError as err:
             self.logger.error(f'Error parsing bands and projections: {err}')
-            return self.exit(self.exit_codes.ERROR_PARSING_PROJECTIONS)
+            return self.exit(self.exit_codes.ERROR_PARSING_PROJECTIONS, logs)
         for linkname, node in new_nodes_list:
             self.out(linkname, node)
 
         Dos_out = XyData()
         Dos_out.set_x(energy, 'Energy', 'eV')
         Dos_out.set_y(dos, 'Dos', 'states/eV')
         self.out('Dos', Dos_out)
 
+        return self.exit(logs=logs)
+
     def _parse_xml(self, retrieved_temporary_folder):
         """Parse the XML file.
 
         The XML must be parsed in order to obtain the required information for the orbital parsing.
         """
         from .parse_xml.exceptions import XMLParseError, XMLUnsupportedFormatError
         from .parse_xml.pw.parse import parse_xml
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pw.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from aiida.common import exceptions
 from aiida.engine import ExitCode
 import numpy
 
 from aiida_quantumespresso.calculations.pw import PwCalculation
 from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 from .parse_raw.pw import reduce_symmetries
 
 
-class PwParser(Parser):
+class PwParser(BaseParser):
     """`Parser` implementation for the `PwCalculation` calculation job class."""
 
     def parse(self, **kwargs):
         """Parse the retrieved files of a completed `PwCalculation` into output nodes.
 
         Two nodes that are expected are the default 'retrieved' `FolderData` node which will store the retrieved files
         permanently in the repository. The second required node is a filepath under the key `retrieved_temporary_files`
@@ -270,14 +270,16 @@
         parameters = self.node.inputs.parameters.get_dict()
         threshold_forces = parameters.get('CONTROL', {}).get('forc_conv_thr', pw.forc_conv_thr)
         threshold_stress = parameters.get('CELL', {}).get('press_conv_thr', pw.press_conv_thr)
         external_pressure = parameters.get('CELL', {}).get('press', 0)
 
         if 'settings' in self.node.inputs:
             settings = _uppercase_dict(self.node.inputs.settings.get_dict(), dict_name='settings')
+        else:
+            settings = {}
 
         fixed_coords = settings.get('FIXED_COORDS', None)
 
         # Through the `cell_dofree` the degrees of freedom of the cell can be constrained, which makes the threshold on
         # the stress hard to interpret. Therefore, unless the `cell_dofree` is set to the default `all` where the cell
         # is fully unconstrained, the stress is ignored even if an explicit `press_conv_thr` is specified in the inputs.
         constrained_cell = parameters.get('CELL', {}).get('cell_dofree', 'all') != 'all'
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2gw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/pw2gw.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 # -*- coding: utf-8 -*-
 """`Parser` implementation for the `Pw2gwCalculation` calculation job class."""
 import io
 
-from aiida import orm
+from aiida.orm import ArrayData, Dict
 import numpy as np
 
-from aiida_quantumespresso.calculations.pw2gw import Pw2gwCalculation
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
-class Pw2gwParser(Parser):
-    """`Parser` implementation for the `Pw2gwCalculation` calculation job class."""
+class Pw2gwParser(BaseParser):
+    """``Parser`` implementation for the ``Pw2gwCalculation`` calculation job class."""
 
     def parse(self, **kwargs):
-        """Parse the retrieved files of a completed `Pw2gwCalculation` into output nodes.
+        """Parse the retrieved files of a completed ``Pw2gwCalculation`` into output nodes.
 
         Two nodes that are expected are the default 'retrieved' `FolderData` node which will store the retrieved files
-        permanently in the repository. The second required node is a filepath under the key `retrieved_temporary_files`
-        which should contain the temporary retrieved files.
+        permanently in the repository. The second required node is a filepath under the key
+        ``retrieved_temporary_files`` which should contain the temporary retrieved files.
         """
-        self.exit_code_stdout = None
-        self.exit_code_eps = None
+        logs = get_logging_container()
 
-        # Parse the pw2gw stout file
-        data, logs_stdout = self.parse_stdout()
+        _, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
 
-        self.emit_logs(logs_stdout)
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
 
-        if self.exit_code_stdout:
-            return self.exit(self.exit_code_stdout)
+        self.out('output_parameters', Dict(dict=parsed_data))
 
-        self.out('output_parameters', orm.Dict(data))
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
 
-        # Parse the pw2g outputfiles
+        self.exit_code_eps = None
         eps = self.parse_eps_files()
 
         if self.exit_code_eps:
-            return self.exit(self.exit_code_eps)
+            return self.exit(self.exit_code_eps, logs)
 
         self.out('eps', eps)
 
+        return self.exit(logs=logs)
+
     def parse_eps_files(self):
-        """Parse the eps*.dat files produced by pw2gw.x and store them in the `eps` node."""
+        """Parse the ``eps*.dat`` files produced by ``pw2gw.x``."""
         retrieved = self.retrieved
         retrieved_names = retrieved.base.repository.list_object_names()
 
-        files = Pw2gwCalculation._internal_retrieve_list
+        files = self.node.process_class._internal_retrieve_list
         if any(_ not in retrieved_names for _ in files):
             self.exit_code_eps = self.exit_codes.ERROR_OUTPUT_FILES
             return
 
         energy = None
-        eps = orm.ArrayData()
-        for name in Pw2gwCalculation._internal_retrieve_list:
+        eps = ArrayData()
+        for name in self.node.process_class._internal_retrieve_list:
             content = retrieved.base.repository.get_object_content(name)
             base = name.split('.')[0]
 
             try:
                 data = np.loadtxt(io.StringIO(content))
             except ValueError:
                 self.exit_code_eps = self.exit_codes.ERROR_OUTPUT_FILES
@@ -73,41 +75,7 @@
             elif not np.allclose(x, energy):
                 self.exit_code_eps = self.exit_codes.ERROR_OUTPUT_FILES_ENERGY_MISMATCH
                 return
 
             eps.set_array(base, y)
 
         return eps
-
-    def parse_stdout(self):
-        """Parse the stdout file of pw2gw to build the `output_parameters` node."""
-        from aiida_quantumespresso.parsers.parse_raw.pw2gw import parse_stdout
-        from aiida_quantumespresso.utils.mapping import get_logging_container
-
-        logs = get_logging_container()
-        parsed_data = {}
-
-        filename_stdout = self.node.base.attributes.get('output_filename')
-
-        if filename_stdout not in self.retrieved.base.repository.list_object_names():
-            self.exit_code_stdout = self.exit_codes.ERROR_OUTPUT_STDOUT_MISSING
-            return parsed_data, logs
-
-        try:
-            stdout = self.retrieved.base.repository.get_object_content(filename_stdout)
-        except IOError:
-            self.exit_code_stdout = self.exit_codes.ERROR_OUTPUT_STDOUT_READ
-            return parsed_data, logs
-
-        try:
-            parsed_data, logs = parse_stdout(stdout)
-        except Exception as exc:
-            import traceback
-            traceback.print_exc()
-            self.exit_code_stdout = self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION.format(exception=exc)
-
-        # If the stdout was incomplete, most likely the job was interrupted before it could cleanly finish, so the
-        # output files are most likely corrupt and cannot be restarted from
-        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE' in logs['error']:
-            self.exit_code_stdout = self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
-
-        return parsed_data, logs
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2wannier90.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/parsers/q2r.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # -*- coding: utf-8 -*-
 from aiida.orm import Dict
 
-from aiida_quantumespresso.parsers.parse_raw.base import parse_output_base
+from aiida_quantumespresso.data.force_constants import ForceConstantsData
+from aiida_quantumespresso.utils.mapping import get_logging_container
 
-from .base import Parser
+from .base import BaseParser
 
 
-class Pw2wannier90Parser(Parser):
-    """`Parser` implementation for the `Pw2wannierCalculation` calculation job class."""
+class Q2rParser(BaseParser):
+    """``Parser`` implementation for the ``Q2rCalculation`` calculation job class."""
 
     def parse(self, **kwargs):
-        """Parse the retrieved files of a completed `Pw2wannierCalculation` into output nodes.
+        """Parse the retrieved files of a ``Q2rCalculation`` into output nodes."""
+        logs = get_logging_container()
 
-        Two nodes that are expected are the default 'retrieved' `FolderData` node which will store the retrieved files
-        permanently in the repository.
-        """
-        try:
-            filename_stdout = self.node.get_option('output_filename')  # or get_attribute(), but this is clearer
-            with self.retrieved.base.repository.open(filename_stdout, 'r') as fil:
-                out_file = fil.read()
-        except OSError:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_READ)
+        _, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
 
-        parsed_data, logs = parse_output_base(out_file, codename='PW2WANNIER')
-        self.emit_logs(logs)
+        base_exit_code = self.check_base_errors(logs)
+        if base_exit_code:
+            return self.exit(base_exit_code, logs)
 
         self.out('output_parameters', Dict(parsed_data))
 
-        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE' in logs.error:
-            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE)
-        elif logs.error:
-            return self.exit(self.exit_codes.ERROR_GENERIC_QE_ERROR)
+        if 'ERROR_OUTPUT_STDOUT_INCOMPLETE'in logs.error:
+            return self.exit(self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE, logs)
+
+        filename_force_constants = self.node.process_class._FORCE_CONSTANTS_NAME
+
+        if filename_force_constants not in self.retrieved.base.repository.list_object_names():
+            return self.exit(self.exit_codes.ERROR_READING_FORCE_CONSTANTS_FILE, logs)
+
+        with self.retrieved.base.repository.open(filename_force_constants, 'rb') as handle:
+            self.out('force_constants', ForceConstantsData(file=handle))
+
+        return self.exit(logs=logs)
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/cpinputparser.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/cpinputparser.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/pwinputparser.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/tools/pwinputparser.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/bands.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/bands.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/convert.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/convert.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/hubbard.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/hubbard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Utility class for handling the :class:`data.hubbard_structure.HubbardStructureData`."""
+"""Utility class for handling the :class:`aiida_quantumespresso.data.hubbard_structure.HubbardStructureData`."""
 # pylint: disable=no-name-in-module
 from itertools import product
 import os
 from typing import List, Tuple, Union
 
 from aiida.orm import StructureData
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/linalg.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/mapping.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/pw.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/pw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/resources.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/restart.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/restart.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/validation/trajectory.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/utils/validation/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/matdyn/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/matdyn/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pdos.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pdos.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 """
 from aiida import orm, plugins
 from aiida.common import AttributeDict
 from aiida.engine import ToContext, WorkChain, if_
 from aiida.orm.nodes.data.base import to_aiida_type
 import jsonschema
 
-from aiida_quantumespresso.calculations.pw import PwCalculation
 from aiida_quantumespresso.utils.mapping import prepare_process_inputs
 
 from .protocols.utils import ProtocolMixin
 
 
 def get_parameter_schema():
     """Return the ``PdosWorkChain`` input parameter schema."""
@@ -238,21 +237,20 @@
                 'required': False,
                 'populate_defaults': False,
             }
         )
         spec.expose_inputs(
             PwBaseWorkChain,
             namespace='nscf',
-            exclude=('clean_workdir', 'pw.structure'),
+            exclude=('clean_workdir', 'pw.structure', 'pw.parent_folder'),
             namespace_options={
                 'help': 'Inputs for the `PwBaseWorkChain` of the `nscf` calculation.',
                 'validator': validate_nscf
             }
         )
-        spec.inputs['nscf']['pw'].validator = PwCalculation.validate_inputs_base
         spec.expose_inputs(
             DosCalculation,
             namespace='dos',
             exclude=('parent_folder',),
             namespace_options={
                 'help': ('Input parameters for the `dos.x` calculation. Note that the `Emin`, `Emax` and `DeltaE` '
                          'values have to match with those in the `projwfc` inputs.'),
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/ph/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/ph/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/utils.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 """Utilities to manipulate the workflow input protocols."""
 import pathlib
 from typing import Optional, Union
 
-from aiida.plugins import DataFactory, GroupFactory
+from aiida.orm import StructureData
+from aiida_pseudo.groups.family import PseudoPotentialFamily
 import yaml
 
-StructureData = DataFactory('core.structure')
-PseudoPotentialFamily = GroupFactory('pseudo.family')
-
 
 class ProtocolMixin:
     """Utility class for processes to build input mappings for a given protocol based on a YAML configuration file."""
 
     @classmethod
     def get_protocol_filepath(cls) -> pathlib.Path:
         """Return the ``pathlib.Path`` to the ``.yaml`` file that defines the protocols."""
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/bands.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/bands.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 """Workchain to compute a band structure for a given structure using Quantum ESPRESSO pw.x."""
 from aiida import orm
 from aiida.common import AttributeDict
 from aiida.engine import ToContext, WorkChain, if_
 
 from aiida_quantumespresso.calculations.functions.seekpath_structure_analysis import seekpath_structure_analysis
-from aiida_quantumespresso.calculations.pw import PwCalculation
 from aiida_quantumespresso.utils.mapping import prepare_process_inputs
 from aiida_quantumespresso.workflows.pw.base import PwBaseWorkChain
 from aiida_quantumespresso.workflows.pw.relax import PwRelaxWorkChain
 
 from ..protocols.utils import ProtocolMixin
 
 
@@ -56,26 +55,26 @@
         spec.expose_inputs(PwRelaxWorkChain, namespace='relax', exclude=('clean_workdir', 'structure'),
             namespace_options={'required': False, 'populate_defaults': False,
             'help': 'Inputs for the `PwRelaxWorkChain`, if not specified at all, the relaxation step is skipped.'})
         spec.expose_inputs(PwBaseWorkChain, namespace='scf',
             exclude=('clean_workdir', 'pw.structure'),
             namespace_options={'help': 'Inputs for the `PwBaseWorkChain` for the SCF calculation.'})
         spec.expose_inputs(PwBaseWorkChain, namespace='bands',
-            exclude=('clean_workdir', 'pw.structure', 'pw.kpoints', 'pw.kpoints_distance'),
+            exclude=('clean_workdir', 'pw.structure', 'pw.kpoints', 'pw.kpoints_distance', 'pw.parent_folder'),
             namespace_options={'help': 'Inputs for the `PwBaseWorkChain` for the BANDS calculation.'})
         spec.input('structure', valid_type=orm.StructureData, help='The inputs structure.')
         spec.input('clean_workdir', valid_type=orm.Bool, default=lambda: orm.Bool(False),
             help='If `True`, work directories of all called calculation will be cleaned at the end of execution.')
         spec.input('nbands_factor', valid_type=orm.Float, required=False,
             help='The number of bands for the BANDS calculation is that used for the SCF multiplied by this factor.')
         spec.input('bands_kpoints', valid_type=orm.KpointsData, required=False,
             help='Explicit kpoints to use for the BANDS calculation. Specify either this or `bands_kpoints_distance`.')
         spec.input('bands_kpoints_distance', valid_type=orm.Float, required=False,
             help='Minimum kpoints distance for the BANDS calculation. Specify either this or `bands_kpoints`.')
-        spec.inputs['bands']['pw'].validator = PwCalculation.validate_inputs_base
+
         spec.inputs.validator = validate_inputs
         spec.outline(
             cls.setup,
             if_(cls.should_run_relax)(
                 cls.run_relax,
                 cls.inspect_relax,
             ),
```

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/relax.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/pw/relax.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/q2r/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/q2r/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xps.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xps.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/base.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/core.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/core.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py` & `aiida_quantumespresso-4.4.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.3.0/PKG-INFO` & `aiida_quantumespresso-4.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-quantumespresso
-Version: 4.3.0
+Version: 4.4.0
 Summary: The official AiiDA plugin for Quantum ESPRESSO
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -16,25 +16,26 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiida_core[atomic_tools]~=2.3
 Requires-Dist: aiida-pseudo~=1.0
 Requires-Dist: click~=8.0
 Requires-Dist: importlib_resources
 Requires-Dist: jsonschema
 Requires-Dist: numpy
-Requires-Dist: pydantic
+Requires-Dist: pydantic~=1.10,>=1.10.8
 Requires-Dist: packaging
 Requires-Dist: qe-tools~=2.0
 Requires-Dist: xmlschema~=1.2,>=1.2.5
-Requires-Dist: sphinx~=4.1 ; extra == "docs"
-Requires-Dist: sphinx-copybutton~=0.5.0 ; extra == "docs"
-Requires-Dist: sphinx-book-theme~=0.3.2 ; extra == "docs"
-Requires-Dist: sphinx-click~=4.0 ; extra == "docs"
-Requires-Dist: sphinx-design~=0.0.13 ; extra == "docs"
+Requires-Dist: sphinx~=6.2.1 ; extra == "docs"
+Requires-Dist: sphinx-copybutton~=0.5.2 ; extra == "docs"
+Requires-Dist: sphinx-book-theme~=1.0.1 ; extra == "docs"
+Requires-Dist: sphinx-click~=4.4.0 ; extra == "docs"
+Requires-Dist: sphinx-design~=0.4.1 ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive~=0.1.0 ; extra == "docs"
-Requires-Dist: sphinx-autoapi ; extra == "docs"
+Requires-Dist: sphinx-autoapi~=2.0.1 ; extra == "docs"
+Requires-Dist: myst_parser~=1.0.0 ; extra == "docs"
 Requires-Dist: pre-commit~=2.17 ; extra == "pre-commit"
 Requires-Dist: pylint~=2.17.2 ; extra == "pre-commit"
 Requires-Dist: pylint-aiida~=0.1.1 ; extra == "pre-commit"
 Requires-Dist: toml ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3 ; extra == "tests"
 Requires-Dist: pytest~=6.0 ; extra == "tests"
 Requires-Dist: pytest-regressions~=2.3 ; extra == "tests"
```

