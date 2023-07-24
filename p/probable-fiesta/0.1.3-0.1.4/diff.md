# Comparing `tmp/probable_fiesta-0.1.3.tar.gz` & `tmp/probable_fiesta-0.1.4.tar.gz`

## Comparing `probable_fiesta-0.1.3.tar` & `probable_fiesta-0.1.4.tar`

### file list

```diff
@@ -1,153 +1,144 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.env
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/env
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/requirements.txt
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tox.ini
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.github/workflows/python_app.yml
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/README.md
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/.gitignore
--rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/coverage_html.js
--rw-r--r--   0        0        0    18544 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_args_parse_py.html
--rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html
--rw-r--r--   0        0        0    17408 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_parser_builder_py.html
--rw-r--r--   0        0        0    29534 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html
--rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_factory_py.html
--rw-r--r--   0        0        0    32638 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_py.html
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_3b40d2e1b447d1de___about___py.html
--rw-r--r--   0        0        0    45718 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html
--rw-r--r--   0        0        0    58461 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html
--rw-r--r--   0        0        0    16956 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_py.html
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html
--rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_py.html
--rw-r--r--   0        0        0    56232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html
--rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html
--rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html
--rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_app_builder_py.html
--rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_app_py.html
--rw-r--r--   0        0        0    20353 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_929858da485d1af8_logging_config_py.html
--rw-r--r--   0        0        0    38348 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_9610c8957119e03c_main_py.html
--rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_a44f0ac069e85531_test_main_app_py.html
--rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_a44f0ac069e85531_test_v1_py.html
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_b5ab6064aa946d24_v1_py.html
--rw-r--r--   0        0        0    38305 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_config_builder_py.html
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_config_factory_py.html
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_default_config_py.html
--rw-r--r--   0        0        0    12207 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_variables_py.html
--rw-r--r--   0        0        0    32979 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_builder_py.html
--rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_factory_py.html
--rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_py.html
--rw-r--r--   0        0        0    31733 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_queue_py.html
--rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html
--rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html
--rw-r--r--   0        0        0    29275 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_py.html
--rw-r--r--   0        0        0    24515 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/favicon_32.png
--rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/status.json
--rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/htmlcov/style.css
--rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/build_install.sh
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/build_publish.sh
--rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/run_tests.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/templater.sh
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/scripts/test_coverage.sh
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/__init__.py
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_abstract_machine.py
--rw-r--r--   0        0        0    10852 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_builder.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/command_context_factory.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_builder.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_factory.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_holder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/my_args_parser.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_builder.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/__init__.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_builder.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_factory.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_queue.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_queue_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/_init__.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/default_config.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/module_config.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/__init__.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder_factory.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/__init__.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/logger_module.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/logging_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/__init__.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_abstract_machine.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_builder.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_factory.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/run/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/src/probable_fiesta/run/main.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/__about__.py.j2
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/hatch.toml
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/hatch.toml.j2
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/make_skeleton.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/pyproject.toml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/pyproject.toml.j2
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/run___init__.py.j2
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/tox.ini
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/tox.ini.j2
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/write_templates.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/app/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/cli/__init__.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/run/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/templates/src/probable_fiesta/run/main.py
--rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/test_main_app.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/test_v1.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/app/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/app/builder/__init__.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/app/builder/test_app_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/cli/builder/__init__.py
--rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/cli/builder/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_builder.py
--rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_context_factory.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_factory.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/command/builder/test_command_queue.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/builder/__init__.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/builder/test_config.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/config/builder/test_config_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/builder/__init__.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/builder/test_logger.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/tests/logger/builder/test_logger_factory.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/.gitignore
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/LICENSE
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/hatch.toml
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 probable_fiesta-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/.env
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/env
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tox.ini
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/.github/workflows/python_app.yml
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/.gitignore
+-rw-r--r--   0        0        0    20650 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0    18544 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_0293064cae6f51b1_args_parse_py.html
+-rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html
+-rw-r--r--   0        0        0    17408 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_0293064cae6f51b1_parser_builder_py.html
+-rw-r--r--   0        0        0    29534 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html
+-rw-r--r--   0        0        0    11939 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_309aba7555c96ec5_logger_factory_py.html
+-rw-r--r--   0        0        0    32638 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_309aba7555c96ec5_logger_py.html
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_3b40d2e1b447d1de___about___py.html
+-rw-r--r--   0        0        0    45718 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html
+-rw-r--r--   0        0        0    58461 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html
+-rw-r--r--   0        0        0    16956 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_app_py.html
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html
+-rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html
+-rw-r--r--   0        0        0     9775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_context_py.html
+-rw-r--r--   0        0        0    56232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html
+-rw-r--r--   0        0        0    17260 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html
+-rw-r--r--   0        0        0    33986 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html
+-rw-r--r--   0        0        0    16398 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_7a0574776d91e073_test_app_builder_py.html
+-rw-r--r--   0        0        0    14310 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_7a0574776d91e073_test_app_py.html
+-rw-r--r--   0        0        0    20353 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_929858da485d1af8_logging_config_py.html
+-rw-r--r--   0        0        0    38348 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_9610c8957119e03c_main_py.html
+-rw-r--r--   0        0        0    17287 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_a44f0ac069e85531_test_main_app_py.html
+-rw-r--r--   0        0        0    14163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_a44f0ac069e85531_test_v1_py.html
+-rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_b5ab6064aa946d24_v1_py.html
+-rw-r--r--   0        0        0    38305 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_config_builder_py.html
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_config_factory_py.html
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_default_config_py.html
+-rw-r--r--   0        0        0    12207 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_variables_py.html
+-rw-r--r--   0        0        0    32979 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_builder_py.html
+-rw-r--r--   0        0        0     8772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_factory_py.html
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_py.html
+-rw-r--r--   0        0        0    31733 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_queue_py.html
+-rw-r--r--   0        0        0    16599 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html
+-rw-r--r--   0        0        0    15012 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html
+-rw-r--r--   0        0        0    29275 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_py.html
+-rw-r--r--   0        0        0    24515 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/status.json
+-rw-r--r--   0        0        0    12429 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/htmlcov/style.css
+-rwxr-xr-x   0        0        0      587 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/scripts/build_install.sh
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/scripts/build_publish.sh
+-rwxr-xr-x   0        0        0      276 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/scripts/run_tests.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/scripts/templater.sh
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/scripts/test_coverage.sh
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/__init__.py
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/app_abstract_machine.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/app_builder.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/command_context_factory.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context_builder.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context_factory.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context_holder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/cli/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/my_args_parser.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/parser.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/parser_builder.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/parser_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/builder/__init__.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command_builder.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command_factory.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command_queue.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command_queue_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/_init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/default_config.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/module_config.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/builder/__init__.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/builder/config.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/builder/config_builder.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/config/builder/config_builder_factory.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/__init__.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/logger_module.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/logging_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/__init__.py
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger_abstract_machine.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger_builder.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger_factory.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/run/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/src/probable_fiesta/run/main.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/__about__.py.j2
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/hatch.toml
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/hatch.toml.j2
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/make_skeleton.py
+-rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/pyproject.toml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/pyproject.toml.j2
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/run___init__.py.j2
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/tox.ini
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/tox.ini.j2
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/write_templates.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/app/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/cli/__init__.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/run/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/templates/src/probable_fiesta/run/main.py
+-rw-r--r--   0        0        0     2506 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/test_main_app.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/test_v1.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/app/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/app/builder/__init__.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/app/builder/test_app_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/cli/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/cli/builder/__init__.py
+-rw-r--r--   0        0        0     5359 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/cli/builder/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/builder/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/builder/test_command.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/builder/test_command_builder.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/builder/test_command_context_factory.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/builder/test_command_factory.py
+-rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/command/builder/test_command_queue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/config/builder/__init__.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/config/builder/test_config.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/config/builder/test_config_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/logger/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/logger/builder/__init__.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/logger/builder/test_logger.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/tests/logger/builder/test_logger_factory.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/LICENSE
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/hatch.toml
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 probable_fiesta-0.1.4/PKG-INFO
```

