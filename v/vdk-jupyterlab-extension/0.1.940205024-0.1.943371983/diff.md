# Comparing `tmp/vdk_jupyterlab_extension-0.1.940205024.tar.gz` & `tmp/vdk_jupyterlab_extension-0.1.943371983.tar.gz`

## Comparing `vdk_jupyterlab_extension-0.1.940205024.tar` & `vdk_jupyterlab_extension-0.1.943371983.tar`

### file list

```diff
@@ -1,80 +1,90 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.eslintignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.eslintrc.js
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.stylelintrc
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/babel.config.js
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/conftest.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/install.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/jest.config.js
--rw-r--r--   0        0        0  1169752 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/package-lock.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/package.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/tsconfig.json
--rw-r--r--   0        0        0   423537 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/yarn.lock
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/jupyter-config/nb-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/jupyter-config/server-config/vdk-jupyterlab-extension.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/schema/plugin.json
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/commandsAndMenu.tsx
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/handler.ts
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/index.ts
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/initVDKConfigCell.ts
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/jobData.ts
--rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/serverRequests.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/utils.ts
--rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/vdkTags.ts
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/convert-job-to-notebook-component.spec.ts
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/create-job-component.spec.ts
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/deploy-job-component.spec.ts
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/download-job-component.spec.ts
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/handler.spec.ts
--rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/resquests.spec.ts
--rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/run-job-component.spec.tsx
--rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/show-dialog.spec.tsx
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-error-message.spec.ts
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-tags.spec.ts
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/ConvertJobToNotebook.tsx
--rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/CreateJob.tsx
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/DeployJob.tsx
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/DownloadJob.tsx
--rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/RunJob.tsx
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/VdkErrorMessage.ts
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/VdkTextInput.tsx
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/components/props.tsx
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/src/vdkOptions/vdk_options.ts
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/base.css
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/index.css
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/index.js
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/vdkDialogs.css
--rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/style/images/versatile-data-kit-logo.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/package.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/playwright.config.js
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/handlers.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/job_data.py
--rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_ui.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/README.md
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
--rw-r--r--   0        0        0    16736 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/161.d4f50a459898d1a8bc76.js
--rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/remoteEntry.3b6333fd6a058bff7cf9.js
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/tests/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/tests/test_handlers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_options/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_options/vdk_options.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/.gitignore
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/LICENSE
--rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/README.md
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/pyproject.toml
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.940205024/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.eslintignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.eslintrc.js
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.stylelintrc
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/babel.config.js
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/conftest.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/install.json
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/jest.config.js
+-rw-r--r--   0        0        0   637348 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/package-lock.json
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/package.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/tsconfig.json
+-rw-r--r--   0        0        0   424494 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/yarn.lock
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/jupyter-config/nb-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/jupyter-config/server-config/vdk-jupyterlab-extension.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/schema/plugin.json
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/commandsAndMenu.tsx
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/handler.ts
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/index.ts
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/initVDKConfigCell.ts
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/jobData.ts
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/serverRequests.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/utils.ts
+-rw-r--r--   0        0        0     4303 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/vdkTags.ts
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/convert-job-to-notebook-component.spec.ts
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/create-job-component.spec.ts
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/deploy-job-component.spec.ts
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/download-job-component.spec.ts
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/handler.spec.ts
+-rw-r--r--   0        0        0     5475 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/resquests.spec.ts
+-rw-r--r--   0        0        0     6323 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/run-job-component.spec.tsx
+-rw-r--r--   0        0        0     6907 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/show-dialog.spec.tsx
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-error-message.spec.ts
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-tags.spec.ts
+-rw-r--r--   0        0        0    12078 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/ConvertJobToNotebook.tsx
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/CreateJob.tsx
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/DeployJob.tsx
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/DownloadJob.tsx
+-rw-r--r--   0        0        0     7861 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/RunJob.tsx
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/VdkErrorMessage.ts
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/VdkTextInput.tsx
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/components/props.tsx
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/src/vdkOptions/vdk_options.ts
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/base.css
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/index.css
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/index.js
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/vdkDialogs.css
+-rw-r--r--   0        0        0     7626 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/style/images/versatile-data-kit-logo.svg
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/testutils/jest-file-mock.js
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/package.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7410 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/convert-job.spec.ts
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/utils.ts
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/vdk-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/10_drop_table.sql
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/20_create_table.sql
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/data/convert-test-job-dirty/30_ingest_to_table.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/convert_job.py
+-rw-r--r--   0        0        0     8109 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/handlers.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/job_data.py
+-rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_ui.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/README.md
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/config.ini
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/requirements.txt
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json
+-rw-r--r--   0        0        0    21604 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/161.58979db168f482d72ccd.js
+-rw-r--r--   0        0        0     5454 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js
+-rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/remoteEntry.f9166f3ab54776548603.js
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/__init__.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_convert_job_directory_processor.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_directory_archiver.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/tests/test_handlers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_options/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_options/vdk_options.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/.gitignore
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/LICENSE
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/README.md
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/pyproject.toml
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 vdk_jupyterlab_extension-0.1.943371983/PKG-INFO
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/.eslintrc.js` & `vdk_jupyterlab_extension-0.1.943371983/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/jest.config.js` & `vdk_jupyterlab_extension-0.1.943371983/jest.config.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -2,39 +2,39 @@
  * Copyright 2021-2023 VMware, Inc.
  * SPDX-License-Identifier: Apache-2.0
  */
 
 const jestJupyterLab = require('@jupyterlab/testutils/lib/jest-config');
 
 const esModules = [
-    '@jupyterlab/',
+    '.*@jupyterlab/',
+    '@jupyter/ydoc',
     'lib0',
     'y\\-protocols',
     'y\\-websocket',
     'yjs'
 ].join('|');
 
 const jlabConfig = jestJupyterLab(__dirname);
 
 const {
     moduleFileExtensions,
     moduleNameMapper,
     preset,
     setupFilesAfterEnv,
-    setupFiles,
     testPathIgnorePatterns,
     transform
 } = jlabConfig;
 
 module.exports = {
     moduleFileExtensions,
     moduleNameMapper,
     preset,
     setupFilesAfterEnv,
-    setupFiles,
+    setupFiles: ['<rootDir>/testutils/jest-setup-files.js'],
     testPathIgnorePatterns,
     transform,
     automock: false,
     testEnvironment: 'jsdom',
     collectCoverageFrom: [
         'src/**/*.{ts,tsx}',
         '!src/**/*.d.ts',
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/package.json` & `vdk_jupyterlab_extension-0.1.943371983/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9762845849802372%*

 * *Differences: {"'devDependencies'": "{'jest-fetch-mock': '^3.0.0'}", "'version'": "'0.1.943371983'"}*

```diff
@@ -46,14 +46,15 @@
         "@typescript-eslint/eslint-plugin": "4.8.1",
         "@typescript-eslint/parser": "4.8.1",
         "babel-jest": "27.5.1",
         "eslint": "7.14.0",
         "eslint-config-prettier": "6.15.0",
         "eslint-plugin-prettier": "3.1.4",
         "jest": "27.0.6",