### Comparing `probable_fiesta-0.1.3/requirements.txt` & `probable_fiesta-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/.github/workflows/python_app.yml` & `probable_fiesta-0.1.4/.github/workflows/python_app.yml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/.github/workflows/python_publish.yml` & `probable_fiesta-0.1.4/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/coverage_html.js` & `probable_fiesta-0.1.4/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_args_parse_py.html` & `probable_fiesta-0.1.4/htmlcov/d_0293064cae6f51b1_args_parse_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_0293064cae6f51b1_args_parser_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_0293064cae6f51b1_parser_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_0293064cae6f51b1_parser_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html` & `probable_fiesta-0.1.4/htmlcov/d_309aba7555c96ec5_logger_abstract_machine_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_309aba7555c96ec5_logger_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_309aba7555c96ec5_logger_py.html` & `probable_fiesta-0.1.4/htmlcov/d_309aba7555c96ec5_logger_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_3b40d2e1b447d1de___about___py.html` & `probable_fiesta-0.1.4/htmlcov/d_3b40d2e1b447d1de___about___py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_app_abstract_machine_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_app_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_app_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_context_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_context_holder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_context_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_context_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_57bbdeba1dacf1cd_my_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_5c9f86e17f38c9da_test_logger_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html` & `probable_fiesta-0.1.4/htmlcov/d_5c9f86e17f38c9da_test_logger_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_app_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_7a0574776d91e073_test_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_app_py.html` & `probable_fiesta-0.1.4/htmlcov/d_7a0574776d91e073_test_app_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_7a0574776d91e073_test_my_app_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_929858da485d1af8_logging_config_py.html` & `probable_fiesta-0.1.4/htmlcov/d_929858da485d1af8_logging_config_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_9610c8957119e03c_main_py.html` & `probable_fiesta-0.1.4/htmlcov/d_9610c8957119e03c_main_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_a44f0ac069e85531_test_main_app_py.html` & `probable_fiesta-0.1.4/htmlcov/d_a44f0ac069e85531_test_main_app_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_a44f0ac069e85531_test_v1_py.html` & `probable_fiesta-0.1.4/htmlcov/d_a44f0ac069e85531_test_v1_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_b5ab6064aa946d24_v1_py.html` & `probable_fiesta-0.1.4/htmlcov/d_b5ab6064aa946d24_v1_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_config_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_config_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_config_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_config_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_default_config_py.html` & `probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_default_config_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_c005feb2a2df0035_variables_py.html` & `probable_fiesta-0.1.4/htmlcov/d_c005feb2a2df0035_variables_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d52ee57c951d550c_command_queue_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d52ee57c951d550c_command_queue_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_builder_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_factory_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html` & `probable_fiesta-0.1.4/htmlcov/d_d76a1542e6a4e766_test_command_queue_py.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/favicon_32.png` & `probable_fiesta-0.1.4/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/index.html` & `probable_fiesta-0.1.4/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/keybd_closed.png` & `probable_fiesta-0.1.4/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/keybd_open.png` & `probable_fiesta-0.1.4/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/status.json` & `probable_fiesta-0.1.4/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/htmlcov/style.css` & `probable_fiesta-0.1.4/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/scripts/build_install.sh` & `probable_fiesta-0.1.4/scripts/build_install.sh`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/main.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/main.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_abstract_machine.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/builder/app_abstract_machine.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/app_builder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/builder/app_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,14 @@
         self.app.cleaned_args = self.clean_arg_function(arguments)
         return self
 
     def set_executables(self, executables: list):
         self.app.executables = executables
         return self
 