+        "jest-fetch-mock": "^3.0.0",
         "mkdirp": "1.0.3",
         "npm-run-all": "4.1.5",
         "prettier": "2.1.1",
         "rimraf": "3.0.2",
         "stylelint": "14.3.0",
         "stylelint-config-prettier": "9.0.4",
         "stylelint-config-recommended": "6.0.0",
@@ -145,9 +146,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.940205024"
+    "version": "0.1.943371983"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/tsconfig.json` & `vdk_jupyterlab_extension-0.1.943371983/tsconfig.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/yarn.lock` & `vdk_jupyterlab_extension-0.1.943371983/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2458,17 +2458,17 @@
 
 "@types/minimist@^1.2.0":
   version "1.2.2"
   resolved "https://registry.yarnpkg.com/@types/minimist/-/minimist-1.2.2.tgz#ee771e2ba4b3dc5b372935d549fd9617bf345b8c"
   integrity sha512-jhuKLIRrhvCPLqwPcx6INqmKeiA5EWrsCOPhrlFSrbrmU4ZMPjj5Ul/oLCMDO98XRUIwVm78xICz4EPCektzeQ==
 
 "@types/node@*":
-  version "20.4.2"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.2.tgz#129cc9ae69f93824f92fac653eebfb4812ab4af9"
-  integrity sha512-Dd0BYtWgnWJKwO1jkmTrzofjK2QXXcai0dmtzvIBhcA+RsG5h8R3xlyta0kGOZRNfL9GuRtb1knmPEhQrePCEw==
+  version "20.4.4"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.4.4.tgz#c79c7cc22c9d0e97a7944954c9e663bcbd92b0cb"
+  integrity sha512-CukZhumInROvLq3+b5gLev+vgpsIqC2D0deQr/yS1WnxvmYLlJXZpaQrQiseMY+6xusl79E04UjWoqyr+t1/Ew==
 
 "@types/normalize-package-data@^2.4.0":
   version "2.4.1"
   resolved "https://registry.yarnpkg.com/@types/normalize-package-data/-/normalize-package-data-2.4.1.tgz#d3357479a0fdfdd5907fe67e17e0a85c906e1301"
   integrity sha512-Gj7cI7z+98M282Tqmp2K5EIsoouUEzbBJhQQzDE3jSIRk6r9gsz0oUokqIUR4u1R3dMHo0pDHM7sNOHyhulypw==
 
 "@types/parse-json@^4.0.0":
@@ -3582,14 +3582,21 @@
   dependencies:
     "@types/parse-json" "^4.0.0"
     import-fresh "^3.2.1"
     parse-json "^5.0.0"
     path-type "^4.0.0"
     yaml "^1.10.0"
 
+cross-fetch@^3.0.4:
+  version "3.1.8"
+  resolved "https://registry.yarnpkg.com/cross-fetch/-/cross-fetch-3.1.8.tgz#0327eba65fd68a7d119f8fb2bf9334a1a7956f82"
+  integrity sha512-cvA+JwZoU0Xq+h6WkMvAUqPEYy92Obet6UdKLfW60qn99ftItKjB5T+BkyWOFWe2pUyfQ+IJHmpOTznqk1M6Kg==
+  dependencies:
+    node-fetch "^2.6.12"
+
 cross-spawn@^6.0.0, cross-spawn@^6.0.5:
   version "6.0.5"
   resolved "https://registry.yarnpkg.com/cross-spawn/-/cross-spawn-6.0.5.tgz#4a5ec7c64dfae22c3a14124dbacdee846d80cbc4"
   integrity sha512-eTVLrBSt7fjbDygz805pMnstIs2VTBNkRm0qxZd+M7A5XDdxVRWO5MxGBXZhjY4cqLYLdtrGqRf8mBPmzwSpWQ==
   dependencies:
     nice-try "^1.0.4"
     path-key "^2.0.1"
@@ -3889,17 +3896,17 @@
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
 electron-to-chromium@^1.4.431:
-  version "1.4.467"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.467.tgz#b0660bf644baff7eedea33b8c742fb53ec60e3c2"
-  integrity sha512-2qI70O+rR4poYeF2grcuS/bCps5KJh6y1jtZMDDEteyKJQrzLOEhFyXCLcHW6DTBjKjWkk26JhWoAi+Ux9A0fg==
+  version "1.4.468"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.468.tgz#3cbf64ad67d9f12bfe69fefe5eb1935ec4f6ab7a"
+  integrity sha512-6M1qyhaJOt7rQtNti1lBA0GwclPH+oKCmsra/hkcWs5INLxfXXD/dtdnaKUYQu/pjOBP/8Osoe4mAcNvvzoFag==
 
 emittery@^0.7.1:
   version "0.7.2"
   resolved "https://registry.yarnpkg.com/emittery/-/emittery-0.7.2.tgz#25595908e13af0f5674ab419396e2fb394cdfa82"
   integrity sha512-A8OG5SR/ij3SsJdWDJdkkSYUjQdCUx6APQXem0SaEePBSRg4eymGYwBkKo1Y6DU+af/Jn2dBQqDBvjnr9Vi8nQ==
 
 emittery@^0.8.1:
@@ -4366,17 +4373,17 @@
 
 fast-diff@^1.1.2:
   version "1.3.0"
   resolved "https://registry.yarnpkg.com/fast-diff/-/fast-diff-1.3.0.tgz#ece407fa550a64d638536cd727e129c61616e0f0"
   integrity sha512-VxPP4NqbUjj6MaAOafWeUn2cXWLcCtljklUtZf0Ind4XQ+QPtmA0b18zZy0jIQx+ExRVCR/ZQpBmik5lXshNsw==
 
 fast-glob@^3.2.11, fast-glob@^3.2.9:
-  version "3.3.0"
-  resolved "https://registry.yarnpkg.com/fast-glob/-/fast-glob-3.3.0.tgz#7c40cb491e1e2ed5664749e87bfb516dbe8727c0"
-  integrity sha512-ChDuvbOypPuNjO8yIDf36x7BlZX1smcUMTTcyoIjycexOxd6DFsKsg21qVBzEmr3G7fUKIRy2/psii+CIUt7FA==
+  version "3.3.1"
+  resolved "https://registry.yarnpkg.com/fast-glob/-/fast-glob-3.3.1.tgz#784b4e897340f3dbbef17413b3f11acf03c874c4"
+  integrity sha512-kNFPyjhh5cKjrUltxs+wFx+ZkbRaxxmZ+X0ZU31SOsxCEtP9VPgtq2teZw1DebupL5GmDaNQ6yKMMVcM41iqDg==
   dependencies:
     "@nodelib/fs.stat" "^2.0.2"
     "@nodelib/fs.walk" "^1.2.3"
     glob-parent "^5.1.2"
     merge2 "^1.3.0"
     micromatch "^4.0.4"
 
@@ -5689,14 +5696,22 @@
     "@jest/environment" "^27.5.1"
     "@jest/fake-timers" "^27.5.1"
     "@jest/types" "^27.5.1"
     "@types/node" "*"
     jest-mock "^27.5.1"
     jest-util "^27.5.1"
 
+jest-fetch-mock@^3.0.0:
+  version "3.0.3"
+  resolved "https://registry.yarnpkg.com/jest-fetch-mock/-/jest-fetch-mock-3.0.3.tgz#31749c456ae27b8919d69824f1c2bd85fe0a1f3b"
+  integrity sha512-Ux1nWprtLrdrH4XwE7O7InRY6psIi3GOsqNESJgMJ+M5cv4A8Lh7SN9d2V2kKRZ8ebAfcd1LNyZguAOb6JiDqw==
+  dependencies:
+    cross-fetch "^3.0.4"
+    promise-polyfill "^8.1.3"
+
 jest-get-type@^26.3.0:
   version "26.3.0"
   resolved "https://registry.yarnpkg.com/jest-get-type/-/jest-get-type-26.3.0.tgz#e97dc3c3f53c2b406ca7afaed4493b1d099199e0"
   integrity sha512-TpfaviN1R2pQWkIihlfEanwOXK0zcxrKEE4MlU6Tn7keoXdN6/3gK/xl0yEh8DOunn5pOVGKf8hB4R9gVh04ig==
 
 jest-get-type@^27.5.1:
   version "27.5.1"
@@ -6941,15 +6956,15 @@
 no-case@^2.2.0:
   version "2.3.2"
   resolved "https://registry.yarnpkg.com/no-case/-/no-case-2.3.2.tgz#60b813396be39b3f1288a4c1ed5d1e7d28b464ac"
   integrity sha512-rmTZ9kz+f3rCvK2TD1Ue/oZlns7OGoIWP4fc3llxxRXlOkHKoWPPWJOfFYpITabSow43QJbRIoHQXtt10VldyQ==
   dependencies:
     lower-case "^1.1.1"
 
-node-fetch@^2.6.0:
+node-fetch@^2.6.0, node-fetch@^2.6.12:
   version "2.6.12"
   resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.6.12.tgz#02eb8e22074018e3d5a83016649d04df0e348fba"
   integrity sha512-C/fGU2E8ToujUivIO0H+tpQ6HWo4eEmchoPIoXtxCrVghxdKq+QOHqEZW7tuP3KlV3bC8FRMO5nMCC7Zm1VP6g==
   dependencies:
     whatwg-url "^5.0.0"
 
 node-gyp-build@~4.1.0:
@@ -7428,14 +7443,19 @@
   integrity sha512-7PiHtLll5LdnKIMw100I+8xJXR5gW2QwWYkT6iJva0bXitZKa/XMrSbdmg3r2Xnaidz9Qumd0VPaMrZlF9V9sA==
 
 promise-inflight@^1.0.1:
   version "1.0.1"
   resolved "https://registry.yarnpkg.com/promise-inflight/-/promise-inflight-1.0.1.tgz#98472870bf228132fcbdd868129bad12c3c029e3"
   integrity sha512-6zWPyEOFaQBJYcGMHBKTKJ3u6TBsnMFOIZSa6ce1e/ZrrsOlnHRHbabMjLiBYKp+n44X9eUI6VUPaukCXHuG4g==
 
+promise-polyfill@^8.1.3:
+  version "8.3.0"
+  resolved "https://registry.yarnpkg.com/promise-polyfill/-/promise-polyfill-8.3.0.tgz#9284810268138d103807b11f4e23d5e945a4db63"
+  integrity sha512-H5oELycFml5yto/atYqmjyigJoAo3+OXwolYiH7OfQuYlAqhxNvTfiNMbV9hsC6Yp83yE5r2KTVmtrG6R9i6Pg==
+
 prompts@^2.0.1:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/prompts/-/prompts-2.4.2.tgz#7b57e73b3a48029ad10ebd44f74b01722a4cb069"
   integrity sha512-NxNv/kLguCA7p3jE8oL2aEBsrJWgAakBpgmgK6lpPWV+WuOmY6r2/zbAVnP+T8bQlA0nzHXSJSJW0Hq7ylaD2Q==
   dependencies:
     kleur "^3.0.3"
     sisteransi "^1.0.5"
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/schema/plugin.json` & `vdk_jupyterlab_extension-0.1.943371983/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/commandsAndMenu.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/commandsAndMenu.tsx`

 * *Files 24% similar despite different names*

```diff
@@ -6,56 +6,62 @@
 import { showCreateJobDialog } from './components/CreateJob';
 import { showDownloadJobDialog } from './components/DownloadJob';
 import { showConvertJobToNotebookDialog } from './components/ConvertJobToNotebook';
 import { jobdDataRequest } from './serverRequests';
 import { VdkOption } from './vdkOptions/vdk_options';
 import { workingDirectory } from '.';
 import { IDocumentManager } from '@jupyterlab/docmanager';