-    # TODO: This method needs work
     @staticmethod
     def map_short_flags(arguments, parsed_args):
         for arg in parsed_args.keys():
             clean = arg.split("_")[-1]
             if clean in arguments:
                 # update dictionary with long flag
                 arguments[arg] = arguments.pop(clean)
```

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_builder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_factory.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/app/builder/context_holder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/app/builder/context_holder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/my_args_parser.py` & `probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/my_args_parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser.py` & `probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_builder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/parser_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/cli/builder/parser_factory.py` & `probable_fiesta-0.1.4/src/probable_fiesta/cli/builder/parser_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command.py` & `probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_builder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/command/builder/command_queue.py` & `probable_fiesta-0.1.4/src/probable_fiesta/command/builder/command_queue.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/config/module_config.py` & `probable_fiesta-0.1.4/src/probable_fiesta/config/module_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/config/variables.py` & `probable_fiesta-0.1.4/src/probable_fiesta/config/variables.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config.py` & `probable_fiesta-0.1.4/src/probable_fiesta/config/builder/config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/config/builder/config_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/config/builder/config_builder_factory.py` & `probable_fiesta-0.1.4/src/probable_fiesta/config/builder/config_builder_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/logger/logging_config.py` & `probable_fiesta-0.1.4/src/probable_fiesta/logger/logging_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger.py` & `probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,28 +17,32 @@
     def set_up_logger(self, log_name=None, log_level=None, format=None):
         if log_name is None:
             log_name = self.name
         if log_level is None:
             log_level = self.level
         if format is None:
             format = self.fmt
+            if format is None:
+                format = "simple"
 
         self.logger = self.set_logger(log_name, log_level, format)
         return self.logger
 
     def set_logger(self, log_name, log_level, format):
         logger = logging.getLogger(log_name)
 
         if log_level is None:
             log_level = logging.INFO
         else:
             log_level = self.parse_level(log_level)
 
         logger.setLevel(log_level)
 
+        if not format:
+            format = "simple"
         formatter = self.set_formatter_format(format)
 
         path = f"{self.directory}/{log_name}.log"
         # print(f"Using {path} as the log file")
 
         fileh = logging.FileHandler(path, "a")
         fileh.setFormatter(formatter)
```

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_abstract_machine.py` & `probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger_abstract_machine.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_builder.py` & `probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/logger/builder/logger_factory.py` & `probable_fiesta-0.1.4/src/probable_fiesta/logger/builder/logger_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 class LoggerFactory:
     @staticmethod
     def new_logger(name=None, level=None, fmt=None, directory=None):
         return Logger.factory.new_logger(name, level, fmt, directory)
 
     @staticmethod
     def new_logger_get_logger(name=None, level=None, fmt=None, directory=None):