+import { FileBrowser } from '@jupyterlab/filebrowser';
+import { INotebookTracker } from '@jupyterlab/notebook';
 
-var runningVdkOperation = false;
+export var runningVdkOperation = '';
 
-export function updateVDKMenu(commands: CommandRegistry, docManager: IDocumentManager) {
+export function updateVDKMenu(commands: CommandRegistry, docManager: IDocumentManager, fileBrowser: FileBrowser, notebookTracker: INotebookTracker) {
   // Add Run job command
-  add_command(commands, 'jp-vdk:menu-run','Run','Execute VDK Run Command', showRunJobDialog, docManager);
+  add_command(commands, 'jp-vdk:menu-run', 'Run', 'Execute VDK Run Command', showRunJobDialog, docManager);
 
   // Add Create job command
-  add_command(commands, 'jp-vdk:menu-create','Create','Execute VDK Create Command', showCreateJobDialog);
+  add_command(commands, 'jp-vdk:menu-create', 'Create', 'Execute VDK Create Command', showCreateJobDialog);
 
   // Add Download job command
-  add_command(commands, 'jp-vdk:menu-download','Download','Execute VDK Download Command', showDownloadJobDialog);
+  add_command(commands, 'jp-vdk:menu-download', 'Download', 'Execute VDK Download Command', showDownloadJobDialog);
 
   // Add Convert Job To Notebook command
-  add_command(commands, 'jp-vdk:menu-convert-job-to-notebook', 'Convert Job To Notebook', 'Convert Data Job To Jupyter Notebook', showConvertJobToNotebookDialog);
+  add_command(commands, 'jp-vdk:menu-convert-job-to-notebook', 'Convert Job To Notebook', 'Convert Data Job To Jupyter Notebook', showConvertJobToNotebookDialog, undefined,
+    fileBrowser, notebookTracker);
 
   // Add Create Deployment command
-  add_command(commands, 'jp-vdk:menu-create-deployment','Deploy','Create deployment of a VDK job', showCreateDeploymentDialog);
+  add_command(commands, 'jp-vdk:menu-create-deployment', 'Deploy', 'Create deployment of a VDK job', showCreateDeploymentDialog);
 }
 
 
 /**
  *@param schemaNaming - string representing the command in the schema in schema/plugin.json
  *@param label - the label that will be added in the Menu
  *@param caption - the caption for the command.
  *@param getOperationDialog - function that will load the dialog for the command
  */
 function add_command(commands: CommandRegistry, schemaNaming: string, label: string, caption: string, getOperationDialog: Function,
-  docManager?: IDocumentManager){
+  docManager?: IDocumentManager, fileBrowser?: FileBrowser, notebookTracker?: INotebookTracker) {
   commands.addCommand(schemaNaming, {
     label: label,
     caption: caption,
     execute: async () => {
       try {
         if (!runningVdkOperation) {
-          runningVdkOperation = true;
+          runningVdkOperation = schemaNaming;
           jobData.set(VdkOption.PATH, workingDirectory);
           await jobdDataRequest();
-          if(docManager) await getOperationDialog(docManager);
-          else  await getOperationDialog();
+          if (label == 'Convert Job To Notebook') await getOperationDialog(commands, fileBrowser, notebookTracker);
+          else if (docManager) {
+            await getOperationDialog(docManager);
+          }
+          else await getOperationDialog();
           setJobDataToDefault();
-          runningVdkOperation = false;
+          runningVdkOperation = '';
         } else {
           showErrorMessage(
             'Another VDK operation is currently running!',
             'Please wait until the operation ends!',
             [Dialog.okButton()]
           );
         }
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/handler.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/handler.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/index.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/index.ts`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
-import { updateVDKMenu } from './commandsAndMenu';
+import { runningVdkOperation, updateVDKMenu } from './commandsAndMenu';
 
 import { FileBrowserModel, IFileBrowserFactory } from '@jupyterlab/filebrowser';
 import { IChangedArgs } from '@jupyterlab/coreutils';
 import { INotebookTracker } from '@jupyterlab/notebook';
 import { trackVdkTags } from './vdkTags';
 import { IThemeManager } from '@jupyterlab/apputils';
 import { IDocumentManager } from '@jupyterlab/docmanager';
 import { initVDKConfigCell } from './initVDKConfigCell';
+import { populateNotebook } from './components/ConvertJobToNotebook';
 
 /**
  * Current working directory in Jupyter
  * The variable can be accessed anywhere in the JupyterFrontEndPlugin
  */
 export let workingDirectory: string = '';
 
@@ -44,21 +45,28 @@
     factory: IFileBrowserFactory,
     notebookTracker: INotebookTracker,
     themeManager: IThemeManager,
     docManager: IDocumentManager
   ) => {
     const { commands } = app;
 
-    updateVDKMenu(commands, docManager);
-
     notebookTracker.activeCellChanged.connect((sender, args) => {
-      initVDKConfigCell(notebookTracker);
+      if (runningVdkOperation !== 'jp-vdk:menu-convert-job-to-notebook') {
+        initVDKConfigCell(notebookTracker);
+      } else {
+        //  * Populates notebook with provided content for convert job operation
+        //  * Check src/components/ConvertJobToNotebook.tsx for more
+        populateNotebook(notebookTracker);
+      }
     });
 
     const fileBrowser = factory.defaultBrowser;
+
+    updateVDKMenu(commands, docManager, fileBrowser, notebookTracker);
+
     fileBrowser.model.pathChanged.connect(onPathChanged);
     trackVdkTags(notebookTracker, themeManager);
   }
 };
 
 export default plugin;
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/initVDKConfigCell.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/initVDKConfigCell.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/jobData.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/jobData.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/serverRequests.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/serverRequests.ts`

 * *Files 12% similar despite different names*

```diff
@@ -87,34 +87,52 @@
       }
     } catch (error) {
       showError(error);
     }
   }
 }
 
+/**
+ * Sends a POST request to the server to perform a 'transform job to notebook' operation.
+ * This function prepares the job data and makes the request.
+ *
+ * Upon success, the server returns an object containing:
+ * - message: A string that includes the 'codeStructure' and 'filenames' os the steps of the transformed job.
+ * - status: A boolean indicating the operation's success. It's '' when no errors occurred during the operation.
+ *
+ * Upon failure (either server-side or client-side), the function returns an object
+ * with an error message and 'false' status.
+ * Any error that occurred during the operation is also shown to the user.
+ *
+ * @returns A Promise that resolves to an object containing the message from the server and the status of the operation.
+ */
 export async function jobConvertToNotebookRequest(): Promise<{
-  message: String;
+  message: string;
   status: boolean;
 }> {
   if (await checkIfVdkOptionDataIsDefined(VdkOption.PATH)) {
     try {
       const data = await requestAPI<serverVdkOperationResult>(
         'convertJobToNotebook',
         {
           body: JSON.stringify(getJobDataJsonObject()),
           method: 'POST'
         }
       );
-      return { message: data['message'], status: data['message'] == '0' };
+      return { message: data['message'], status: data['error'] == '' };
     } catch (error) {
       showError(error);
       return { message: '', status: false };
     }
   } else {
-    return { message: '', status: false };
+    return {
+      message:
+        'The job path is not defined. Please define it before attempting to convert the job to a notebook.',
+      status: false
+    };
   }
 }
 
 /**
  * Sent a POST request to the server to get information about the data job of current directory
  */
 export async function jobdDataRequest(): Promise<void> {
@@ -191,7 +209,23 @@
     });
     return data;
   } catch (error) {
     showError(error);
   }
   return [];
 }
+
+export async function getServerDirRequest(): Promise<string> {
+  const data = await requestAPI<any>('serverPath', {
+    method: 'GET'
+  });
+  if (data) {
+    return data;
+  } else {
+    await showErrorMessage(
+      "Encountered an error while trying to connect the server. Error: \
+      the server's location cannot be identified!",
+      [Dialog.okButton()]
+    );
+    return '';
+  }
+}
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/vdkTags.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/vdkTags.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/create-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/create-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/deploy-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/deploy-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/download-job-component.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/download-job-component.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/handler.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/handler.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/resquests.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/resquests.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/run-job-component.spec.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/run-job-component.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/show-dialog.spec.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/show-dialog.spec.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-error-message.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-error-message.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/__tests__/vdk-tags.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/__tests__/vdk-tags.spec.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/components/ConvertJobToNotebook.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/components/CreateJob.tsx`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,126 @@
 import React, { Component } from 'react';
 import { jobData } from '../jobData';
 import { VdkOption } from '../vdkOptions/vdk_options';
 import VDKTextInput from './VdkTextInput';
 import { Dialog, showDialog } from '@jupyterlab/apputils';
-import { jobConvertToNotebookRequest } from '../serverRequests';
-import { IJobPathProp } from './props';
-import { VdkErrorMessage } from './VdkErrorMessage';
-import { CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL } from '../utils';
+import { jobRequest } from '../serverRequests';
+import { IJobFullProps } from './props';
+import { CREATE_JOB_BUTTON_LABEL } from '../utils';
 
-export default class ConvertJobToNotebookDialog extends Component<IJobPathProp> {
+export default class CreateJobDialog extends Component<(IJobFullProps)> {
   /**
-   * Returns a React component for rendering a convert menu.
+   * Returns a React component for rendering a create menu.
    *
    * @param props - component properties
    * @returns React component
    */
-  constructor(props: IJobPathProp) {
+  constructor(props: IJobFullProps) {
     super(props);
   }
   /**
-   * Renders a dialog for converting a data job.
+   * Renders a dialog for creating a data job.
    *
    * @returns React element
    */
   render(): React.ReactElement {
     return (
       <>
+        <div className="jp-vdk-checkbox-wrappers">
+          <div>
+            <input
+              type="checkbox"
+              name="Local"
+              id="Local"
+              className="jp-vdk-checkbox"
+              onClick={this._onLocalClick()}
+            />
+            <label className="checkboxLabel" htmlFor="Local">
+              Local
+            </label>
+          </div>
+          <div>
+            <input
+              type="checkbox"
+              name="Cloud"
+              id="Cloud"
+              className="jp-vdk-checkbox"
+              onClick={this._onCloudClick()}
+            />
+            <label className="checkboxLabel" htmlFor="Cloud">
+              Cloud
+            </label>
+          </div>
+        </div>
+        <VDKTextInput
+          option={VdkOption.NAME}
+          value={this.props.jobName}
+          label="Job Name:"
+        ></VDKTextInput>
+        <VDKTextInput
+          option={VdkOption.TEAM}
+          value={this.props.jobTeam}
+          label="Job Team:"
+        ></VDKTextInput>
         <VDKTextInput
           option={VdkOption.PATH}
           value={this.props.jobPath}
           label="Path to job directory:"
         ></VDKTextInput>
       </>
     );
   }
+  /**
+   * Callback invoked upon choosing local checkbox
+   */
+  private _onLocalClick() {
+    return (event: React.MouseEvent) => {
+      this.setJobFlags('Local');
+    };
+  }
+  /**
+   * Callback invoked upon choosing cloud checkbox
+   */
+  private _onCloudClick() {
+    return (event: React.MouseEvent) => {
+      this.setJobFlags('Cloud');
+    };
+  }
+  /**
+   * Function that sets job's cloud/local flags
+   */
+  private setJobFlags(flag: string) {
+    let checkbox = document.getElementById(flag);
+    if (checkbox?.classList.contains('checked')) {
+      checkbox.classList.remove('checked');
+      if (flag === 'Cloud') {
+        jobData.set(VdkOption.CLOUD, '');
+      } else {
+        jobData.set(VdkOption.LOCAL, '');
+      }
+    } else {
+      checkbox?.classList.add('checked');
+      if (flag === 'Cloud') {
+        jobData.set(VdkOption.CLOUD, '1');
+      } else {
+        jobData.set(VdkOption.LOCAL, '1');
+      }
+    }
+  }
 }
 
-export async function showConvertJobToNotebookDialog() {
+export async function showCreateJobDialog() {
   const result = await showDialog({
-    title: CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL,
+    title: CREATE_JOB_BUTTON_LABEL,
     body: (
-      <ConvertJobToNotebookDialog
+      <CreateJobDialog
         jobPath={jobData.get(VdkOption.PATH)!}
-      ></ConvertJobToNotebookDialog>
+        jobName={jobData.get(VdkOption.NAME)!}
+        jobTeam={jobData.get(VdkOption.TEAM)!}
+      ></CreateJobDialog>
     ),
     buttons: [Dialog.okButton(), Dialog.cancelButton()]
   });
   if (result.button.accept) {
-    const confirmation = await showDialog({
-      title: CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL,
-      body: (
-        <p>
-          Are you sure you want to convert the Data Job with path:{' '}
-          <i>{jobData.get(VdkOption.PATH)}</i> to notebook?
-        </p>
-      ),
-      buttons: [Dialog.okButton(), Dialog.cancelButton()]
-    });
-    if (confirmation.button.accept) {
-      let { message, status } = await jobConvertToNotebookRequest();
-      if (status) {
-        await showDialog({
-          title: CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL,
-          body: (
-            <div className="vdk-convert-to-notebook-dialog-message-container">
-              <p className="vdk-convert-to-notebook-dialog-message">
-                The Data Job with path <i>{jobData.get(VdkOption.PATH)}</i> was
-                converted to notebook successfully!
-              </p>
-            </div>
-          ),
-          buttons: [Dialog.okButton()]
-        });
-      } else {
-        message = 'ERROR : ' + message;
-        const errorMessage = new VdkErrorMessage(message);
-        await showDialog({
-          title: CONVERT_JOB_TO_NOTEBOOK_BUTTON_LABEL,
-          body: (
-            <div className="vdk-convert-to-notebook-error-message ">
-              <p>{errorMessage.exception_message}</p>
-              <p>{errorMessage.what_happened}</p>
-              <p>{errorMessage.why_it_happened}</p>
-              <p>{errorMessage.consequences}</p>
-              <p>{errorMessage.countermeasures}</p>
-            </div>
-          ),
-          buttons: [Dialog.okButton()]
-        });
-      }
-    }
+    await jobRequest('create');
   }
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/components/DeployJob.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/components/DeployJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/components/DownloadJob.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/components/DownloadJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/components/RunJob.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/components/RunJob.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/components/VdkErrorMessage.ts` & `vdk_jupyterlab_extension-0.1.943371983/src/components/VdkErrorMessage.ts`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/src/components/VdkTextInput.tsx` & `vdk_jupyterlab_extension-0.1.943371983/src/components/VdkTextInput.tsx`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/style/base.css` & `vdk_jupyterlab_extension-0.1.943371983/style/base.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/style/vdkDialogs.css` & `vdk_jupyterlab_extension-0.1.943371983/style/vdkDialogs.css`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/style/images/versatile-data-kit-logo.svg` & `vdk_jupyterlab_extension-0.1.943371983/style/images/versatile-data-kit-logo.svg`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/ui-tests/README.md` & `vdk_jupyterlab_extension-0.1.943371983/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/ui-tests/jupyter_server_test_config.py` & `vdk_jupyterlab_extension-0.1.943371983/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/ui-tests/tests/vdk-jupyterlab-extension.spec.ts` & `vdk_jupyterlab_extension-0.1.943371983/ui-tests/tests/vdk-jupyterlab-extension.spec.ts`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 test('should try to run a job with incorrect data and get a dialog error message', async ({
   page
 }) => {
   await page.goto('');
   await page.menu.open('VDK');
   await page.locator('#jp-vdk-menu').getByText('Run').click();
-  await page.getByLabel('Path to parent directory:').click();
-  await page.getByLabel('Path to parent directory:').fill('/my-folder');
+  await page.getByLabel('Path to job directory:').click();
+  await page.getByLabel('Path to job directory:').fill('/my-folder');
   await page.getByRole('button', { name: 'OK' }).click();
   page.once('dialog', async dialog => {
     console.log(`Dialog message: ${dialog.message()}`);
     dialog.dismiss().catch(() => {});
   });
 });
 
@@ -82,16 +82,16 @@
   await page.menu.open('VDK');
   await page.locator('#jp-vdk-menu').getByText('Create').click();
   await page.getByLabel('Local').check();
   await page.getByLabel('Job name:').click();
   await page.getByLabel('Job name:').fill('first-job');
   await page.getByLabel('Job team:').click();
   await page.getByLabel('Job team:').fill('example-team');
-  await page.getByLabel('Path to parent directory:').click();
-  await page.getByLabel('Path to parent directory:').fill('sdfgsdfsdfsd');
+  await page.getByLabel('Path to job directory:').click();
+  await page.getByLabel('Path to job directory:').fill('sdfgsdfsdfsd');
   await page.getByRole('button', { name: 'OK' }).click();
   await page
     .locator('div')
     .filter({ hasText: 'Encountered an error when creating the job.' });
   await page.getByRole('button', { name: 'OK' }).click();
 });
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/__init__.py` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/handlers.py` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/handlers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
+import os
 
 import tornado
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.utils import url_path_join
 
 from .job_data import JobDataLoader
 from .vdk_options.vdk_options import VdkOption
@@ -64,14 +65,34 @@
         run_result = VdkUI.run_job(
             input_data[VdkOption.PATH.value],
             input_data[VdkOption.ARGUMENTS.value],
         )
         self.finish(json.dumps(run_result))
 
 
+class DeleteJobHandler(APIHandler):
+    """
+    Class responsible for handling POST request for deleting a Data Job given its name, team and Rest API URL
+    Response: return a json formatted str including:
+        ::error field with error message if an error exists
+        ::message field with status of the Vdk operation
+    """
+
+    @tornado.web.authenticated
+    def post(self):
+        input_data = self.get_json_body()
+        try:
+            status = VdkUI.delete_job(
+                input_data[VdkOption.NAME.value], input_data[VdkOption.TEAM.value]
+            )
+            self.finish(json.dumps({"message": f"{status}", "error": ""}))
+        except Exception as e:
+            self.finish(json.dumps({"message": f"{e}", "error": "true"}))
+
+
 class DownloadJobHandler(APIHandler):
     """
     Class responsible for handling POST request for downloading a Data Job given its name, team,
     Rest API URL, and the path to where the job will be downloaded
     Response: return a json formatted str including:
         ::error field with error message if an error exists
         ::message field with status of the Vdk operation
@@ -87,24 +108,28 @@
                 input_data[VdkOption.PATH.value],
             )
             self.finish(json.dumps({"message": f"{status}", "error": ""}))
         except Exception as e:
             self.finish(json.dumps({"message": f"{e}", "error": "true"}))
 
 
-class ConvertJobToNotebookHandler(APIHandler):
+class ConvertJobHandler(APIHandler):
     """
-    Class responsible for handling POST request for converting a Data Job to Notebook given the Rest API URL
-    and the path to its directory
+    Class responsible for handling POST request for transforming a directory type Data job(with .py and .sql files)
+    to a notebook type data job
     """
 
     @tornado.web.authenticated
     def post(self):
-        # TODO fix this as part of the implementation
-        print("Successfully connected to the Convert Job To Notebook handler!")
+        input_data = self.get_json_body()
+        try:
+            message = json.dumps(VdkUI.convert_job(input_data[VdkOption.PATH.value]))
+            self.finish(json.dumps({"message": f"{message}", "error": ""}))
+        except Exception as e:
+            self.finish(json.dumps({"message": f"{e}", "error": "true"}))
 
 
 class CreateJobHandler(APIHandler):
     """
     Class responsible for handling POST request for creating a Data Job given its name, team,
     flags whether it will be created locally or in the cloud, path to where job will be created (if local),
     Rest API URL (if cloud)
@@ -168,26 +193,34 @@
     @tornado.web.authenticated
     def post(self):
         input_data = self.get_json_body()
         vdk_indices = VdkUI.get_vdk_tagged_cell_indices(input_data["nbPath"])
         self.finish(json.dumps(vdk_indices))
 
 
+class GetServerPathHandler(APIHandler):
+    @tornado.web.authenticated
+    def get(self):
+        self.finish(json.dumps(os.getcwd()))
+
+
 def setup_handlers(web_app):
     host_pattern = ".*$"
     base_url = web_app.settings["base_url"]
 
     def add_handler(handler, endpoint):
         job_route_pattern = url_path_join(
             base_url, "vdk-jupyterlab-extension", endpoint
         )
         job_handlers = [(job_route_pattern, handler)]
         web_app.add_handlers(host_pattern, job_handlers)
 
     add_handler(RunJobHandler, "run")
+    add_handler(DeleteJobHandler, "delete")
     add_handler(DownloadJobHandler, "download")
-    add_handler(ConvertJobToNotebookHandler, "convertJobToNotebook")
+    add_handler(ConvertJobHandler, "convertJobToNotebook")
     add_handler(CreateJobHandler, "create")
     add_handler(LoadJobDataHandler, "job")
     add_handler(CreateDeploymentHandler, "deploy")
     add_handler(GetNotebookInfoHandler, "notebook")
     add_handler(GetVdkCellIndicesHandler, "vdkCellIndices")
+    add_handler(GetServerPathHandler, "serverPath")
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/vdk_ui.py` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/vdk_ui.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import os
 import pathlib
 import shlex
 import subprocess
 from pathlib import Path
 
 from vdk.internal.control.command_groups.job.create import JobCreate
+from vdk.internal.control.command_groups.job.delete import JobDelete
 from vdk.internal.control.command_groups.job.deploy_cli_impl import JobDeploy
 from vdk.internal.control.command_groups.job.download_job import JobDownloadSource
 from vdk.internal.control.utils import cli_utils
+from vdk_jupyterlab_extension.convert_job import ConvertJobDirectoryProcessor
+from vdk_jupyterlab_extension.convert_job import DirectoryArchiver
 
 
 class RestApiUrlConfiguration:
     @staticmethod
     def get_rest_api_url():
         try:
             rest_api_url = os.environ["REST_API_URL"]
@@ -85,14 +88,26 @@
                         # the json is generated in vdk-notebook plugin
                         # you can see /vdk-notebook/src/vdk/notebook-plugin.py
                         error = json.load(file)
                         return {"message": error["details"]}
             return {"message": process.returncode}
 
     @staticmethod
+    def delete_job(name: str, team: str):
+        """
+        Execute `delete job`.
+        :param name: the name of the data job that will be deleted
+        :param team: the team of the data job that will be deleted
+        :return: message that the job is deleted
+        """
+        cmd = JobDelete(RestApiUrlConfiguration.get_rest_api_url())
+        cmd.delete_job(name, team)
+        return f"Deleted the job with name {name} from {team} team. "
+
+    @staticmethod
     def download_job(name: str, team: str, path: str):
         """
         Execute `download job`.
         :param name: the name of the data job that will be downloaded
         :param team: the team of the data job that will be downloaded
         :param path: the path to the directory where the job will be downloaded
         :return: message that the job is downloaded
@@ -205,7 +220,27 @@
         with open(notebook_path) as f:
             notebook_json = json.load(f)
             vdk_cells = []
             for index, jupyter_cell in enumerate(notebook_json["cells"]):
                 if "vdk" in jupyter_cell["metadata"].get("tags", {}):
                     vdk_cells.append(index)
             return vdk_cells
+
+    @staticmethod
+    def convert_job(job_dir: str):
+        """
+        Transforms the job in the specified directory by archiving it, processing the Python and SQL files,
+        and returning a processed code structure.
+        :param job_dir: Path to the directory of the job to be transformed.
+        :return: The processed code structure.
+        """
+        job_dir = Path(job_dir)
+        archiver = DirectoryArchiver(job_dir)
+        processor = ConvertJobDirectoryProcessor(job_dir)
+        archiver.archive_folder()
+        processor.process_files()
+        message = {
+            "code_structure": processor.get_code_structure(),
+            "removed_files": processor.get_removed_files(),
+        }
+        processor.cleanup()
+        return message
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/10_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/README.md` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/jupyter_sample_job/config.ini` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/jupyter_sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/package.json` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759057971014493%*

 * *Differences: {"'devDependencies'": "{'jest-fetch-mock': '^3.0.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f9166f3ab54776548603.js'}}",*

 * * "'version'": "'0.1.943371983'"}*

```diff
@@ -46,14 +46,15 @@
         "@typescript-eslint/eslint-plugin": "4.8.1",
         "@typescript-eslint/parser": "4.8.1",
         "babel-jest": "27.5.1",
         "eslint": "7.14.0",
         "eslint-config-prettier": "6.15.0",
         "eslint-plugin-prettier": "3.1.4",
         "jest": "27.0.6",
+        "jest-fetch-mock": "^3.0.0",
         "mkdirp": "1.0.3",
         "npm-run-all": "4.1.5",
         "prettier": "2.1.1",
         "rimraf": "3.0.2",
         "stylelint": "14.3.0",
         "stylelint-config-prettier": "9.0.4",
         "stylelint-config-recommended": "6.0.0",
@@ -77,15 +78,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3b6333fd6a058bff7cf9.js",
+            "load": "static/remoteEntry.f9166f3ab54776548603.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "vdk_jupyterlab_extension"
                 },
@@ -150,9 +151,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.940205024"
+    "version": "0.1.943371983"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9762845849802372%*

 * *Differences: {"'devDependencies'": "{'jest-fetch-mock': '^3.0.0'}", "'version'": "'0.1.943371983'"}*

```diff
@@ -46,14 +46,15 @@
         "@typescript-eslint/eslint-plugin": "4.8.1",
         "@typescript-eslint/parser": "4.8.1",
         "babel-jest": "27.5.1",
         "eslint": "7.14.0",
         "eslint-config-prettier": "6.15.0",
         "eslint-plugin-prettier": "3.1.4",
         "jest": "27.0.6",
+        "jest-fetch-mock": "^3.0.0",
         "mkdirp": "1.0.3",
         "npm-run-all": "4.1.5",
         "prettier": "2.1.1",
         "rimraf": "3.0.2",
         "stylelint": "14.3.0",
         "stylelint-config-prettier": "9.0.4",
         "stylelint-config-recommended": "6.0.0",
@@ -145,9 +146,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.940205024"
+    "version": "0.1.943371983"
 }
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/schemas/vdk-jupyterlab-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/747.e678254df7945f8ed34d.js`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/remoteEntry.3b6333fd6a058bff7cf9.js` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/remoteEntry.f9166f3ab54776548603.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, d, s, p, c, h, v, b = {
+    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v, b = {
             913: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(161).then((() => () => t(161))),
                         "./extension": () => t.e(161).then((() => () => t(161))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -43,49 +43,49 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        161: "d4f50a459898d1a8bc76",
+        161: "58979db168f482d72ccd",
         747: "e678254df7945f8ed34d"
     } [e] + ".js?v=" + {
-        161: "d4f50a459898d1a8bc76",
+        161: "58979db168f482d72ccd",
         747: "e678254df7945f8ed34d"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "vdk-jupyterlab-extension:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, u;
             if (void 0 !== o)
                 for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
-                    var d = l[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + o) {
-                        i = d;
+                    var s = l[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+                        i = s;
                         break
                     }
                 }
             i || (u = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var s = (r, n) => {
+            var d = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), u && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), u && document.head.appendChild(i)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => y.e(161).then((() => () => y(161))),
                         from: i,
                         eager: !1
                     })
-                })("vdk-jupyterlab-extension", "0.1.940205024"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("vdk-jupyterlab-extension", "0.1.943371983"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,33 +164,33 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, d, s = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !l || ("u" == s ? u > n && !o : "" == s != o);
-                if ("u" == d) {
-                    if (!l || "u" != s) return !1
+                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                if ("u" == s) {
+                    if (!l || "u" != d) return !1
                 } else if (l)
-                    if (s == d)
+                    if (d == s)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (o ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || d < s != o) return !1;
+                    if (u <= n || s < d != o) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, u--)
+                } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
@@ -201,18 +201,18 @@
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
-        return a(n, o) || d(l(e, t, o, n)), s(e[t][o])
-    }, d = e => {
+        return a(n, o) || s(l(e, t, o, n)), d(e[t][o])
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+    }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
         var a = y.I(r);
         return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
     })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), c = {}, h = {
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
```

### Comparing `vdk_jupyterlab_extension-0.1.940205024/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json` & `vdk_jupyterlab_extension-0.1.943371983/vdk_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/.gitignore` & `vdk_jupyterlab_extension-0.1.943371983/.gitignore`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/README.md` & `vdk_jupyterlab_extension-0.1.943371983/README.md`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/pyproject.toml` & `vdk_jupyterlab_extension-0.1.943371983/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vdk_jupyterlab_extension-0.1.940205024/PKG-INFO` & `vdk_jupyterlab_extension-0.1.943371983/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-jupyterlab-extension
-Version: 0.1.940205024
+Version: 0.1.943371983
 Summary: A Jupyterlab extension for using VDK
 Project-URL: Homepage, https://github.com/vmware/versatile-data-kit
 Project-URL: Bug Tracker, https://github.com/vmware/versatile-data-kit/issues
 Project-URL: Repository, https://github.com/vmware/versatile-data-kit
 Author-email: Versatile Data Kit Development Team <versatile-data-kit@vmware.com>
 License: See https://github.com/vmware/versatile-data-kit/blob/main/LICENSE
 License-File: LICENSE
```