+        if not directory:
+            directory = "logs"
         return Logger.new_get_logger(name, level, fmt, directory)
 
     @staticmethod
     def new_logger_default(name=None, level=None, fmt=None, directory=None):
         if not directory:
             directory = LoggerDef.ROOT_DIR + "/logger"
         if not fmt:
```

### Comparing `probable_fiesta-0.1.3/src/probable_fiesta/run/__init__.py` & `probable_fiesta-0.1.4/src/probable_fiesta/run/__init__.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/templates/hatch.toml` & `probable_fiesta-0.1.4/templates/hatch.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/templates/hatch.toml.j2` & `probable_fiesta-0.1.4/templates/hatch.toml.j2`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/templates/make_skeleton.py` & `probable_fiesta-0.1.4/templates/make_skeleton.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/templates/pyproject.toml` & `probable_fiesta-0.1.4/templates/pyproject.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/templates/pyproject.toml.j2` & `probable_fiesta-0.1.4/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/templates/write_templates.py` & `probable_fiesta-0.1.4/templates/write_templates.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/test_main_app.py` & `probable_fiesta-0.1.4/tests/test_main_app.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/test_v1.py` & `probable_fiesta-0.1.4/tests/test_v1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """Test file for cli/v1.py."""
 from src.probable_fiesta.cli.builder.parser_factory import ParserFactory as PF
 from src.probable_fiesta.logger.builder.logger_factory import LoggerFactory as LF
 
 from unittest import TestCase
 
-LOG = LF.new_logger_get_logger("test_v1", "DEBUG")
+LOG = LF.new_logger_get_logger("test_v1", "DEBUG", directory="logs")
 
 
 class TestCliV1(TestCase):
-
-
     def test_parse_arguments_short_flags(self):
         """Test parsed arguments."""
         # you can also test long flags but it's redundant.
-        #parsed = PF().new_only_args(['--version'])
-        #parsed = self.parser.parser.parse_args(['--version'])
-        #self.assertEqual(parsed.version, True)
+        # parsed = PF().new_only_args(['--version'])
+        # parsed = self.parser.parser.parse_args(['--version'])
+        # self.assertEqual(parsed.version, True)
         ## Add more tests here
 
     def test_parse_arguments_invalid(self):
-        test_arguments = '--unknown invalid'
-        #self.parser.parse_args(test_arguments.split())
-        #parsed = PF().new(test_arguments.split())
-        #expected = f"unrecognized arguments: {test_arguments}"
-        #self.assertEqual(parsed.error_message, expected)
+        test_arguments = "--unknown invalid"
+        # self.parser.parse_args(test_arguments.split())
+        # parsed = PF().new(test_arguments.split())
+        # expected = f"unrecognized arguments: {test_arguments}"
+        # self.assertEqual(parsed.error_message, expected)
 
     def test_parse_arguments_empty(self):
         test_arguments = None
-        #parsed = PF().new(test_arguments)
-        #expected = "invalid empty arguments"
-        #self.assertEqual(parsed, expected)
+        # parsed = PF().new(test_arguments)
+        # expected = "invalid empty arguments"
+        # self.assertEqual(parsed, expected)
```

### Comparing `probable_fiesta-0.1.3/tests/app/builder/test_app_builder.py` & `probable_fiesta-0.1.4/tests/app/builder/test_app_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/cli/builder/test_parser.py` & `probable_fiesta-0.1.4/tests/cli/builder/test_parser.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/command/builder/test_command.py` & `probable_fiesta-0.1.4/tests/command/builder/test_command.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/command/builder/test_command_builder.py` & `probable_fiesta-0.1.4/tests/command/builder/test_command_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/command/builder/test_command_context_factory.py` & `probable_fiesta-0.1.4/tests/command/builder/test_command_context_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/command/builder/test_command_factory.py` & `probable_fiesta-0.1.4/tests/command/builder/test_command_factory.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/command/builder/test_command_queue.py` & `probable_fiesta-0.1.4/tests/command/builder/test_command_queue.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/config/builder/test_config.py` & `probable_fiesta-0.1.4/tests/config/builder/test_config.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/config/builder/test_config_builder.py` & `probable_fiesta-0.1.4/tests/config/builder/test_config_builder.py`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/tests/logger/builder/test_logger.py` & `probable_fiesta-0.1.4/tests/logger/builder/test_logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,80 +1,94 @@
 """Unit test file for logger.builder.logger.py."""
 from src.probable_fiesta.logger.builder import logger
 
 from unittest import TestCase
 
 import os
+
 ROOT_DIR = str(os.path.dirname(os.path.abspath(__file__)).rsplit("/tests")[0])
 
-class TestLogger(TestCase):
 
+class TestLogger(TestCase):
     def setUp(self):
         self.logger = None
 
     def test_init(self):
         self.logger = logger.Logger(None, None, None, None)
 
         self.assertEqual(self.logger.name, None)
         self.assertEqual(self.logger.level, None)
         self.assertEqual(self.logger.fmt, None)
         self.assertEqual(self.logger.directory, None)
         self.assertEqual(self.logger.logger, None)
         self.assertEqual(self.logger.file_handler, None)
 
         # test _str__
-        self.assertEqual(str(self.logger), "Logger: {'name': None, 'level': None, 'fmt': None, 'directory': None, 'logger': None, 'file_handler': None}")
+        self.assertEqual(
+            str(self.logger),
+            "Logger: {'name': None, 'level': None, 'fmt': None, 'directory': None, 'logger': None, 'file_handler': None}",
+        )
 
     def test_new(self):
         log_name = "test_logger"
         log_level = "DEBUG"
-        log_fmt = 'simple'
-        log_directory = ROOT_DIR+'/tests/logs'
+        log_fmt = "simple"
+        log_directory = ROOT_DIR + "/tests/logs"
 
         self.logger = logger.Logger().new(log_name, log_level, log_fmt, log_directory)
 
         self.assertEqual(self.logger.name, log_name)
         self.assertEqual(self.logger.level, log_level)
         self.assertEqual(self.logger.fmt, log_fmt)
         self.assertEqual(self.logger.directory, log_directory)
         self.assertEqual(self.logger.logger, None)
         self.assertEqual(self.logger.file_handler, None)
 
     def test_set_logger(self):
         self.logger = logger.Logger()
-        self.logger.set_logger("MY_MOCK_CLASS")
-        self.assertEqual(self.logger.logger, "MY_MOCK_CLASS")
+        self.logger.directory = "logs"
+        self.logger = self.logger.set_logger("MY_MOCK_CLASS", "INFO", "simple")
+        self.assertEqual(self.logger.name, "MY_MOCK_CLASS")
+        self.assertEqual(self.logger.level, 20)
 
     def test_get_logger(self):
         log_name = "test_logger"
         log_level = "DEBUG"
-        log_fmt = 'simple'
-        log_directory = ROOT_DIR+'/tests/logs'
+        log_fmt = "simple"
+        log_directory = ROOT_DIR + "/tests/logs"
         self.logger = logger.Logger().new(log_name, log_level, log_fmt, log_directory)
         parsed_logger = self.logger.get_logger()
         self.assertEqual(str(parsed_logger.__class__), "<class 'logging.Logger'>")
 
     def test_new_get_logger(self):
         log_name = "test_logger"
         log_level = "DEBUG"
-        log_fmt = 'simple'
-        log_directory = ROOT_DIR+'/tests/logs'
-        self.logger = logger.Logger().new_get_logger(log_name, log_level, log_fmt, log_directory)
+        log_fmt = "simple"
+        log_directory = ROOT_DIR + "/tests/logs"
+        self.logger = logger.Logger().new_get_logger(
+            log_name, log_level, log_fmt, log_directory
+        )
         self.assertEqual(str(self.logger.__class__), "<class 'logging.Logger'>")
 
     def test_factory_new(self):
         log_name = "test_logger"
         log_level = "DEBUG"
-        log_fmt = 'simple'
-        log_directory = ROOT_DIR+'/tests/logs'
-        self.logger = logger.Logger().Factory.new_logger(log_name, log_level, log_fmt, log_directory)
+        log_fmt = "simple"
+        log_directory = ROOT_DIR + "/tests/logs"
+        self.logger = logger.Logger().Factory.new_logger(
+            log_name, log_level, log_fmt, log_directory
+        )
         self.assertEqual(str(self.logger.name), "test_logger")
 
     def test_factory_create_file_handler(self):
         log_name = "test_logger"
         log_level = "DEBUG"
-        log_fmt = 'simple'
-        log_directory = ROOT_DIR+'/tests/logs'
-        self.logger = logger.Logger().Factory.new_logger(log_name, log_level, log_fmt, log_directory)
+        log_fmt = "simple"
+        log_directory = ROOT_DIR + "/tests/logs"
+        self.logger = logger.Logger().Factory.new_logger(
+            log_name, log_level, log_fmt, log_directory
+        )
         file_handler = self.logger.create_file_handler()
-        factory_file_handler = logger.Logger().Factory.new_file_handler(log_name, log_level, log_fmt, log_directory)
-        self.assertEqual(file_handler.name, factory_file_handler.name)
+        factory_file_handler = logger.Logger().Factory.new_file_handler(
+            log_name, log_level, log_fmt, log_directory
+        )
+        self.assertEqual(file_handler.name, factory_file_handler.name)
```

### Comparing `probable_fiesta-0.1.3/.gitignore` & `probable_fiesta-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/LICENSE` & `probable_fiesta-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/README.md` & `probable_fiesta-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/hatch.toml` & `probable_fiesta-0.1.4/hatch.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/pyproject.toml` & `probable_fiesta-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `probable_fiesta-0.1.3/PKG-INFO` & `probable_fiesta-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probable_fiesta
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python Core Package.
 Project-URL: Homepage, https://github.com/sergio-munoz/probable_fiesta/
 Project-URL: Bug Tracker, https://github.com/sergio-munoz/probable_fiesta/issues
 Project-URL: Documentation, https://github.com/sergio-munoz/probable_fiesta#readme
 Project-URL: Issues, https://github.com/sergio-munoz/probable_fiesta/issues
 Project-URL: Source, https://github.com/sergio-munoz/probable_fiesta
 Author-email: Sergio Munoz <sergio.munoz@pubnub.com>
```

