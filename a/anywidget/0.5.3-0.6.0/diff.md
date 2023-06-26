# Comparing `tmp/anywidget-0.5.3.tar.gz` & `tmp/anywidget-0.6.0.tar.gz`

## Comparing `anywidget-0.5.3.tar` & `anywidget-0.6.0.tar`

### file list

```diff
@@ -1,107 +1,108 @@
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.5.3/.pre-commit-config.yaml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.3/CHANGELOG.md -> packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.5.3/CITATION.cff
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 anywidget-0.5.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget.json
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 anywidget-0.5.3/package.json
--rw-r--r--   0        0        0   274383 2020-02-02 00:00:00.000000 anywidget-0.5.3/pnpm-lock.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.5.3/pnpm-workspace.yaml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 anywidget-0.5.3/tsconfig.json
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.5.3/.changeset/config.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/__init__.py
--rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/_descriptor.py
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/_file_contents.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/_protocols.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/_util.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/_version.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/experimental.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/py.typed
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/widget.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/labextension/package.json
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/labextension/static/138.ac38585aaafa27f6d52e.js
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/labextension/static/326.cde4b6122e4ffce92951.js
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/labextension/static/remoteEntry.06234e67efd98a0438df.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/nbextension/extension.js
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 anywidget-0.5.3/anywidget/nbextension/index.js
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/README.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/astro.config.js
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/package.json
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/tailwind.config.cjs
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/tsconfig.json
--rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/anywidget-overview.png
--rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/banner-dark.png
--rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/banner-light.png
--rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/banner-minimal.png
--rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/client-js-diagram.png
--rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/default-og-image.png
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/favicon.svg
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/make-scrollable-code-focusable.js
--rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/public/widget-overview.png
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/scripts/ipynb.mjs
--rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/scripts/render.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/scripts/utils.mjs
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/consts.ts
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/env.d.ts
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/languages.ts
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/util.ts
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/CodeHero.astro
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/ConfettiButton.astro
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/CounterButton.astro
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/HeadCommon.astro
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/HeadSEO.astro
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Hero.astro
--rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Footer/AvatarList.astro
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Footer/Footer.astro
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/AnyWidgetLogo.astro
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/AstroLogo.astro
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/Header.astro
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/HeaderButton.css
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/LanguageSelect.css
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/LanguageSelect.tsx
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/Search.css
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/Search.tsx
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/SidebarToggle.css
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/SidebarToggle.tsx
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/SkipToContent.astro
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/ThemeToggleButton.css
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/Header/ThemeToggleButton.tsx
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/LeftSidebar/LeftSidebar.astro
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/PageContent/PageContent.astro
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/RightSidebar/MoreMenu.astro
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/RightSidebar/RightSidebar.astro
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/RightSidebar/TableOfContents.tsx
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/components/examples/Counter.astro
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/layouts/MainLayout.astro
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/layouts/SplashLayout.astro
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/index.astro
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/blog/anywidget-02.md
--rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/blog/introducing-anywidget.mdx
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/en/bundling.md
--rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/en/experimental.md
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/en/getting-started.mdx
--rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/en/jupyter-widgets-the-good-parts.md
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/pages/en/notebooks/counter.ipynb
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/styles/index.css
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.5.3/docs/src/styles/theme.css
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.5.3/examples/Counter.ipynb
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.5.3/examples/minimal_example.ipynb
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/CHANGELOG.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/build.mjs
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/package.json
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/tsconfig.json
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/src/index.js
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/src/plugin.js
--rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 anywidget-0.5.3/packages/anywidget/src/widget.js
--rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.5.3/tests/test_descriptor.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.5.3/tests/test_experimental.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.5.3/tests/test_file_contents.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.5.3/tests/test_protocols.py
--rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.5.3/tests/test_utils.py
--rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.5.3/tests/test_widget.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.5.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.5.3/LICENSE
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 anywidget-0.5.3/README.md
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 anywidget-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 anywidget-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 anywidget-0.6.0/.pre-commit-config.yaml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.0/CHANGELOG.md -> packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 anywidget-0.6.0/CITATION.cff
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 anywidget-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget.json
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 anywidget-0.6.0/package.json
+-rw-r--r--   0        0        0   267802 2020-02-02 00:00:00.000000 anywidget-0.6.0/pnpm-lock.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 anywidget-0.6.0/pnpm-workspace.yaml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 anywidget-0.6.0/tsconfig.json
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 anywidget-0.6.0/.changeset/config.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/__init__.py
+-rw-r--r--   0        0        0    25087 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_descriptor.py
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_file_contents.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_protocols.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_util.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/_version.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/experimental.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/py.typed
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/widget.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/package.json
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/138.3fd6605047ad3df65a9e.js
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/326.c68678f64e2971595925.js
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/remoteEntry.cba6b4061725caaf22a8.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/nbextension/extension.js
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 anywidget-0.6.0/anywidget/nbextension/index.js
+-rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/README.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/astro.config.js
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/package.json
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/tailwind.config.cjs
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/tsconfig.json
+-rw-r--r--   0        0        0   625221 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/anywidget-overview.png
+-rw-r--r--   0        0        0   440603 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/banner-dark.png
+-rw-r--r--   0        0        0   413948 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/banner-light.png
+-rw-r--r--   0        0        0   101574 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/banner-minimal.png
+-rw-r--r--   0        0        0   678629 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/client-js-diagram.png
+-rw-r--r--   0        0        0   748347 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/default-og-image.png
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/favicon.svg
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/make-scrollable-code-focusable.js
+-rw-r--r--   0        0        0   275942 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/public/widget-overview.png
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/scripts/ipynb.mjs
+-rwxr-xr-x   0        0        0      271 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/scripts/render.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/scripts/utils.mjs
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/consts.ts
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/env.d.ts
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/languages.ts
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/util.ts
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/CodeHero.astro
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/ConfettiButton.astro
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/CounterButton.astro
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/HeadCommon.astro
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/HeadSEO.astro
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Hero.astro
+-rw-r--r--   0        0        0     5676 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Footer/AvatarList.astro
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Footer/Footer.astro
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/AnyWidgetLogo.astro
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/AstroLogo.astro
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/Header.astro
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/HeaderButton.css
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/LanguageSelect.css
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/LanguageSelect.tsx
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/Search.css
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/Search.tsx
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/SidebarToggle.css
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/SidebarToggle.tsx
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/SkipToContent.astro
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.css
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.tsx
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/LeftSidebar/LeftSidebar.astro
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/PageContent/PageContent.astro
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/RightSidebar/MoreMenu.astro
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/RightSidebar/RightSidebar.astro
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/RightSidebar/TableOfContents.tsx
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/components/examples/Counter.astro
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/layouts/MainLayout.astro
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/layouts/SplashLayout.astro
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/index.astro
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/blog/anywidget-02.md
+-rw-r--r--   0        0        0    22399 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/blog/introducing-anywidget.mdx
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/bundling.md
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/experimental.md
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/getting-started.mdx
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/pages/en/notebooks/counter.ipynb
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/styles/index.css
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 anywidget-0.6.0/docs/src/styles/theme.css
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 anywidget-0.6.0/examples/Counter.ipynb
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 anywidget-0.6.0/examples/minimal_example.ipynb
+-rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/CHANGELOG.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/build.mjs
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/tsconfig.json
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/__tests__/widget.test.ts
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/src/index.js
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/src/plugin.js
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 anywidget-0.6.0/packages/anywidget/src/widget.js
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_descriptor.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_experimental.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_file_contents.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_protocols.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 anywidget-0.6.0/tests/test_widget.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 anywidget-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 anywidget-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 anywidget-0.6.0/README.md
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 anywidget-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 anywidget-0.6.0/PKG-INFO
```

### Comparing `anywidget-0.5.3/.pre-commit-config.yaml` & `anywidget-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/CITATION.cff` & `anywidget-0.6.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/CONTRIBUTING.md` & `anywidget-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/package.json` & `anywidget-0.6.0/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/pnpm-lock.yaml` & `anywidget-0.6.0/pnpm-lock.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-lockfileVersion: '6.1'
+lockfileVersion: '6.0'
 
 settings:
   autoInstallPeers: true
   excludeLinksFromLockfile: false
 
 importers:
 
@@ -94,31 +94,34 @@
         specifier: ^0.7.2
         version: 0.7.2
       shiki:
         specifier: ^0.14.1
         version: 0.14.1
       vite:
         specifier: ^4.1.4
-        version: 4.1.4(@types/node@18.0.0)
+        version: 4.3.9(@types/node@18.0.0)
 
   packages/anywidget:
     dependencies:
       '@anywidget/types':
         specifier: workspace:~
         version: link:../types
       '@anywidget/vite':
         specifier: workspace:~
         version: link:../vite
       '@jupyter-widgets/base':
         specifier: ^2 || ^3 || ^4 || ^5 || ^6
         version: 2.0.0
     devDependencies:
+      '@jupyter-widgets/base-manager':
+        specifier: ^1.0.5
+        version: 1.0.5(crypto@1.0.1)
       '@jupyterlab/builder':
-        specifier: ^3.6.4
-        version: 3.6.4(crypto@1.0.1)(esbuild@0.18.6)
+        specifier: ^4.0.2
+        version: 4.0.2(esbuild@0.18.6)
 
   packages/types: {}
 
   packages/vite:
     devDependencies:
       vite:
         specifier: ^4.3.9
@@ -132,137 +135,137 @@
       '@algolia/autocomplete-shared': 1.6.3
     dev: false
 
   /@algolia/autocomplete-shared@1.6.3:
     resolution: {integrity: sha512-UV46bnkTztyADFaETfzFC5ryIdGVb2zpAoYgu0tfcuYWjhg1KbLXveFffZIrGVoboqmAk1b+jMrl6iCja1i3lg==}
     dev: false
 
-  /@algolia/cache-browser-local-storage@4.17.2:
-    resolution: {integrity: sha512-ZkVN7K/JE+qMQbpR6h3gQOGR6yCJpmucSBCmH5YDxnrYbp2CbrVCu0Nr+FGVoWzMJNznj1waShkfQ9awERulLw==}
+  /@algolia/cache-browser-local-storage@4.18.0:
+    resolution: {integrity: sha512-rUAs49NLlO8LVLgGzM4cLkw8NJLKguQLgvFmBEe3DyzlinoqxzQMHfKZs6TSq4LZfw/z8qHvRo8NcTAAUJQLcw==}
     dependencies:
-      '@algolia/cache-common': 4.17.2
+      '@algolia/cache-common': 4.18.0
     dev: false
 
   /@algolia/cache-common@4.13.1:
     resolution: {integrity: sha512-7Vaf6IM4L0Jkl3sYXbwK+2beQOgVJ0mKFbz/4qSxKd1iy2Sp77uTAazcX+Dlexekg1fqGUOSO7HS4Sx47ZJmjA==}
     dev: false
 
-  /@algolia/cache-common@4.17.2:
-    resolution: {integrity: sha512-fojbhYIS8ovfYs6hwZpy1O4mBfVRxNgAaZRqsdVQd54hU4MxYDYFCxagYX28lOBz7btcDHld6BMoWXvjzkx6iQ==}
+  /@algolia/cache-common@4.18.0:
+    resolution: {integrity: sha512-BmxsicMR4doGbeEXQu8yqiGmiyvpNvejYJtQ7rvzttEAMxOPoWEHrWyzBQw4x7LrBY9pMrgv4ZlUaF8PGzewHg==}
     dev: false
 
-  /@algolia/cache-in-memory@4.17.2:
-    resolution: {integrity: sha512-UYQcMzPurNi+cPYkuPemTZkjKAjdgAS1hagC5irujKbrYnN4yscK4TkOI5tX+O8/KegtJt3kOK07OIrJ2QDAAw==}
+  /@algolia/cache-in-memory@4.18.0:
+    resolution: {integrity: sha512-evD4dA1nd5HbFdufBxLqlJoob7E2ozlqJZuV3YlirNx5Na4q1LckIuzjNYZs2ddLzuTc/Xd5O3Ibf7OwPskHxw==}
     dependencies:
-      '@algolia/cache-common': 4.17.2
+      '@algolia/cache-common': 4.18.0
     dev: false
 
-  /@algolia/client-account@4.17.2:
-    resolution: {integrity: sha512-doSk89pBPDpDyKJSHFADIGa2XSGrBCj3QwPvqtRJXDADpN+OjW+eTR8r4hEs/7X4GGfjfAOAES8JgDx+fZntYw==}
+  /@algolia/client-account@4.18.0:
+    resolution: {integrity: sha512-XsDnlROr3+Z1yjxBJjUMfMazi1V155kVdte6496atvBgOEtwCzTs3A+qdhfsAnGUvaYfBrBkL0ThnhMIBCGcew==}
     dependencies:
-      '@algolia/client-common': 4.17.2
-      '@algolia/client-search': 4.17.2
-      '@algolia/transporter': 4.17.2
+      '@algolia/client-common': 4.18.0
+      '@algolia/client-search': 4.18.0
+      '@algolia/transporter': 4.18.0
     dev: false
 
-  /@algolia/client-analytics@4.17.2:
-    resolution: {integrity: sha512-V+DcXbOtD/hKwAR3qGQrtlrJ3q2f9OKfx843q744o4m3xHv5ueCAvGXB1znPsdaUrVDNAImcgEgqwI9x7EJbDw==}
+  /@algolia/client-analytics@4.18.0:
+    resolution: {integrity: sha512-chEUSN4ReqU7uRQ1C8kDm0EiPE+eJeAXiWcBwLhEynfNuTfawN9P93rSZktj7gmExz0C8XmkbBU19IQ05wCNrQ==}
     dependencies:
-      '@algolia/client-common': 4.17.2
-      '@algolia/client-search': 4.17.2
-      '@algolia/requester-common': 4.17.2
-      '@algolia/transporter': 4.17.2
+      '@algolia/client-common': 4.18.0
+      '@algolia/client-search': 4.18.0
+      '@algolia/requester-common': 4.18.0
+      '@algolia/transporter': 4.18.0
     dev: false
 
   /@algolia/client-common@4.13.1:
     resolution: {integrity: sha512-LcDoUE0Zz3YwfXJL6lJ2OMY2soClbjrrAKB6auYVMNJcoKZZ2cbhQoFR24AYoxnGUYBER/8B+9sTBj5bj/Gqbg==}
     dependencies:
       '@algolia/requester-common': 4.13.1
       '@algolia/transporter': 4.13.1
     dev: false
 
-  /@algolia/client-common@4.17.2:
-    resolution: {integrity: sha512-gKBUnjxi0ukJYIJxVREYGt1Dmj1B3RBYbfGWi0dIPp1BC1VvQm+BOuNwsIwmq/x3MPO+sGuK978eKiP3tZDvag==}
+  /@algolia/client-common@4.18.0:
+    resolution: {integrity: sha512-7N+soJFP4wn8tjTr3MSUT/U+4xVXbz4jmeRfWfVAzdAbxLAQbHa0o/POSdTvQ8/02DjCLelloZ1bb4ZFVKg7Wg==}
     dependencies:
-      '@algolia/requester-common': 4.17.2
-      '@algolia/transporter': 4.17.2
+      '@algolia/requester-common': 4.18.0
+      '@algolia/transporter': 4.18.0
     dev: false
 
-  /@algolia/client-personalization@4.17.2:
-    resolution: {integrity: sha512-wc4UgOWxSYWz5wpuelNmlt895jA9twjZWM2ms17Ws8qCvBHF7OVGdMGgbysPB8790YnfvvDnSsWOv3CEj26Eow==}
+  /@algolia/client-personalization@4.18.0:
+    resolution: {integrity: sha512-+PeCjODbxtamHcPl+couXMeHEefpUpr7IHftj4Y4Nia1hj8gGq4VlIcqhToAw8YjLeCTfOR7r7xtj3pJcYdP8A==}
     dependencies:
-      '@algolia/client-common': 4.17.2
-      '@algolia/requester-common': 4.17.2
-      '@algolia/transporter': 4.17.2
+      '@algolia/client-common': 4.18.0
+      '@algolia/requester-common': 4.18.0
+      '@algolia/transporter': 4.18.0
     dev: false
 
   /@algolia/client-search@4.13.1:
     resolution: {integrity: sha512-YQKYA83MNRz3FgTNM+4eRYbSmHi0WWpo019s5SeYcL3HUan/i5R09VO9dk3evELDFJYciiydSjbsmhBzbpPP2A==}
     dependencies:
       '@algolia/client-common': 4.13.1
       '@algolia/requester-common': 4.13.1
       '@algolia/transporter': 4.13.1
     dev: false
 
-  /@algolia/client-search@4.17.2:
-    resolution: {integrity: sha512-FUjIs+gRe0upJC++uVs4sdxMw15JxfkT86Gr/kqVwi9kcqaZhXntSbW/Fw959bIYXczjmeVQsilYvBWW4YvSZA==}
+  /@algolia/client-search@4.18.0:
+    resolution: {integrity: sha512-F9xzQXTjm6UuZtnsLIew6KSraXQ0AzS/Ee+OD+mQbtcA/K1sg89tqb8TkwjtiYZ0oij13u3EapB3gPZwm+1Y6g==}
     dependencies:
-      '@algolia/client-common': 4.17.2
-      '@algolia/requester-common': 4.17.2
-      '@algolia/transporter': 4.17.2
+      '@algolia/client-common': 4.18.0
+      '@algolia/requester-common': 4.18.0
+      '@algolia/transporter': 4.18.0
     dev: false
 
   /@algolia/logger-common@4.13.1:
     resolution: {integrity: sha512-L6slbL/OyZaAXNtS/1A8SAbOJeEXD5JcZeDCPYDqSTYScfHu+2ePRTDMgUTY4gQ7HsYZ39N1LujOd8WBTmM2Aw==}
     dev: false
 
-  /@algolia/logger-common@4.17.2:
-    resolution: {integrity: sha512-EfXuweUE+1HiSMsQidaDWA5Lv4NnStYIlh7PO5pLkI+sdhbMX0e5AO5nUAMIFM1VkEANes70RA8fzhP6OqCqQQ==}
+  /@algolia/logger-common@4.18.0:
+    resolution: {integrity: sha512-46etYgSlkoKepkMSyaoriSn2JDgcrpc/nkOgou/lm0y17GuMl9oYZxwKKTSviLKI5Irk9nSKGwnBTQYwXOYdRg==}
     dev: false
 
-  /@algolia/logger-console@4.17.2:
-    resolution: {integrity: sha512-JuG8HGVlJ+l/UEDK4h2Y8q/IEmRjQz1J0aS9tf6GPNbGYiSvMr1DDdZ+hqV3bb1XE6wU8Ypex56HisWMSpnG0A==}
+  /@algolia/logger-console@4.18.0:
+    resolution: {integrity: sha512-3P3VUYMl9CyJbi/UU1uUNlf6Z8N2ltW3Oqhq/nR7vH0CjWv32YROq3iGWGxB2xt3aXobdUPXs6P0tHSKRmNA6g==}
     dependencies:
-      '@algolia/logger-common': 4.17.2
+      '@algolia/logger-common': 4.18.0
     dev: false
 
-  /@algolia/requester-browser-xhr@4.17.2:
-    resolution: {integrity: sha512-FKI2lYWwksALfRt2OETFmGb5+P7WVc4py2Ai3H7k8FSfTLwVvs9WVVmtlx6oANQ8RFEK4B85h8DQJTJ29TDfmA==}
+  /@algolia/requester-browser-xhr@4.18.0:
+    resolution: {integrity: sha512-/AcWHOBub2U4TE/bPi4Gz1XfuLK6/7dj4HJG+Z2SfQoS1RjNLshZclU3OoKIkFp8D2NC7+BNsPvr9cPLyW8nyQ==}
     dependencies:
-      '@algolia/requester-common': 4.17.2
+      '@algolia/requester-common': 4.18.0
     dev: false
 
   /@algolia/requester-common@4.13.1:
     resolution: {integrity: sha512-eGVf0ID84apfFEuXsaoSgIxbU3oFsIbz4XiotU3VS8qGCJAaLVUC5BUJEkiFENZIhon7hIB4d0RI13HY4RSA+w==}
     dev: false
 
-  /@algolia/requester-common@4.17.2:
-    resolution: {integrity: sha512-Rfim23ztAhYpE9qm+KCfCRo+YLJCjiiTG+IpDdzUjMpYPhUtirQT0A35YEd/gKn86YNyydxS9w8iRSjwKh+L0A==}
+  /@algolia/requester-common@4.18.0:
+    resolution: {integrity: sha512-xlT8R1qYNRBCi1IYLsx7uhftzdfsLPDGudeQs+xvYB4sQ3ya7+ppolB/8m/a4F2gCkEO6oxpp5AGemM7kD27jA==}
     dev: false
 
-  /@algolia/requester-node-http@4.17.2:
-    resolution: {integrity: sha512-E0b0kyCDMvUIhQmDNd/mH4fsKJdEEX6PkMKrYJjzm6moo+rP22tqpq4Rfe7DZD8OB6/LsDD3zs3Kvd+L+M5wwQ==}
+  /@algolia/requester-node-http@4.18.0:
+    resolution: {integrity: sha512-TGfwj9aeTVgOUhn5XrqBhwUhUUDnGIKlI0kCBMdR58XfXcfdwomka+CPIgThRbfYw04oQr31A6/95ZH2QVJ9UQ==}
     dependencies:
-      '@algolia/requester-common': 4.17.2
+      '@algolia/requester-common': 4.18.0
     dev: false
 
   /@algolia/transporter@4.13.1:
     resolution: {integrity: sha512-pICnNQN7TtrcYJqqPEXByV8rJ8ZRU2hCiIKLTLRyNpghtQG3VAFk6fVtdzlNfdUGZcehSKGarPIZEHlQXnKjgw==}
     dependencies:
       '@algolia/cache-common': 4.13.1
       '@algolia/logger-common': 4.13.1
       '@algolia/requester-common': 4.13.1
     dev: false
 
-  /@algolia/transporter@4.17.2:
-    resolution: {integrity: sha512-m8pXlz5OnNzjD1rcw+duCN4jG4yEzkJBsvKYMoN22Oq6rQwy1AY5muZ+IQUs4dL+A364CYkRMLRWhvXpCZ1x+g==}
+  /@algolia/transporter@4.18.0:
+    resolution: {integrity: sha512-xbw3YRUGtXQNG1geYFEDDuFLZt4Z8YNKbamHPkzr3rWc6qp4/BqEeXcI2u/P/oMq2yxtXgMxrCxOPA8lyIe5jw==}
     dependencies:
-      '@algolia/cache-common': 4.17.2
-      '@algolia/logger-common': 4.17.2
-      '@algolia/requester-common': 4.17.2
+      '@algolia/cache-common': 4.18.0
+      '@algolia/logger-common': 4.18.0
+      '@algolia/requester-common': 4.18.0
     dev: false
 
   /@alloc/quick-lru@5.2.0:
     resolution: {integrity: sha512-UrcABB+4bUrFABwbluTIBErXwvbsU/V7TZWfmbgJfbkwiBuziS9gxdODUyuiecfdGQ85jglMW6juS3+z5TsKLw==}
     engines: {node: '>=10'}
     dev: false
 
@@ -646,15 +649,15 @@
       '@changesets/git': 2.0.0
       '@changesets/types': 5.2.1
       '@manypkg/get-packages': 1.1.3
       detect-indent: 6.1.0
       fs-extra: 7.0.1
       lodash.startcase: 4.4.0
       outdent: 0.5.0
-      prettier: 2.8.8
+      prettier: 2.8.2
       resolve-from: 5.0.0
       semver: 5.7.1
     dev: true
 
   /@changesets/assemble-release-plan@5.2.3:
     resolution: {integrity: sha512-g7EVZCmnWz3zMBAdrcKhid4hkHT+Ft1n0mLussFMcB1dE2zCuwcvGoy9ec3yOgPGF4hoMtgHaMIk3T3TBdvU9g==}
     dependencies:
@@ -823,15 +826,15 @@
   /@changesets/write@0.2.3:
     resolution: {integrity: sha512-Dbamr7AIMvslKnNYsLFafaVORx4H0pvCA2MHqgtNCySMe1blImEyAEOzDmcgKAkgz4+uwoLz7demIrX+JBr/Xw==}
     dependencies:
       '@babel/runtime': 7.22.5
       '@changesets/types': 5.2.1
       fs-extra: 7.0.1
       human-id: 1.0.2
-      prettier: 2.8.8
+      prettier: 2.8.2
     dev: true
 
   /@discoveryjs/json-ext@0.5.7:
     resolution: {integrity: sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==}
     engines: {node: '>=10.0.0'}
     dev: true
 
@@ -845,15 +848,15 @@
       '@types/react': '>= 16.8.0 < 19.0.0'
       react: '>= 16.8.0 < 19.0.0'
       react-dom: '>= 16.8.0 < 19.0.0'
     dependencies:
       '@algolia/autocomplete-core': 1.6.3
       '@docsearch/css': 3.1.0
       '@types/react': 18.2.8
-      algoliasearch: 4.17.2
+      algoliasearch: 4.18.0
       react: 18.2.0
       react-dom: 18.2.0(react@18.2.0)
     dev: false
 
   /@emmetio/abbreviation@2.3.3:
     resolution: {integrity: sha512-mgv58UrU3rh4YgbE/TzgLQwJ3pFsHHhCLqY20aJq+9comytTXUDNGG/SMtSeMJdkpxgXSXunBGLD8Boka3JyVA==}
     dependencies:
@@ -863,23 +866,14 @@
     resolution: {integrity: sha512-s9yjhJ6saOO/uk1V74eifykk2CBYi01STTK3WlXWGOepyKa23ymJ053+DNQjpFcy1ingpaO7AxCcwLvHFY9tuw==}
     dependencies:
       '@emmetio/scanner': 1.0.4
 
   /@emmetio/scanner@1.0.4:
     resolution: {integrity: sha512-IqRuJtQff7YHHBk4G8YZ45uB9BaAGcwQeVzgj/zj8/UdOhtQpEIupUhSk8dys6spFIWVZVeK20CzGEnqR5SbqA==}
 
-  /@esbuild/android-arm64@0.16.17:
-    resolution: {integrity: sha512-MIGl6p5sc3RDTLLkYL1MyL8BMRN4tLMRCn+yRJJmEDvYZ2M7tmAf80hx1kbNEUX2KJ50RRtxZ4JHLvCfuB6kBg==}
-    engines: {node: '>=12'}
-    cpu: [arm64]
-    os: [android]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/android-arm64@0.17.19:
     resolution: {integrity: sha512-KBMWvEZooR7+kzY0BtbTQn0OAYY7CsiydT63pVEaPtVYF0hXbUaOyZog37DKxK7NF3XacBJOpYT4adIJh+avxA==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     optional: true
@@ -889,23 +883,14 @@
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-arm@0.16.17:
-    resolution: {integrity: sha512-N9x1CMXVhtWEAMS7pNNONyA14f71VPQN9Cnavj1XQh6T7bskqiLLrSca4O0Vr8Wdcga943eThxnVp3JLnBMYtw==}
-    engines: {node: '>=12'}
-    cpu: [arm]
-    os: [android]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/android-arm@0.17.19:
     resolution: {integrity: sha512-rIKddzqhmav7MSmoFCmDIb6e2W57geRsM94gV2l38fzhXMwq7hZoClug9USI2pFRGL06f4IOPHHpFNOkWieR8A==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     optional: true
@@ -915,23 +900,14 @@
     engines: {node: '>=12'}
     cpu: [arm]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/android-x64@0.16.17:
-    resolution: {integrity: sha512-a3kTv3m0Ghh4z1DaFEuEDfz3OLONKuFvI4Xqczqx4BqLyuFaFkuaG4j2MtA6fuWEFeC5x9IvqnX7drmRq/fyAQ==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [android]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/android-x64@0.17.19:
     resolution: {integrity: sha512-uUTTc4xGNDT7YSArp/zbtmbhO0uEEK9/ETW29Wk1thYUJBz3IVnvgEiEwEa9IeLyvnpKrWK64Utw2bgUmDveww==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     optional: true
@@ -941,23 +917,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [android]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/darwin-arm64@0.16.17:
-    resolution: {integrity: sha512-/2agbUEfmxWHi9ARTX6OQ/KgXnOWfsNlTeLcoV7HSuSTv63E4DqtAc+2XqGw1KHxKMHGZgbVCZge7HXWX9Vn+w==}
-    engines: {node: '>=12'}
-    cpu: [arm64]
-    os: [darwin]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/darwin-arm64@0.17.19:
     resolution: {integrity: sha512-80wEoCfF/hFKM6WE1FyBHc9SfUblloAWx6FJkFWTWiCoht9Mc0ARGEM47e67W9rI09YoUxJL68WHfDRYEAvOhg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     optional: true
@@ -967,23 +934,14 @@
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/darwin-x64@0.16.17:
-    resolution: {integrity: sha512-2By45OBHulkd9Svy5IOCZt376Aa2oOkiE9QWUK9fe6Tb+WDr8hXL3dpqi+DeLiMed8tVXspzsTAvd0jUl96wmg==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [darwin]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/darwin-x64@0.17.19:
     resolution: {integrity: sha512-IJM4JJsLhRYr9xdtLytPLSH9k/oxR3boaUIYiHkAawtwNOXKE8KoU8tMvryogdcT8AU+Bflmh81Xn6Q0vTZbQw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     optional: true
@@ -993,23 +951,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [darwin]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/freebsd-arm64@0.16.17:
-    resolution: {integrity: sha512-mt+cxZe1tVx489VTb4mBAOo2aKSnJ33L9fr25JXpqQqzbUIw/yzIzi+NHwAXK2qYV1lEFp4OoVeThGjUbmWmdw==}
-    engines: {node: '>=12'}
-    cpu: [arm64]
-    os: [freebsd]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/freebsd-arm64@0.17.19:
     resolution: {integrity: sha512-pBwbc7DufluUeGdjSU5Si+P3SoMF5DQ/F/UmTSb8HXO80ZEAJmrykPyzo1IfNbAoaqw48YRpv8shwd1NoI0jcQ==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     optional: true
@@ -1019,23 +968,14 @@
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/freebsd-x64@0.16.17:
-    resolution: {integrity: sha512-8ScTdNJl5idAKjH8zGAsN7RuWcyHG3BAvMNpKOBaqqR7EbUhhVHOqXRdL7oZvz8WNHL2pr5+eIT5c65kA6NHug==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [freebsd]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/freebsd-x64@0.17.19:
     resolution: {integrity: sha512-4lu+n8Wk0XlajEhbEffdy2xy53dpR06SlzvhGByyg36qJw6Kpfk7cp45DR/62aPH9mtJRmIyrXAS5UWBrJT6TQ==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     optional: true
@@ -1045,23 +985,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [freebsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-arm64@0.16.17:
-    resolution: {integrity: sha512-7S8gJnSlqKGVJunnMCrXHU9Q8Q/tQIxk/xL8BqAP64wchPCTzuM6W3Ra8cIa1HIflAvDnNOt2jaL17vaW+1V0g==}
-    engines: {node: '>=12'}
-    cpu: [arm64]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-arm64@0.17.19:
     resolution: {integrity: sha512-ct1Tg3WGwd3P+oZYqic+YZF4snNl2bsnMKRkb3ozHmnM0dGWuxcPTTntAF6bOP0Sp4x0PjSF+4uHQ1xvxfRKqg==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1071,23 +1002,14 @@
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-arm@0.16.17:
-    resolution: {integrity: sha512-iihzrWbD4gIT7j3caMzKb/RsFFHCwqqbrbH9SqUSRrdXkXaygSZCZg1FybsZz57Ju7N/SHEgPyaR0LZ8Zbe9gQ==}
-    engines: {node: '>=12'}
-    cpu: [arm]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-arm@0.17.19:
     resolution: {integrity: sha512-cdmT3KxjlOQ/gZ2cjfrQOtmhG4HJs6hhvm3mWSRDPtZ/lP5oe8FWceS10JaSJC13GBd4eH/haHnqf7hhGNLerA==}
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1097,23 +1019,14 @@
     engines: {node: '>=12'}
     cpu: [arm]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-ia32@0.16.17:
-    resolution: {integrity: sha512-kiX69+wcPAdgl3Lonh1VI7MBr16nktEvOfViszBSxygRQqSpzv7BffMKRPMFwzeJGPxcio0pdD3kYQGpqQ2SSg==}
-    engines: {node: '>=12'}
-    cpu: [ia32]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-ia32@0.17.19:
     resolution: {integrity: sha512-w4IRhSy1VbsNxHRQpeGCHEmibqdTUx61Vc38APcsRbuVgK0OPEnQ0YD39Brymn96mOx48Y2laBQGqgZ0j9w6SQ==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1123,23 +1036,14 @@
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-loong64@0.16.17:
-    resolution: {integrity: sha512-dTzNnQwembNDhd654cA4QhbS9uDdXC3TKqMJjgOWsC0yNCbpzfWoXdZvp0mY7HU6nzk5E0zpRGGx3qoQg8T2DQ==}
-    engines: {node: '>=12'}
-    cpu: [loong64]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-loong64@0.17.19:
     resolution: {integrity: sha512-2iAngUbBPMq439a+z//gE+9WBldoMp1s5GWsUSgqHLzLJ9WoZLZhpwWuym0u0u/4XmZ3gpHmzV84PonE+9IIdQ==}
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1149,23 +1053,14 @@
     engines: {node: '>=12'}
     cpu: [loong64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-mips64el@0.16.17:
-    resolution: {integrity: sha512-ezbDkp2nDl0PfIUn0CsQ30kxfcLTlcx4Foz2kYv8qdC6ia2oX5Q3E/8m6lq84Dj/6b0FrkgD582fJMIfHhJfSw==}
-    engines: {node: '>=12'}
-    cpu: [mips64el]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-mips64el@0.17.19:
     resolution: {integrity: sha512-LKJltc4LVdMKHsrFe4MGNPp0hqDFA1Wpt3jE1gEyM3nKUvOiO//9PheZZHfYRfYl6AwdTH4aTcXSqBerX0ml4A==}
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1175,23 +1070,14 @@
     engines: {node: '>=12'}
     cpu: [mips64el]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-ppc64@0.16.17:
-    resolution: {integrity: sha512-dzS678gYD1lJsW73zrFhDApLVdM3cUF2MvAa1D8K8KtcSKdLBPP4zZSLy6LFZ0jYqQdQ29bjAHJDgz0rVbLB3g==}
-    engines: {node: '>=12'}
-    cpu: [ppc64]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-ppc64@0.17.19:
     resolution: {integrity: sha512-/c/DGybs95WXNS8y3Ti/ytqETiW7EU44MEKuCAcpPto3YjQbyK3IQVKfF6nbghD7EcLUGl0NbiL5Rt5DMhn5tg==}
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1201,23 +1087,14 @@
     engines: {node: '>=12'}
     cpu: [ppc64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-riscv64@0.16.17:
-    resolution: {integrity: sha512-ylNlVsxuFjZK8DQtNUwiMskh6nT0vI7kYl/4fZgV1llP5d6+HIeL/vmmm3jpuoo8+NuXjQVZxmKuhDApK0/cKw==}
-    engines: {node: '>=12'}
-    cpu: [riscv64]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-riscv64@0.17.19:
     resolution: {integrity: sha512-FC3nUAWhvFoutlhAkgHf8f5HwFWUL6bYdvLc/TTuxKlvLi3+pPzdZiFKSWz/PF30TB1K19SuCxDTI5KcqASJqA==}
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1227,23 +1104,14 @@
     engines: {node: '>=12'}
     cpu: [riscv64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-s390x@0.16.17:
-    resolution: {integrity: sha512-gzy7nUTO4UA4oZ2wAMXPNBGTzZFP7mss3aKR2hH+/4UUkCOyqmjXiKpzGrY2TlEUhbbejzXVKKGazYcQTZWA/w==}
-    engines: {node: '>=12'}
-    cpu: [s390x]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-s390x@0.17.19:
     resolution: {integrity: sha512-IbFsFbxMWLuKEbH+7sTkKzL6NJmG2vRyy6K7JJo55w+8xDk7RElYn6xvXtDW8HCfoKBFK69f3pgBJSUSQPr+4Q==}
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1253,23 +1121,14 @@
     engines: {node: '>=12'}
     cpu: [s390x]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/linux-x64@0.16.17:
-    resolution: {integrity: sha512-mdPjPxfnmoqhgpiEArqi4egmBAMYvaObgn4poorpUaqmvzzbvqbowRllQ+ZgzGVMGKaPkqUmPDOOFQRUFDmeUw==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [linux]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/linux-x64@0.17.19:
     resolution: {integrity: sha512-68ngA9lg2H6zkZcyp22tsVt38mlhWde8l3eJLWkyLrp4HwMUr3c1s/M2t7+kHIhvMjglIBrFpncX1SzMckomGw==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     optional: true
@@ -1279,23 +1138,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [linux]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/netbsd-x64@0.16.17:
-    resolution: {integrity: sha512-/PzmzD/zyAeTUsduZa32bn0ORug+Jd1EGGAUJvqfeixoEISYpGnAezN6lnJoskauoai0Jrs+XSyvDhppCPoKOA==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [netbsd]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/netbsd-x64@0.17.19:
     resolution: {integrity: sha512-CwFq42rXCR8TYIjIfpXCbRX0rp1jo6cPIUPSaWwzbVI4aOfX96OXY8M6KNmtPcg7QjYeDmN+DD0Wp3LaBOLf4Q==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     optional: true
@@ -1305,23 +1155,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [netbsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/openbsd-x64@0.16.17:
-    resolution: {integrity: sha512-2yaWJhvxGEz2RiftSk0UObqJa/b+rIAjnODJgv2GbGGpRwAfpgzyrg1WLK8rqA24mfZa9GvpjLcBBg8JHkoodg==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [openbsd]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/openbsd-x64@0.17.19:
     resolution: {integrity: sha512-cnq5brJYrSZ2CF6c35eCmviIN3k3RczmHz8eYaVlNasVqsNY+JKohZU5MKmaOI+KkllCdzOKKdPs762VCPC20g==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     optional: true
@@ -1331,23 +1172,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [openbsd]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/sunos-x64@0.16.17:
-    resolution: {integrity: sha512-xtVUiev38tN0R3g8VhRfN7Zl42YCJvyBhRKw1RJjwE1d2emWTVToPLNEQj/5Qxc6lVFATDiy6LjVHYhIPrLxzw==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [sunos]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/sunos-x64@0.17.19:
     resolution: {integrity: sha512-vCRT7yP3zX+bKWFeP/zdS6SqdWB8OIpaRq/mbXQxTGHnIxspRtigpkUcDMlSCOejlHowLqII7K2JKevwyRP2rg==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     optional: true
@@ -1357,23 +1189,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [sunos]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-arm64@0.16.17:
-    resolution: {integrity: sha512-ga8+JqBDHY4b6fQAmOgtJJue36scANy4l/rL97W+0wYmijhxKetzZdKOJI7olaBaMhWt8Pac2McJdZLxXWUEQw==}
-    engines: {node: '>=12'}
-    cpu: [arm64]
-    os: [win32]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/win32-arm64@0.17.19:
     resolution: {integrity: sha512-yYx+8jwowUstVdorcMdNlzklLYhPxjniHWFKgRqH7IFlUEa0Umu3KuYplf1HUZZ422e3NU9F4LGb+4O0Kdcaag==}
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     optional: true
@@ -1383,23 +1206,14 @@
     engines: {node: '>=12'}
     cpu: [arm64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-ia32@0.16.17:
-    resolution: {integrity: sha512-WnsKaf46uSSF/sZhwnqE4L/F89AYNMiD4YtEcYekBt9Q7nj0DiId2XH2Ng2PHM54qi5oPrQ8luuzGszqi/veig==}
-    engines: {node: '>=12'}
-    cpu: [ia32]
-    os: [win32]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/win32-ia32@0.17.19:
     resolution: {integrity: sha512-eggDKanJszUtCdlVs0RB+h35wNlb5v4TWEkq4vZcmVt5u/HiDZrTXe2bWFQUez3RgNHwx/x4sk5++4NSSicKkw==}
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     optional: true
@@ -1409,23 +1223,14 @@
     engines: {node: '>=12'}
     cpu: [ia32]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@esbuild/win32-x64@0.16.17:
-    resolution: {integrity: sha512-y+EHuSchhL7FjHgvQL/0fnnFmO4T1bhvWANX6gcnqTjtnKWbTvUMCpGnv2+t+31d7RzyEAYAd4u2fnIhHL6N/Q==}
-    engines: {node: '>=12'}
-    cpu: [x64]
-    os: [win32]
-    requiresBuild: true
-    dev: true
-    optional: true
-
   /@esbuild/win32-x64@0.17.19:
     resolution: {integrity: sha512-lAhycmKnVOuRYNtRtatQR1LPQf2oYCkRGkSFnseDAKPl8lu5SOsK/e1sXe5a0Pc5kHIHe6P2I/ilntNv2xf3cA==}
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     optional: true
@@ -1435,18 +1240,14 @@
     engines: {node: '>=12'}
     cpu: [x64]
     os: [win32]
     requiresBuild: true
     dev: true
     optional: true
 
-  /@gar/promisify@1.1.3:
-    resolution: {integrity: sha512-k2Ty1JcVojjJFwrg/ThKi2ujJ7XNLYaFGNB/bWT9wGR+oSMJHMa5w+CUq6p/pVrKeNNgA7pCqEcjSnHVoqJQFw==}
-    dev: true
-
   /@jridgewell/gen-mapping@0.3.3:
     resolution: {integrity: sha512-HLhSWOLRi875zjjMG/r+Nv0oCW8umGb0BgEhyX3dDX3egwZtB8PqLnjz3yedt8R5StBrzcg4aBpnh8UA9D1BoQ==}
     engines: {node: '>=6.0.0'}
     dependencies:
       '@jridgewell/set-array': 1.1.2
       '@jridgewell/sourcemap-codec': 1.4.15
       '@jridgewell/trace-mapping': 0.3.18
@@ -1474,14 +1275,29 @@
 
   /@jridgewell/trace-mapping@0.3.18:
     resolution: {integrity: sha512-w+niJYzMHdd7USdiH2U6869nqhD2nbfZXND5Yp93qIbEmnDNk7PD48o+YchRVpzMU7M6jVCbenTR7PA1FLQ9pA==}
     dependencies:
       '@jridgewell/resolve-uri': 3.1.0
       '@jridgewell/sourcemap-codec': 1.4.14
 
+  /@jupyter-widgets/base-manager@1.0.5(crypto@1.0.1):
+    resolution: {integrity: sha512-+pagXIXBbSq1NdqaJ8xJj52SF3t0zyUofDHVZ1bFrfWIhl5qZuLxtD16PvnqO+n1gIPLlW238Og6QuIGKOKkZQ==}
+    dependencies:
+      '@jupyter-widgets/base': 6.0.4(crypto@1.0.1)
+      '@jupyterlab/services': 6.6.4(crypto@1.0.1)
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      base64-js: 1.5.1
+      sanitize-html: 2.11.0
+    transitivePeerDependencies:
+      - bufferutil
+      - crypto
+      - encoding
+      - utf-8-validate
+    dev: true
+
   /@jupyter-widgets/base@2.0.0:
     resolution: {integrity: sha512-oL7iFmBZcx5daHJhR6r4Y+Y6E3yqwhQf6Yo7VswcRmLgDAkks56qr5a11mxzPQdgFlNYRKKmF1tW3bZCfEdWog==}
     dependencies:
       '@jupyterlab/services': 4.2.3
       '@phosphor/coreutils': 1.3.1
       '@phosphor/messaging': 1.3.0
       '@phosphor/widgets': 1.9.3
@@ -1493,59 +1309,71 @@
       lodash: 4.17.21
     transitivePeerDependencies:
       - bufferutil
       - encoding
       - utf-8-validate
     dev: false
 
-  /@jupyterlab/builder@3.6.4(crypto@1.0.1)(esbuild@0.18.6):
-    resolution: {integrity: sha512-ycTW4P7VRF+67JCb/PlJ358CBsoUYxxkiAEkR6R9QJEY0Zk4S4NuuHq2Sv87Zclpj+xlrxlnSR9WaLq8zEvR7A==}
-    hasBin: true
+  /@jupyter-widgets/base@6.0.4(crypto@1.0.1):
+    resolution: {integrity: sha512-w5KUL8q44Isp0N/ElOAJbPSgWBdeGZO5EYEcz50rfqYAUMSh2Qx0oQJYMddbRgi8b5CajGHFvcHTfvwaNDLSmA==}
     dependencies:
-      '@lumino/algorithm': 1.9.2
-      '@lumino/application': 1.31.4(crypto@1.0.1)
-      '@lumino/commands': 1.21.1(crypto@1.0.1)
+      '@jupyterlab/services': 6.6.4(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
-      '@lumino/disposable': 1.10.4
-      '@lumino/domutils': 1.8.2
-      '@lumino/dragdrop': 1.14.5(crypto@1.0.1)
       '@lumino/messaging': 1.10.3
-      '@lumino/properties': 1.8.2
-      '@lumino/signaling': 1.11.1
-      '@lumino/virtualdom': 1.14.3
       '@lumino/widgets': 1.37.2(crypto@1.0.1)
-      ajv: 6.12.6
-      commander: 6.0.0
-      css-loader: 5.2.7(webpack@5.88.0)
+      '@types/backbone': 1.4.14
+      '@types/lodash': 4.14.195
+      backbone: 1.4.0
+      jquery: 3.7.0
+      lodash: 4.17.21
+    transitivePeerDependencies:
+      - bufferutil
+      - crypto
+      - encoding
+      - utf-8-validate
+    dev: true
+
+  /@jupyterlab/builder@4.0.2(esbuild@0.18.6):
+    resolution: {integrity: sha512-b4NPnnMNkfs07jeqxD2kctsZqYGncXWTmo0VsiMeiO4P19QaRMJrigjI56SC3V6100FpQby24yDZK625CR41lg==}
+    hasBin: true
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+      '@lumino/application': 2.2.0
+      '@lumino/commands': 2.1.2
+      '@lumino/coreutils': 2.1.1
+      '@lumino/disposable': 2.1.1
+      '@lumino/domutils': 2.0.0
+      '@lumino/dragdrop': 2.1.2
+      '@lumino/messaging': 2.0.0
+      '@lumino/properties': 2.0.0
+      '@lumino/signaling': 2.1.1
+      '@lumino/virtualdom': 2.0.0
+      '@lumino/widgets': 2.2.0
+      ajv: 8.12.0
+      commander: 9.5.0
+      css-loader: 6.8.1(webpack@5.88.0)
       duplicate-package-checker-webpack-plugin: 3.0.0
-      file-loader: 6.0.0(webpack@5.88.0)
-      fs-extra: 9.1.0
+      fs-extra: 10.1.0
       glob: 7.1.7
       license-webpack-plugin: 2.3.21(webpack@5.88.0)
-      mini-css-extract-plugin: 1.3.9(webpack@5.88.0)
+      mini-css-extract-plugin: 2.7.6(webpack@5.88.0)
+      mini-svg-data-uri: 1.4.4
       path-browserify: 1.0.1
       process: 0.11.10
-      raw-loader: 4.0.2(webpack@5.88.0)
       source-map-loader: 1.0.2(webpack@5.88.0)
-      style-loader: 2.0.0(webpack@5.88.0)
+      style-loader: 3.3.3(webpack@5.88.0)
       supports-color: 7.2.0
-      svg-url-loader: 6.0.0(webpack@5.88.0)
-      terser-webpack-plugin: 4.2.3(webpack@5.88.0)
-      to-string-loader: 1.2.0
-      url-loader: 4.1.1(file-loader@6.0.0)(webpack@5.88.0)
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-      webpack-cli: 4.10.0(webpack@5.88.0)
+      terser-webpack-plugin: 5.3.9(esbuild@0.18.6)(webpack@5.88.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack-cli: 5.1.4(webpack@5.88.0)
       webpack-merge: 5.9.0
       worker-loader: 3.0.8(webpack@5.88.0)
     transitivePeerDependencies:
       - '@swc/core'
       - '@webpack-cli/generators'
-      - '@webpack-cli/migrate'
-      - bluebird
-      - crypto
       - esbuild
       - uglify-js
       - webpack-bundle-analyzer
       - webpack-dev-server
     dev: true
 
   /@jupyterlab/coreutils@3.2.0:
@@ -1560,24 +1388,58 @@
       json5: 2.2.3
       minimist: 1.2.8
       moment: 2.29.4
       path-posix: 1.0.0
       url-parse: 1.4.7
     dev: false
 
+  /@jupyterlab/coreutils@5.6.4(crypto@1.0.1):
+    resolution: {integrity: sha512-KKZcX+b4YPhoOkDKpxPXhc/QUmPNImgcsVsxceCNrznXNxLwwQcreSCMfKQ+i9Z1QayvYUETphAO5dUmfUQkjg==}
+    dependencies:
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/signaling': 1.11.1
+      minimist: 1.2.8
+      moment: 2.29.4
+      path-browserify: 1.0.1
+      url-parse: 1.5.10
+    transitivePeerDependencies:
+      - crypto
+    dev: true
+
+  /@jupyterlab/nbformat@3.6.4(crypto@1.0.1):
+    resolution: {integrity: sha512-FIXm3PjtVJOyd+og8mMBcKMgSSq5iGf11rDH9rjFzd1Uo6TwCBiKmkipyAaa8wVcB07A5ocpU0wCE/do2m24kg==}
+    dependencies:
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+    transitivePeerDependencies:
+      - crypto
+    dev: true
+
   /@jupyterlab/observables@2.4.0:
     resolution: {integrity: sha512-M/fhAnPqd6F4Zwt4IIsvHCkJmwbSw1Tko/hUXgdUQG86lPsJiTOh98sB3qwV1gtzb9oFF+kH21XsHnQZ6Yl6Pw==}
     dependencies:
       '@phosphor/algorithm': 1.2.0
       '@phosphor/coreutils': 1.3.1
       '@phosphor/disposable': 1.3.1
       '@phosphor/messaging': 1.3.0
       '@phosphor/signaling': 1.3.1
     dev: false
 
+  /@jupyterlab/observables@4.6.4(crypto@1.0.1):
+    resolution: {integrity: sha512-HqIYzHj+HYWnZTFMWr6b0GG92UfrFk7k8ihLlVm0W289Pz+0YlOBPgXhEJsTPPIm+YiICXD8WzvySXUWo92ryA==}
+    dependencies:
+      '@lumino/algorithm': 1.9.2
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/messaging': 1.10.3
+      '@lumino/signaling': 1.11.1
+    transitivePeerDependencies:
+      - crypto
+    dev: true
+
   /@jupyterlab/services@4.2.3:
     resolution: {integrity: sha512-bCPq1j8+qU5pCzsaKvT39e8Aj4snFCchSAoVr12wAOlp0gQZYpUZAgaFhnYtawGo44aBfEYWhQuW5UPol/XUag==}
     dependencies:
       '@jupyterlab/coreutils': 3.2.0
       '@jupyterlab/observables': 2.4.0
       '@phosphor/algorithm': 1.2.0
       '@phosphor/coreutils': 1.3.1
@@ -1587,107 +1449,234 @@
       ws: 7.5.9
     transitivePeerDependencies:
       - bufferutil
       - encoding
       - utf-8-validate
     dev: false
 
-  /@ljharb/has-package-exports-patterns@0.0.2:
-    resolution: {integrity: sha512-4/RWEeXDO6bocPONheFe6gX/oQdP/bEpv0oL4HqjPP5DCenBSt0mHgahppY49N0CpsaqffdwPq+TlX9CYOq2Dw==}
+  /@jupyterlab/services@6.6.4(crypto@1.0.1):
+    resolution: {integrity: sha512-qtPnCfPWyKvQmr5w/YLO3+Tif1fYkJvCAufLljiWpAORFF06LvURbP9Lb+GOsXS9VHZQTcXLBv8sdlQSbj5qNg==}
+    dependencies:
+      '@jupyterlab/coreutils': 5.6.4(crypto@1.0.1)
+      '@jupyterlab/nbformat': 3.6.4(crypto@1.0.1)
+      '@jupyterlab/observables': 4.6.4(crypto@1.0.1)
+      '@jupyterlab/settingregistry': 3.6.4(crypto@1.0.1)
+      '@jupyterlab/statedb': 3.6.4(crypto@1.0.1)
+      '@lumino/algorithm': 1.9.2
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/polling': 1.11.4(crypto@1.0.1)
+      '@lumino/signaling': 1.11.1
+      node-fetch: 2.6.11
+      ws: 7.5.9
+    transitivePeerDependencies:
+      - bufferutil
+      - crypto
+      - encoding
+      - utf-8-validate
+    dev: true
 
-  /@lumino/algorithm@1.9.2:
-    resolution: {integrity: sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==}
+  /@jupyterlab/settingregistry@3.6.4(crypto@1.0.1):
+    resolution: {integrity: sha512-DD3qrd2X6fvkC67MlNkPlHZBh14mecu5+fkE8KBbAQwPZsn9E/JdOVbNVc3sd5Jl/hzobGdtcMhQUTfK46g6ow==}
+    dependencies:
+      '@jupyterlab/statedb': 3.6.4(crypto@1.0.1)
+      '@lumino/commands': 1.21.1(crypto@1.0.1)
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/signaling': 1.11.1
+      ajv: 6.12.6
+      json5: 2.2.3
+    transitivePeerDependencies:
+      - crypto
     dev: true
 
-  /@lumino/application@1.31.4(crypto@1.0.1):
-    resolution: {integrity: sha512-dOSsDJ1tXOxC3fnSHvtDQK5RcICLEVPtO19HeCGwurb5W2ZZ55SZT2b5jZu6V/v8lGdtkNbr1RJltRpJRSRb/A==}
+  /@jupyterlab/statedb@3.6.4(crypto@1.0.1):
+    resolution: {integrity: sha512-sfbAMU7wTf8pzdyW1TLOUzdki1wu7amtDD9JgrD6RrUXTve9QaiKjC+FenFEBPMzogWDogZGAtBEoTLMY+k3pg==}
     dependencies:
       '@lumino/commands': 1.21.1(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
-      '@lumino/widgets': 1.37.2(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/properties': 1.8.2
+      '@lumino/signaling': 1.11.1
     transitivePeerDependencies:
       - crypto
     dev: true
 
+  /@ljharb/has-package-exports-patterns@0.0.2:
+    resolution: {integrity: sha512-4/RWEeXDO6bocPONheFe6gX/oQdP/bEpv0oL4HqjPP5DCenBSt0mHgahppY49N0CpsaqffdwPq+TlX9CYOq2Dw==}
+
+  /@lumino/algorithm@1.9.2:
+    resolution: {integrity: sha512-Z06lp/yuhz8CtIir3PNTGnuk7909eXt4ukJsCzChsGuot2l5Fbs96RJ/FOHgwCedaX74CtxPjXHXoszFbUA+4A==}
+    dev: true
+
+  /@lumino/algorithm@2.0.0:
+    resolution: {integrity: sha512-SwM/8U1zlMWMJj00wTCThdTUit9zap2Xghuo4uUxvZ+mfog5b1UIk2j1dP8TPpzEXHCDPEb85s2/ERo1tee3Dw==}
+    dev: true
+
+  /@lumino/application@2.2.0:
+    resolution: {integrity: sha512-hivdDH2/YiOLtvsfY60GSUc+d6Rxh07dz6wp8ZnoalFmzdqqI8mcW4H30PchVdmqxXK0qxZIjLlP9A3fOu/xIw==}
+    dependencies:
+      '@lumino/commands': 2.1.2
+      '@lumino/coreutils': 2.1.1
+      '@lumino/widgets': 2.2.0
+    dev: true
+
   /@lumino/collections@1.9.3:
     resolution: {integrity: sha512-2i2Wf1xnfTgEgdyKEpqM16bcYRIhUOGCDzaVCEZACVG9R1CgYwOe3zfn71slBQOVSjjRgwYrgLXu4MBpt6YK+g==}
     dependencies:
       '@lumino/algorithm': 1.9.2
     dev: true
 
+  /@lumino/collections@2.0.0:
+    resolution: {integrity: sha512-uQvsRaQ8R8x/fTI2mk4+Z3EdUBDg/RtnqePDKtggWuu+BEjfk6vJ1jo42OGvEcurvhrrIZhFcpQJhtC+nNk4lA==}
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+    dev: true
+
   /@lumino/commands@1.21.1(crypto@1.0.1):
     resolution: {integrity: sha512-d1zJmwz5bHU0BM/Rl3tRdZ7/WgXnFB0bM7x7Bf0XDlmX++jnU9k0j3mh6/5JqCGLmIApKCRwVqSaV7jPmSJlcQ==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
       '@lumino/domutils': 1.8.2
       '@lumino/keyboard': 1.8.2
       '@lumino/signaling': 1.11.1
       '@lumino/virtualdom': 1.14.3
     transitivePeerDependencies:
       - crypto
     dev: true
 
+  /@lumino/commands@2.1.2:
+    resolution: {integrity: sha512-wdA7kx2z0oygD44yQo5Tlk+yViKqmjTqwQSg2jfKfGyVOrwM3i1NXdZ8ntIV8WQIHmg24D2WqElwjUq5G7bGlw==}
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+      '@lumino/coreutils': 2.1.1
+      '@lumino/disposable': 2.1.1
+      '@lumino/domutils': 2.0.0
+      '@lumino/keyboard': 2.0.0
+      '@lumino/signaling': 2.1.1
+      '@lumino/virtualdom': 2.0.0
+    dev: true
+
   /@lumino/coreutils@1.12.1(crypto@1.0.1):
     resolution: {integrity: sha512-JLu3nTHzJk9N8ohZ85u75YxemMrmDzJdNgZztfP7F7T7mxND3YVNCkJG35a6aJ7edu1sIgCjBxOvV+hv27iYvQ==}
     peerDependencies:
       crypto: 1.0.1
     dependencies:
       crypto: 1.0.1
     dev: true
 
+  /@lumino/coreutils@2.1.1:
+    resolution: {integrity: sha512-OmEzvphZC/EVpFfwBkmcuzNwKXvkij6gJo1mbf4/tZMC1/8NO3aVnjK1FsgC0TlaGwMD1BLIFgGay2mC/I/cyQ==}
+    dev: true
+
   /@lumino/disposable@1.10.4:
     resolution: {integrity: sha512-4ZxyYcyzUS+ZeB2KAH9oAH3w0DUUceiVr+FIZHZ2TAYGWZI/85WlqJtfm0xjwEpCwLLW1TDqJrISuZu3iMmVMA==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/signaling': 1.11.1
     dev: true
 
+  /@lumino/disposable@2.1.1:
+    resolution: {integrity: sha512-zGl5hDDgDgPlrCN8b37gmNRjmYrTXnVq4WaseRtEgjj/en+gHLQW7sgTzkLgPj5rFaVETPkyrDTQ5uZVewFOAw==}
+    dependencies:
+      '@lumino/signaling': 2.1.1
+    dev: true
+
   /@lumino/domutils@1.8.2:
     resolution: {integrity: sha512-QIpMfkPJrs4GrWBuJf2Sn1fpyVPmvqUUAeD8xAQo8+4V5JAT0vUDLxZ9HijefMgNCi3+Bs8Z3lQwRCrz+cFP1A==}
     dev: true
 
+  /@lumino/domutils@2.0.0:
+    resolution: {integrity: sha512-GYsz6CS6Gd+7r9IBe/0m+3/xAuOKrjfiXwWt7OLsOM1icRv93yS+gxleCLp2+LSwoqU90sqfav+uYABtPkA4QA==}
+    dev: true
+
   /@lumino/dragdrop@1.14.5(crypto@1.0.1):
     resolution: {integrity: sha512-LC5xB82+xGF8hFyl716TMpV32OIMIMl+s3RU1PaqDkD6B7PkgiVk6NkJ4X9/GcEvl2igkvlGQt/3L7qxDAJNxw==}
     dependencies:
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
     transitivePeerDependencies:
       - crypto
     dev: true
 
+  /@lumino/dragdrop@2.1.2:
+    resolution: {integrity: sha512-89Sc2HpGHQnzQx4/A/oVmS1uOfy4YjRJtNvdr/7zoUeJTib9vxKvlzrsRopLqvmyQPzJMnulEkiWuWsgzNnLeA==}
+    dependencies:
+      '@lumino/coreutils': 2.1.1
+      '@lumino/disposable': 2.1.1
+    dev: true
+
   /@lumino/keyboard@1.8.2:
     resolution: {integrity: sha512-Dy+XqQ1wXbcnuYtjys5A0pAqf4SpAFl9NY6owyIhXAo0Va7w3LYp3jgiP1xAaBAwMuUppiUAfrbjrysZuZ625g==}
     dev: true
 
+  /@lumino/keyboard@2.0.0:
+    resolution: {integrity: sha512-bX42YYLJPuATGKH7DQaQrji28HXJJVU2QwAK/vrTiLpiZD28x6Q0QhwKaP5x4wNH8ikhwR9jRP7b9PNNtUGGfg==}
+    dev: true
+
   /@lumino/messaging@1.10.3:
     resolution: {integrity: sha512-F/KOwMCdqvdEG8CYAJcBSadzp6aI7a47Fr60zAKGqZATSRRRV41q53iXU7HjFPqQqQIvdn9Z7J32rBEAyQAzww==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/collections': 1.9.3
     dev: true
 
+  /@lumino/messaging@2.0.0:
+    resolution: {integrity: sha512-B8cMK36hrkngntsdLNic3GEPfAk4qp6HIYWDrRSC1z7pjgjH8EEKUOO2MNNYNKNq3Hzpog7FM0nhT1tLqoFAYA==}
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+      '@lumino/collections': 2.0.0
+    dev: true
+
+  /@lumino/polling@1.11.4(crypto@1.0.1):
+    resolution: {integrity: sha512-yC7JLssj3mqVK6TsYj7dg4AG0rcsC42YtpoDLtz9yzO84Q5flQUfmjAPQB6oPA6wZOlISs3iasF+uO2w1ls5jg==}
+    dependencies:
+      '@lumino/coreutils': 1.12.1(crypto@1.0.1)
+      '@lumino/disposable': 1.10.4
+      '@lumino/signaling': 1.11.1
+    transitivePeerDependencies:
+      - crypto
+    dev: true
+
   /@lumino/properties@1.8.2:
     resolution: {integrity: sha512-EkjI9Cw8R0U+xC9HxdFSu7X1tz1H1vKu20cGvJ2gU+CXlMB1DvoYJCYxCThByHZ+kURTAap4SE5x8HvKwNPbig==}
     dev: true
 
+  /@lumino/properties@2.0.0:
+    resolution: {integrity: sha512-2TZE3gu1EZj5x2kEUBmr1aSemtgkkGlLkd3CwK0zjlukUhdrONveLsOX/Hr8+EnXv070i5lSr+9PzNNVqs9vPg==}
+    dev: true
+
   /@lumino/signaling@1.11.1:
     resolution: {integrity: sha512-YCUmgw08VoyMN5KxzqPO3KMx+cwdPv28tAN06C0K7Q/dQf+oufb1XocuhZb5selTrTmmuXeizaYxgLIQGdS1fA==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/properties': 1.8.2
     dev: true
 
+  /@lumino/signaling@2.1.1:
+    resolution: {integrity: sha512-EUPJlC/kis5DEPA4UxsJRPidGk4qcgS+rfQlYfGfA4Z6vR8nzcwU9WE0UIWdqo6GN7cLWR8lGLzZzyIGY3+qiA==}
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+      '@lumino/coreutils': 2.1.1
+    dev: true
+
   /@lumino/virtualdom@1.14.3:
     resolution: {integrity: sha512-5joUC1yuxeXbpfbSBm/OR8Mu9HoTo6PDX0RKqzlJ9o97iml7zayFN/ynzcxScKGQAo9iaXOY8uVIvGUT8FnsGw==}
     dependencies:
       '@lumino/algorithm': 1.9.2
     dev: true
 
+  /@lumino/virtualdom@2.0.0:
+    resolution: {integrity: sha512-N+Q4+ZcoaeQUb4cwxSzyy/DSuiCdHAtrGegrRo1M2KChKKa9DoyuQy3H9jZItrPpqh5VIQDu3UHMY0BsiwdgUA==}
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+    dev: true
+
   /@lumino/widgets@1.37.2(crypto@1.0.1):
     resolution: {integrity: sha512-NHKu1NBDo6ETBDoNrqSkornfUCwc8EFFzw6+LWBfYVxn2PIwciq2SdiJGEyNqL+0h/A9eVKb5ui5z4cwpRekmQ==}
     dependencies:
       '@lumino/algorithm': 1.9.2
       '@lumino/commands': 1.21.1(crypto@1.0.1)
       '@lumino/coreutils': 1.12.1(crypto@1.0.1)
       '@lumino/disposable': 1.10.4
@@ -1698,14 +1687,30 @@
       '@lumino/properties': 1.8.2
       '@lumino/signaling': 1.11.1
       '@lumino/virtualdom': 1.14.3
     transitivePeerDependencies:
       - crypto
     dev: true
 
+  /@lumino/widgets@2.2.0:
+    resolution: {integrity: sha512-nQ5UXjcl+Tvddeev0We5aoW2erm5KffKCJZEo6/1i4t2cj90v2ndqtXtbiCjeQOBDojIH6u1BVPtUExTh00cbA==}
+    dependencies:
+      '@lumino/algorithm': 2.0.0
+      '@lumino/commands': 2.1.2
+      '@lumino/coreutils': 2.1.1
+      '@lumino/disposable': 2.1.1
+      '@lumino/domutils': 2.0.0
+      '@lumino/dragdrop': 2.1.2
+      '@lumino/keyboard': 2.0.0
+      '@lumino/messaging': 2.0.0
+      '@lumino/properties': 2.0.0
+      '@lumino/signaling': 2.1.1
+      '@lumino/virtualdom': 2.0.0
+    dev: true
+
   /@manypkg/find-root@1.1.0:
     resolution: {integrity: sha512-mki5uBvhHzO8kYYix/WRy2WX8S3B5wdVSc9D6KcU5lQNglP2yt58/VfLuAK49glRXChosY8ap2oJ1qgma3GUVA==}
     dependencies:
       '@babel/runtime': 7.22.5
       '@types/node': 12.20.55
       find-up: 4.1.0
       fs-extra: 8.1.0
@@ -1760,30 +1765,14 @@
   /@nodelib/fs.walk@1.2.8:
     resolution: {integrity: sha512-oGB+UxlgWcgQkgwo8GcEGwemoTFt3FIO9ababBmaGwXIoBKZ+GTy0pP185beGg7Llih/NSHSV2XAs1lnznocSg==}
     engines: {node: '>= 8'}
     dependencies:
       '@nodelib/fs.scandir': 2.1.5
       fastq: 1.15.0
 
-  /@npmcli/fs@1.1.1:
-    resolution: {integrity: sha512-8KG5RD0GVP4ydEzRn/I4BNDuxDtqVbOdm8675T49OIG/NGhaK0pjPX7ZcDlvKYbA+ulvVK3ztfcF4uBdOxuJbQ==}
-    dependencies:
-      '@gar/promisify': 1.1.3
-      semver: 7.5.2
-    dev: true
-
-  /@npmcli/move-file@1.1.2:
-    resolution: {integrity: sha512-1SUf/Cg2GzGDyaf15aR9St9TWlb+XvbZXWpDx8YKs7MLzMH/BCeopv+y9vzrzgkfykCGuWOlSu3mZhj2+FQcrg==}
-    engines: {node: '>=10'}
-    deprecated: This functionality has been moved to @npmcli/fs
-    dependencies:
-      mkdirp: 1.0.4
-      rimraf: 3.0.2
-    dev: true
-
   /@phosphor/algorithm@1.2.0:
     resolution: {integrity: sha512-C9+dnjXyU2QAkWCW6QVDGExk4hhwxzAKf5/FIuYlHAI9X5vFv99PYm0EREDxX1PbMuvfFBZhPNu0PvuSDQ7sFA==}
     dev: false
 
   /@phosphor/collections@1.2.0:
     resolution: {integrity: sha512-T9/0EjSuY6+ga2LIFRZ0xupciOR3Qnyy8Q95lhGTC0FXZUFwC8fl9e8On6IcwasCszS+1n8dtZUWSIynfgdpzw==}
     dependencies:
@@ -1934,14 +1923,21 @@
       '@babel/types': 7.22.5
 
   /@types/babel__traverse@7.20.1:
     resolution: {integrity: sha512-MitHFXnhtgwsGZWtT68URpOvLN4EREih1u3QtQiN4VdAxWKRVvGCSvw/Qth0M0Qq3pJpnGOu5JaM/ydK7OGbqg==}
     dependencies:
       '@babel/types': 7.22.5
 
+  /@types/backbone@1.4.14:
+    resolution: {integrity: sha512-85ldQ99fiYTJFBlZuAJRaCdvTZKZ2p1fSs3fVf+6Ub6k1X0g0hNJ0qJ/2FOByyyAQYLtbEz3shX5taKQfBKBDw==}
+    dependencies:
+      '@types/jquery': 3.5.16
+      '@types/underscore': 1.11.5
+    dev: true
+
   /@types/backbone@1.4.15:
     resolution: {integrity: sha512-WWeKtYlsIMtDyLbbhkb96taJMEbfQBnuz7yw1u0pkphCOtksemoWhIXhK74VRCY9hbjnsH3rsJu2uUiFtnsEYg==}
     dependencies:
       '@types/jquery': 3.5.16
       '@types/underscore': 1.11.5
     dev: false
 
@@ -1998,26 +1994,24 @@
       ci-info: 3.8.0
     dev: true
 
   /@types/jquery@3.5.16:
     resolution: {integrity: sha512-bsI7y4ZgeMkmpG9OM710RRzDFp+w4P1RGiIt30C1mSBT+ExCleeh4HObwgArnDFELmRrOpXgSYN9VF1hj+f1lw==}
     dependencies:
       '@types/sizzle': 2.3.3
-    dev: false
 
   /@types/json-schema@7.0.12:
     resolution: {integrity: sha512-Hr5Jfhc9eYOQNPYO5WLDq/n4jqijdHNlDXjuAQkkt+mWdQR+XJToOHrsD4cPaMXpn6KO7y2+wM8AZEs8VpBLVA==}
     dev: true
 
   /@types/json5@0.0.30:
     resolution: {integrity: sha512-sqm9g7mHlPY/43fcSNrCYfOeX9zkTTK+euO5E6+CVijSMm5tTjkVdwdqRkY3ljjIAf8679vps5jKUoJBCLsMDA==}
 
   /@types/lodash@4.14.195:
     resolution: {integrity: sha512-Hwx9EUgdwf2GLarOjQp5ZH8ZmblzcbTBC2wtQWNKARBSxM9ezRIAUpeDTgoQRAFB0+8CNWXVA9+MaSOzOF3nPg==}
-    dev: false
 
   /@types/mdast@3.0.11:
     resolution: {integrity: sha512-Y/uImid8aAwrEA24/1tcRZwpxX3pIFTSilcNDKSPn+Y2iDywSEachzRuvgAYYLR3wpGXAsMbv5lvKLDZLeYPAw==}
     dependencies:
       '@types/unist': 2.0.6
 
   /@types/mdx@2.0.5:
@@ -2077,23 +2071,21 @@
 
   /@types/semver@6.2.3:
     resolution: {integrity: sha512-KQf+QAMWKMrtBMsB8/24w53tEsxllMj6TuA80TT/5igJalLI/zm0L3oXRbIAl4Ohfc85gyHX/jhMwsVkmhLU4A==}
     dev: true
 
   /@types/sizzle@2.3.3:
     resolution: {integrity: sha512-JYM8x9EGF163bEyhdJBpR2QX1R5naCJHC8ucJylJ3w9/CVBaskdQ8WqBf8MmQrd1kRvp/a4TS8HJ+bxzR7ZJYQ==}
-    dev: false
 
   /@types/source-list-map@0.1.2:
     resolution: {integrity: sha512-K5K+yml8LTo9bWJI/rECfIPrGgxdpeNbj+d53lwN4QjW1MCwlkhUms+gtdzigTeUyBr09+u8BwOIY3MXvHdcsA==}
     dev: true
 
   /@types/underscore@1.11.5:
     resolution: {integrity: sha512-b8e//LrIlhoXaaBcMC0J/s2/lIF9y5VJYKqbW4nA+tW/nqqDk1Dacd1ULLT7zgGsKs7PGbSnqCPzqEniZ0RxYg==}
-    dev: false
 
   /@types/unist@2.0.6:
     resolution: {integrity: sha512-PBjIUxZHOuj0R15/xuwJYjFi+KZdNFrehocChv4g5hu6aFroHue8m0lBP0POdK2nKzbw0cgV1mws8+V/JAcEkQ==}
 
   /@types/webpack-sources@0.1.9:
     resolution: {integrity: sha512-bvzMnzqoK16PQIC8AYHNdW45eREJQMd6WG/msQWX5V2+vZmODCOPb4TJcbgRljTZZTwTM4wUMcsI8FftNA7new==}
     dependencies:
@@ -2258,43 +2250,49 @@
   /@webassemblyjs/wast-printer@1.11.6:
     resolution: {integrity: sha512-JM7AhRcE+yW2GWYaKeHL5vt4xqee5N2WcezptmgyhNS+ScggqcT1OtXykhAb13Sn5Yas0j2uv9tHgrjwvzAP4A==}
     dependencies:
       '@webassemblyjs/ast': 1.11.6
       '@xtuc/long': 4.2.2
     dev: true
 
-  /@webpack-cli/configtest@1.2.0(webpack-cli@4.10.0)(webpack@5.88.0):
-    resolution: {integrity: sha512-4FB8Tj6xyVkyqjj1OaTqCjXYULB9FMkqQ8yGrZjRDrYh0nOE+7Lhs45WioWQQMV+ceFlE368Ukhe6xdvJM9Egg==}
+  /@webpack-cli/configtest@2.1.1(webpack-cli@5.1.4)(webpack@5.88.0):
+    resolution: {integrity: sha512-wy0mglZpDSiSS0XHrVR+BAdId2+yxPSoJW8fsna3ZpYSlufjvxnP4YbKTCBZnNIcGN4r6ZPXV55X4mYExOfLmw==}
+    engines: {node: '>=14.15.0'}
     peerDependencies:
-      webpack: 4.x.x || 5.x.x
-      webpack-cli: 4.x.x
+      webpack: 5.x.x
+      webpack-cli: 5.x.x
     dependencies:
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-      webpack-cli: 4.10.0(webpack@5.88.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack-cli: 5.1.4(webpack@5.88.0)
     dev: true
 
-  /@webpack-cli/info@1.5.0(webpack-cli@4.10.0):
-    resolution: {integrity: sha512-e8tSXZpw2hPl2uMJY6fsMswaok5FdlGNRTktvFk2sD8RjH0hE2+XistawJx1vmKteh4NmGmNUrp+Tb2w+udPcQ==}
+  /@webpack-cli/info@2.0.2(webpack-cli@5.1.4)(webpack@5.88.0):
+    resolution: {integrity: sha512-zLHQdI/Qs1UyT5UBdWNqsARasIA+AaF8t+4u2aS2nEpBQh2mWIVb8qAklq0eUENnC5mOItrIB4LiS9xMtph18A==}
+    engines: {node: '>=14.15.0'}
     peerDependencies:
-      webpack-cli: 4.x.x
+      webpack: 5.x.x
+      webpack-cli: 5.x.x
     dependencies:
-      envinfo: 7.9.0
-      webpack-cli: 4.10.0(webpack@5.88.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack-cli: 5.1.4(webpack@5.88.0)
     dev: true
 
-  /@webpack-cli/serve@1.7.0(webpack-cli@4.10.0):
-    resolution: {integrity: sha512-oxnCNGj88fL+xzV+dacXs44HcDwf1ovs3AuEzvP7mqXw7fQntqIhQ1BRmynh4qEKQSSSRSWVyXRjmTbZIX9V2Q==}
+  /@webpack-cli/serve@2.0.5(webpack-cli@5.1.4)(webpack@5.88.0):
+    resolution: {integrity: sha512-lqaoKnRYBdo1UgDX8uF24AfGMifWK19TxPmM5FHc2vAGxrJ/qtyUyFBWoY1tISZdelsQ5fBcOusifo5o5wSJxQ==}
+    engines: {node: '>=14.15.0'}
     peerDependencies:
-      webpack-cli: 4.x.x
+      webpack: 5.x.x
+      webpack-cli: 5.x.x
       webpack-dev-server: '*'
     peerDependenciesMeta:
       webpack-dev-server:
         optional: true
     dependencies:
-      webpack-cli: 4.10.0(webpack@5.88.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+      webpack-cli: 5.1.4(webpack@5.88.0)
     dev: true
 
   /@xtuc/ieee754@1.2.0:
     resolution: {integrity: sha512-DX8nKgqcGwsc0eJSqYt5lwP4DH5FlHnmuWWBRy7X0NcaGR0ZtuyeESgMwTYVEtxmsNGY+qit4QYT/MIYTOTPeA==}
     dev: true
 
   /@xtuc/long@4.2.2:
@@ -2327,55 +2325,76 @@
     dev: true
 
   /acorn@8.9.0:
     resolution: {integrity: sha512-jaVNAFBHNLXspO543WnNNPZFRtavh3skAkITqD0/2aeMkKZTN+254PyhwxFYrk3vQ1xfY+2wbesJMs/JC8/PwQ==}
     engines: {node: '>=0.4.0'}
     hasBin: true
 
-  /aggregate-error@3.1.0:
-    resolution: {integrity: sha512-4I7Td01quW/RpocfNayFdFVk1qSuoh0E7JrbRJ16nH01HhKFQ88INq9Sd+nd72zqRySlr9BmDA8xlEJ6vJMrYA==}
-    engines: {node: '>=8'}
+  /ajv-formats@2.1.1(ajv@8.12.0):
+    resolution: {integrity: sha512-Wx0Kx52hxE7C18hkMEggYlEifqWZtYaRgouJor+WMdPnQyEK13vgEWyVNup7SoeeoLMsr4kf5h6dOW11I15MUA==}
+    peerDependencies:
+      ajv: ^8.0.0
+    peerDependenciesMeta:
+      ajv:
+        optional: true
     dependencies:
-      clean-stack: 2.2.0
-      indent-string: 4.0.0
+      ajv: 8.12.0
     dev: true
 
   /ajv-keywords@3.5.2(ajv@6.12.6):
     resolution: {integrity: sha512-5p6WTN0DdTGVQk6VjcEju19IgaHudalcfabD7yhDGeA6bcQnmL+CpveLJq/3hvfwd1aof6L386Ougkx6RfyMIQ==}
     peerDependencies:
       ajv: ^6.9.1
     dependencies:
       ajv: 6.12.6
     dev: true
 
+  /ajv-keywords@5.1.0(ajv@8.12.0):
+    resolution: {integrity: sha512-YCS/JNFAUyr5vAuhk1DWm1CBxRHW9LbJ2ozWeemrIqpbsqKjHVxYPyi5GC0rjZIT5JxJ3virVTS8wk4i/Z+krw==}
+    peerDependencies:
+      ajv: ^8.8.2
+    dependencies:
+      ajv: 8.12.0
+      fast-deep-equal: 3.1.3
+    dev: true
+
   /ajv@6.12.6:
     resolution: {integrity: sha512-j3fVLgvTo527anyYyJOGTYJbG+vnnQYvE0m5mmkc1TK+nxAppkCLMIL0aZ4dblVCNoGShhm+kzE4ZUykBoMg4g==}
     dependencies:
       fast-deep-equal: 3.1.3
       fast-json-stable-stringify: 2.1.0
       json-schema-traverse: 0.4.1
       uri-js: 4.4.1
 
-  /algoliasearch@4.17.2:
-    resolution: {integrity: sha512-VFu43JJNYIW74awp7oeQcQsPcxOhd8psqBDTfyNO2Zt6L1NqnNMTVnaIdQ+8dtKqUDBqQZp0szPxECvX8CK2Fg==}
+  /ajv@8.12.0:
+    resolution: {integrity: sha512-sRu1kpcO9yLtYxBKvqfTeh9KzZEwO3STyX1HT+4CaDzC6HpTGYhIhPIzj9XuKU7KYDwnaeh5hcOwjy1QuJzBPA==}
     dependencies:
-      '@algolia/cache-browser-local-storage': 4.17.2
-      '@algolia/cache-common': 4.17.2
-      '@algolia/cache-in-memory': 4.17.2
-      '@algolia/client-account': 4.17.2
-      '@algolia/client-analytics': 4.17.2
-      '@algolia/client-common': 4.17.2
-      '@algolia/client-personalization': 4.17.2
-      '@algolia/client-search': 4.17.2
-      '@algolia/logger-common': 4.17.2
-      '@algolia/logger-console': 4.17.2
-      '@algolia/requester-browser-xhr': 4.17.2
-      '@algolia/requester-common': 4.17.2
-      '@algolia/requester-node-http': 4.17.2
-      '@algolia/transporter': 4.17.2
+      fast-deep-equal: 3.1.3
+      json-schema-traverse: 1.0.0
+      require-from-string: 2.0.2
+      uri-js: 4.4.1
+    dev: true
+
+  /algoliasearch@4.18.0:
+    resolution: {integrity: sha512-pCuVxC1SVcpc08ENH32T4sLKSyzoU7TkRIDBMwSLfIiW+fq4znOmWDkAygHZ6pRcO9I1UJdqlfgnV7TRj+MXrA==}
+    dependencies:
+      '@algolia/cache-browser-local-storage': 4.18.0
+      '@algolia/cache-common': 4.18.0
+      '@algolia/cache-in-memory': 4.18.0
+      '@algolia/client-account': 4.18.0
+      '@algolia/client-analytics': 4.18.0
+      '@algolia/client-common': 4.18.0
+      '@algolia/client-personalization': 4.18.0
+      '@algolia/client-search': 4.18.0
+      '@algolia/logger-common': 4.18.0
+      '@algolia/logger-console': 4.18.0
+      '@algolia/requester-browser-xhr': 4.18.0
+      '@algolia/requester-common': 4.18.0
+      '@algolia/requester-node-http': 4.18.0
+      '@algolia/transporter': 4.18.0
     dev: false
 
   /ansi-align@3.0.1:
     resolution: {integrity: sha512-IOfwwBF5iczOjp/WeY4YxyjqAFMQoZufdQWDd19SEExbVLNXqvpzSJ/M7Za4/sCPmQ0+GRquoA7bGcINcxew6w==}
     dependencies:
       string-width: 4.2.3
 
@@ -2525,15 +2544,15 @@
       mime: 3.0.0
       ora: 6.3.1
       p-limit: 4.0.0
       path-to-regexp: 6.2.1
       preferred-pm: 3.0.3
       prompts: 2.4.2
       rehype: 12.0.1
-      semver: 7.5.2
+      semver: 7.5.3
       server-destroy: 1.0.1
       shiki: 0.14.1
       slash: 4.0.0
       string-width: 5.1.2
       strip-ansi: 7.1.0
       supports-esm: 1.0.0
       tsconfig-resolver: 3.0.1
@@ -2549,28 +2568,23 @@
       - less
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
 
-  /at-least-node@1.0.0:
-    resolution: {integrity: sha512-+q/t7Ekv1EDY2l6Gda6LLiX14rU9TV20Wa3ofeQmwPFZbOMo9DXrLbOjFaaclkXKWidIaopwAObQDqwWtGUjqg==}
-    engines: {node: '>= 4.0.0'}
-    dev: true
-
   /autoprefixer@10.4.14(postcss@8.4.24):
     resolution: {integrity: sha512-FQzyfOsTlwVzjHxKEqRIAdJx9niO6VCBCoEwax/VLSoQF29ggECcPuBqUMZ+u8jCZOPSy8b8/8KnuFbp0SaFZQ==}
     engines: {node: ^10 || ^12 || >=14}
     hasBin: true
     peerDependencies:
       postcss: ^8.1.0
     dependencies:
       browserslist: 4.21.9
-      caniuse-lite: 1.0.30001506
+      caniuse-lite: 1.0.30001507
       fraction.js: 4.2.0
       normalize-range: 0.1.2
       picocolors: 1.0.0
       postcss: 8.4.24
       postcss-value-parser: 4.2.0
     dev: false
 
@@ -2592,14 +2606,20 @@
 
   /backbone@1.2.3:
     resolution: {integrity: sha512-1/eXj4agG79UDN7TWnZXcGD6BJrBwLZKCX7zYcBIy9jWf4mrtVkw7IE1VOYFnrKahsmPF9L55Tib9IQRvk027w==}
     dependencies:
       underscore: 1.13.6
     dev: false
 
+  /backbone@1.4.0:
+    resolution: {integrity: sha512-RLmDrRXkVdouTg38jcgHhyQ/2zjg7a8E6sz2zxfz21Hh17xDJYUHBZimVIt5fUyS8vbfpeSmTL3gUjTEvUV3qQ==}
+    dependencies:
+      underscore: 1.13.6
+    dev: true
+
   /bail@2.0.2:
     resolution: {integrity: sha512-0xO6mYd7JB2YesxDKplafRpsiOzPt9V02ddPCLbY1xYGPOX24NTyN50qnUxgCPcSoYMhKpAuBTjQoRZCAkUDRw==}
 
   /balanced-match@1.0.2:
     resolution: {integrity: sha512-3oSeUO0TMV67hN1AmbXsK4yaqU7tjiHlbxRDZOpH0KW9+CeX4bRAaX0Anxt0tx2MrpRpWwQaPwIlISEJhYU5Pw==}
 
   /base64-js@1.5.1:
@@ -2679,16 +2699,16 @@
     dev: true
 
   /browserslist@4.21.9:
     resolution: {integrity: sha512-M0MFoZzbUrRU4KNfCrDLnvyE7gub+peetoTid3TBIqtunaDJyXlwhakT+/VkvSXcfIzFfK/nkCs4nmyTmxdNSg==}
     engines: {node: ^6 || ^7 || ^8 || ^9 || ^10 || ^11 || ^12 || >=13.7}
     hasBin: true
     dependencies:
-      caniuse-lite: 1.0.30001506
-      electron-to-chromium: 1.4.437
+      caniuse-lite: 1.0.30001507
+      electron-to-chromium: 1.4.439
       node-releases: 2.0.12
       update-browserslist-db: 1.0.11(browserslist@4.21.9)
 
   /buffer-from@1.1.2:
     resolution: {integrity: sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==}
     dev: true
 
@@ -2711,40 +2731,14 @@
       streamsearch: 1.1.0
 
   /cac@6.7.14:
     resolution: {integrity: sha512-b6Ilus+c3RrdDk+JhLKUAQfzzgLEPy6wcXqS7f/xe1EETvsDP6GORG7SFuOs6cID5YkqchW/LXZbX5bc8j7ZcQ==}
     engines: {node: '>=8'}
     dev: true
 
-  /cacache@15.3.0:
-    resolution: {integrity: sha512-VVdYzXEn+cnbXpFgWs5hTT7OScegHVmLhJIR8Ufqk3iFD6A6j5iSX1KuBTfNEv4tdJWE2PzA6IVFtcLC7fN9wQ==}
-    engines: {node: '>= 10'}
-    dependencies:
-      '@npmcli/fs': 1.1.1
-      '@npmcli/move-file': 1.1.2
-      chownr: 2.0.0
-      fs-minipass: 2.1.0
-      glob: 7.1.7
-      infer-owner: 1.0.4
-      lru-cache: 6.0.0
-      minipass: 3.3.6
-      minipass-collect: 1.0.2
-      minipass-flush: 1.0.5
-      minipass-pipeline: 1.2.4
-      mkdirp: 1.0.4
-      p-map: 4.0.0
-      promise-inflight: 1.0.1
-      rimraf: 3.0.2
-      ssri: 8.0.1
-      tar: 6.1.15
-      unique-filename: 1.1.1
-    transitivePeerDependencies:
-      - bluebird
-    dev: true
-
   /call-bind@1.0.2:
     resolution: {integrity: sha512-7O+FbCihrB5WGbFYesctwmTKae6rOiIzmz1icreWJ+0aA7LJfuqhEso2T9ncpcFtzMQtzXf2QGGueWJGTYsqrA==}
     dependencies:
       function-bind: 1.1.1
       get-intrinsic: 1.2.1
     dev: true
 
@@ -2767,16 +2761,16 @@
     engines: {node: '>=6'}
     dev: true
 
   /camelcase@6.3.0:
     resolution: {integrity: sha512-Gmy6FhYlCY7uOElZUSbxo2UCDH8owEk996gkbrpsgGtrJLM3J7jGxl9Ic7Qwwj4ivOE5AWZWRMecDdF7hqGjFA==}
     engines: {node: '>=10'}
 
-  /caniuse-lite@1.0.30001506:
-    resolution: {integrity: sha512-6XNEcpygZMCKaufIcgpQNZNf00GEqc7VQON+9Rd0K1bMYo8xhMZRAo5zpbnbMNizi4YNgIDAFrdykWsvY3H4Hw==}
+  /caniuse-lite@1.0.30001507:
+    resolution: {integrity: sha512-SFpUDoSLCaE5XYL2jfqe9ova/pbQHEmbheDf5r4diNwbAgR3qxM9NQtfsiSscjqoya5K7kFcHPUQ+VsUkIJR4A==}
 
   /ccount@2.0.1:
     resolution: {integrity: sha512-eyrF0jiFpY+3drT6383f1qhkbGsLSifNAjA61IUjZjmLCWjItY6LB9ft9YhoDgwfmclB2zhu51Lc7+95b8NRAg==}
 
   /chai@4.3.7:
     resolution: {integrity: sha512-HLnAzZ2iupm25PlN0xFreAlBA5zaBSv3og0DdeGA4Ar6h6rJ3A0rolRUKJhSF2V10GZKDgWF/VmAEsNWjCRB+A==}
     engines: {node: '>=4'}
@@ -2840,33 +2834,23 @@
       is-binary-path: 2.1.0
       is-glob: 4.0.3
       normalize-path: 3.0.0
       readdirp: 3.6.0
     optionalDependencies:
       fsevents: 2.3.2
 
-  /chownr@2.0.0:
-    resolution: {integrity: sha512-bIomtDF5KGpdogkLd9VspvFzk9KfpyyGlS8YFVZl7TGPBHL5snIOnxeshwVgPteQ9b4Eydl+pVbIyE1DcvCWgQ==}
-    engines: {node: '>=10'}
-    dev: true
-
   /chrome-trace-event@1.0.3:
     resolution: {integrity: sha512-p3KULyQg4S7NIHixdwbGX+nFHkoBiA4YQmyWtjb8XngSKV124nJmRysgAeujbUVb15vh+RvFUfCPqU7rXk+hZg==}
     engines: {node: '>=6.0'}
     dev: true
 
   /ci-info@3.8.0:
     resolution: {integrity: sha512-eXTggHWSooYhq49F2opQhuHWgzucfF2YgODK4e1566GQs5BIfP30B0oenwBJHfWxAs2fyPB1s7Mg949zLf61Yw==}
     engines: {node: '>=8'}
 
-  /clean-stack@2.2.0:
-    resolution: {integrity: sha512-4diC9HaTE+KRAMWhDhrGOECgWZxoevMc5TlkObMqNSsVU62PYzXZ/SMTjzyGAFF1YusgxGcSWTEXBhp0CPwQ1A==}
-    engines: {node: '>=6'}
-    dev: true
-
   /cli-boxes@3.0.0:
     resolution: {integrity: sha512-/lzGpEWL/8PfI0BmBOPRwp0c/wFNX1RdUML3jK/RcSBA9T8mZDdQpqYBKtCFTOfQbwPqWEOpjqW+Fnayc0969g==}
     engines: {node: '>=10'}
 
   /cli-cursor@4.0.0:
     resolution: {integrity: sha512-VGtlMu3x/4DOtIUwEkRezxUZ2lBacNJCHash0N0WeZDBS+7Ux1dm3XWAgWYxLJFMMdOeXMHXorshEFhbMSGelg==}
     engines: {node: ^12.20.0 || ^14.13.1 || >=16.0.0}
@@ -2927,54 +2911,50 @@
   /colorette@2.0.20:
     resolution: {integrity: sha512-IfEDxwoWIjkeXL1eXcDiow4UbKjhLdq6/EuSVR9GMN7KVH3r9gQ83e73hsz1Nd1T3ijd5xv1wcWRYO+D6kCI2w==}
     dev: true
 
   /comma-separated-tokens@2.0.3:
     resolution: {integrity: sha512-Fu4hJdvzeylCfQPp9SGWidpzrMs7tTrlu6Vb8XGaRGck8QSNZJJp538Wrb60Lax4fPwR64ViY468OIUTbRlGZg==}
 
+  /commander@10.0.1:
+    resolution: {integrity: sha512-y4Mg2tXshplEbSGzx7amzPwKKOCGuoSRP/CjEdwwk0FOGlUbq6lKuoyDZTNZkmxHdJtp54hdfY/JUrdL7Xfdug==}
+    engines: {node: '>=14'}
+    dev: true
+
   /commander@2.20.3:
     resolution: {integrity: sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==}
     dev: true
 
   /commander@4.1.1:
     resolution: {integrity: sha512-NOKm8xhkzAjzFx8B2v5OAHT+u5pRQc2UCa2Vq9jYL/31o2wi9mxBA7LIFs3sV5VSC49z6pEhfbMULvShKj26WA==}
     engines: {node: '>= 6'}
     dev: false
 
-  /commander@6.0.0:
-    resolution: {integrity: sha512-s7EA+hDtTYNhuXkTlhqew4txMZVdszBmKWSPEMxGr8ru8JXR7bLUFIAtPhcSuFdJQ0ILMxnJi8GkQL0yvDy/YA==}
-    engines: {node: '>= 6'}
-    dev: true
-
-  /commander@7.2.0:
-    resolution: {integrity: sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==}
-    engines: {node: '>= 10'}
+  /commander@9.5.0:
+    resolution: {integrity: sha512-KRs7WVDKg86PWiuAqhDrAQnTXZKraVcCc6vFdL14qrZ/DcWwuRo7VoiYXalXO7S5GKpqYiVEwCbgFDfxNHKJBQ==}
+    engines: {node: ^12.20.0 || >=14}
     dev: true
 
   /common-ancestor-path@1.0.1:
     resolution: {integrity: sha512-L3sHRo1pXXEqX8VU28kfgUY+YGsk09hPqZiZmLacNib6XNTCM8ubYeT7ryXQw8asB1sKgcU5lkB7ONug08aB8w==}
 
-  /commondir@1.0.1:
-    resolution: {integrity: sha512-W9pAhw0ja1Edb5GVdIF1mjZw/ASI0AlShXM83UUGe2DVr5TdAPEA1OA8m/g8zWp9x6On7gqufY+FatDbC3MDQg==}
-    dev: true
-
   /concat-map@0.0.1:
     resolution: {integrity: sha512-/Srv4dswyQNBfohGpz9o6Yb3Gz3SrUDqBH5rTuhGR7ahtlbYKnVxw2bCFMRljaA7EXHaXZ8wsHdodFvbkhKmqg==}
 
   /concordance@5.0.4:
     resolution: {integrity: sha512-OAcsnTEYu1ARJqWVGwf4zh4JDfHZEaSNlNccFmt8YjB2l/n19/PF2viLINHc57vO4FKIAFl2FWASIGZZWZ2Kxw==}
     engines: {node: '>=10.18.0 <11 || >=12.14.0 <13 || >=14'}
     dependencies:
       date-time: 3.1.0
       esutils: 2.0.3
       fast-diff: 1.3.0
       js-string-escape: 1.0.1
       lodash: 4.17.21
       md5-hex: 3.0.1
-      semver: 7.5.2
+      semver: 7.5.3
       well-known-symbols: 2.0.0
     dev: true
 
   /convert-source-map@1.9.0:
     resolution: {integrity: sha512-ASFBup0Mz1uyiIjANan1jzLQami9z1PoYSZCiiYW2FczPbenXc45FZdBZLzOT+r6+iciuEModtmCti+hjaAk0A==}
 
   /cookie@0.5.0:
@@ -2998,31 +2978,29 @@
       which: 2.0.2
 
   /crypto@1.0.1:
     resolution: {integrity: sha512-VxBKmeNcqQdiUQUW2Tzq0t377b54N2bMtXO/qiLa+6eRRmmC4qT3D4OnTGoT/U6O9aklQ/jTwbOtRMTTY8G0Ig==}
     deprecated: This package is no longer supported. It's now a built-in Node module. If you've depended on crypto, you should switch to the one that's built-in.
     dev: true
 
-  /css-loader@5.2.7(webpack@5.88.0):
-    resolution: {integrity: sha512-Q7mOvpBNBG7YrVGMxRxcBJZFL75o+cH2abNASdibkj/fffYD8qWbInZrD0S9ccI6vZclF3DsHE7njGlLtaHbhg==}
-    engines: {node: '>= 10.13.0'}
+  /css-loader@6.8.1(webpack@5.88.0):
+    resolution: {integrity: sha512-xDAXtEVGlD0gJ07iclwWVkLoZOpEvAWaSyf6W18S2pOC//K8+qUDIx8IIT3D+HjnmkJPQeesOPv5aiUaJsCM2g==}
+    engines: {node: '>= 12.13.0'}
     peerDependencies:
-      webpack: ^4.27.0 || ^5.0.0
+      webpack: ^5.0.0
     dependencies:
       icss-utils: 5.1.0(postcss@8.4.24)
-      loader-utils: 2.0.4
       postcss: 8.4.24
       postcss-modules-extract-imports: 3.0.0(postcss@8.4.24)
       postcss-modules-local-by-default: 4.0.3(postcss@8.4.24)
       postcss-modules-scope: 3.0.0(postcss@8.4.24)
       postcss-modules-values: 4.0.0(postcss@8.4.24)
       postcss-value-parser: 4.2.0
-      schema-utils: 3.3.0
-      semver: 7.5.2
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      semver: 7.5.3
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
     dev: true
 
   /css.escape@1.5.1:
     resolution: {integrity: sha512-YUifsXXuknHlUsmlgyY0PKzgPOr7/FjCePfHNt0jxm83wHZi44VDMQ7/fGNkjY3/jV1MC+1CmZbaHzugyeRtpg==}
     dev: true
 
   /cssesc@3.0.0:
@@ -3115,15 +3093,14 @@
   /deepmerge-ts@4.3.0:
     resolution: {integrity: sha512-if3ZYdkD2dClhnXR5reKtG98cwyaRT1NeugQoAPTTfsOpV9kqyeiBF9Qa5RHjemb3KzD5ulqygv6ED3t5j9eJw==}
     engines: {node: '>=12.4.0'}
 
   /deepmerge@4.3.1:
     resolution: {integrity: sha512-3sUqbMEc77XqpdNO7FRyRog+eW3ph+GYCbj+rK+uYyRMuwsVy0rMiVtPn+QJlKFvWP/1PYpapqYn0Me2knFn+A==}
     engines: {node: '>=0.10.0'}
-    dev: false
 
   /default-browser-id@3.0.0:
     resolution: {integrity: sha512-OZ1y3y0SqSICtE8DE4S8YOE9UZOJ8wO16fKWVP5J1Qz42kV9jcnMVFrEE/noXb/ss3Q4pZIH79kxofzyNNtUNA==}
     engines: {node: '>=12'}
     dependencies:
       bplist-parser: 0.2.0
       untildify: 4.0.0
@@ -3185,14 +3162,41 @@
     dependencies:
       path-type: 4.0.0
     dev: true
 
   /dlv@1.1.3:
     resolution: {integrity: sha512-+HlytyjlPKnIG8XuRG8WvmBP8xs8P71y+SKKS6ZXWoEgLuePxtDoUEiH7WkdePWrQ5JBpE6aoVqfZfJUQkjXwA==}
 
+  /dom-serializer@2.0.0:
+    resolution: {integrity: sha512-wIkAryiqt/nV5EQKqQpo3SToSOV9J0DnbJqwK7Wv/Trc92zIAYZ4FlMu+JPFW1DfGFt81ZTCGgDEabffXeLyJg==}
+    dependencies:
+      domelementtype: 2.3.0
+      domhandler: 5.0.3
+      entities: 4.5.0
+    dev: true
+
+  /domelementtype@2.3.0:
+    resolution: {integrity: sha512-OLETBj6w0OsagBwdXnPdN0cnMfF9opN69co+7ZrbfPGrdpPVNBUj02spi6B1N7wChLQiPn4CSH/zJvXw56gmHw==}
+    dev: true
+
+  /domhandler@5.0.3:
+    resolution: {integrity: sha512-cgwlv/1iFQiFnU96XXgROh8xTeetsnJiDsTc7TYCLFd9+/WNkIqPTxiM/8pSd8VIrhXGTf1Ny1q1hquVqDJB5w==}
+    engines: {node: '>= 4'}
+    dependencies:
+      domelementtype: 2.3.0
+    dev: true
+
+  /domutils@3.1.0:
+    resolution: {integrity: sha512-H78uMmQtI2AhgDJjWeQmHwJJ2bLPD3GMmO7Zja/ZZh84wkm+4ut+IUnUdRa8uCGX88DiVx1j6FRe1XfxEgjEZA==}
+    dependencies:
+      dom-serializer: 2.0.0
+      domelementtype: 2.3.0
+      domhandler: 5.0.3
+    dev: true
+
   /dotenv@16.3.1:
     resolution: {integrity: sha512-IPzF4w4/Rd94bA9imS68tZBaYyBWSCE47V1RGuMrB94iyTOIEwRmVL2x/4An+6mETpLrKJ5hQkB8W4kFAadeIQ==}
     engines: {node: '>=12'}
     dev: true
 
   /dset@3.1.2:
     resolution: {integrity: sha512-g/M9sqy3oHe477Ar4voQxWtaPIFw1jTdKZuomOjhCcBx9nHUNn0pu6NopuFFrTh/TRZIKEj+76vLWFu9BNKk+Q==}
@@ -3206,16 +3210,16 @@
       lodash: 4.17.21
       semver: 5.7.1
     dev: true
 
   /eastasianwidth@0.2.0:
     resolution: {integrity: sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==}
 
-  /electron-to-chromium@1.4.437:
-    resolution: {integrity: sha512-ZFekRuBOHUXp21wrR5lshT6pZa/KmjkhKBAtmZz4NN5sCWlHOk3kdhiwFINrDBsRLX6FjyBAb1TRN+KBeNlyzQ==}
+  /electron-to-chromium@1.4.439:
+    resolution: {integrity: sha512-BHpErPSNhb9FB25+OwQP6mCAf3ZXfGbmuvc4LzBNVJwpCcXQJm++LerimocYRG9FRxUVRKZqaB7d0+pImSTPSg==}
 
   /emmet@2.4.4:
     resolution: {integrity: sha512-v8Mwpjym55CS3EjJgiCLWUB3J2HSR93jhzXW325720u8KvYxdI2voYLstW3pHBxFz54H6jFjayR9G4LfTG0q+g==}
     dependencies:
       '@emmetio/abbreviation': 2.3.3
       '@emmetio/css-abbreviation': 2.1.8
 
@@ -3325,44 +3329,14 @@
     engines: {node: '>= 0.4'}
     dependencies:
       is-callable: 1.2.7
       is-date-object: 1.0.5
       is-symbol: 1.0.4
     dev: true
 
-  /esbuild@0.16.17:
-    resolution: {integrity: sha512-G8LEkV0XzDMNwXKgM0Jwu3nY3lSTwSGY6XbxM9cr9+s0T/qSV1q1JVPBGzm3dcjhCic9+emZDmMffkwgPeOeLg==}
-    engines: {node: '>=12'}
-    hasBin: true
-    requiresBuild: true
-    optionalDependencies:
-      '@esbuild/android-arm': 0.16.17
-      '@esbuild/android-arm64': 0.16.17
-      '@esbuild/android-x64': 0.16.17
-      '@esbuild/darwin-arm64': 0.16.17
-      '@esbuild/darwin-x64': 0.16.17
-      '@esbuild/freebsd-arm64': 0.16.17
-      '@esbuild/freebsd-x64': 0.16.17
-      '@esbuild/linux-arm': 0.16.17
-      '@esbuild/linux-arm64': 0.16.17
-      '@esbuild/linux-ia32': 0.16.17
-      '@esbuild/linux-loong64': 0.16.17
-      '@esbuild/linux-mips64el': 0.16.17
-      '@esbuild/linux-ppc64': 0.16.17
-      '@esbuild/linux-riscv64': 0.16.17
-      '@esbuild/linux-s390x': 0.16.17
-      '@esbuild/linux-x64': 0.16.17
-      '@esbuild/netbsd-x64': 0.16.17
-      '@esbuild/openbsd-x64': 0.16.17
-      '@esbuild/sunos-x64': 0.16.17
-      '@esbuild/win32-arm64': 0.16.17
-      '@esbuild/win32-ia32': 0.16.17
-      '@esbuild/win32-x64': 0.16.17
-    dev: true
-
   /esbuild@0.17.19:
     resolution: {integrity: sha512-XQ0jAPFkK/u3LcVRcvVHQcTIqD6E2H1fvZMA5dQPSOWb3suUbWbfbRf94pjc0bNzRYLfIrDRQXr7X+LHIm5oHw==}
     engines: {node: '>=12'}
     hasBin: true
     requiresBuild: true
     optionalDependencies:
       '@esbuild/android-arm': 0.17.19
@@ -3422,14 +3396,19 @@
     resolution: {integrity: sha512-k0er2gUkLf8O0zKJiAhmkTnJlTvINGv7ygDNPbeIsX/TJjGJZHuh9B2UxbsaEkmlEo9MfhrSzmhIlhRlI2GXnw==}
     engines: {node: '>=6'}
 
   /escape-string-regexp@1.0.5:
     resolution: {integrity: sha512-vbRorB5FUQWvla16U8R/qgaFIya2qGzwDrNmCZuYKrbdSUMG6I1ZCGQRefkRVhuOkIGVne7BQ35DSfo1qvJqFg==}
     engines: {node: '>=0.8.0'}
 
+  /escape-string-regexp@4.0.0:
+    resolution: {integrity: sha512-TtpcNJ3XAzx3Gq8sWRzJaVajRs0uVxA2YAkdb1jm2YkPz4G6egUFAyA3n5vtEIZefPk5Wa4UXbKuS5fKkJWdgA==}
+    engines: {node: '>=10'}
+    dev: true
+
   /escape-string-regexp@5.0.0:
     resolution: {integrity: sha512-/veY75JbMK4j1yjvuUxuVsiS/hr/4iHs9FTT6cgTexxdE0Ly/glccBAkloH/DofkjRbZU3bnoj38mOmhkZ0lHw==}
     engines: {node: '>=12'}
 
   /eslint-scope@5.1.1:
     resolution: {integrity: sha512-2NxwbF/hZ0KpepYN0cNbo+FN6XoK7GaHlQhgx/hIZl6Va0bF45RQOOwhLIy8lQDbuCiadSLCBnH2CFYquit5bw==}
     engines: {node: '>=8.0.0'}
@@ -3607,48 +3586,28 @@
 
   /fault@2.0.1:
     resolution: {integrity: sha512-WtySTkS4OKev5JtpHXnib4Gxiurzh5NCGvWrFaZ34m6JehfTUhKZvn9njTfw48t6JumVQOmrKqpmGcdwxnhqBQ==}
     dependencies:
       format: 0.2.2
     dev: false
 
-  /file-loader@6.0.0(webpack@5.88.0):
-    resolution: {integrity: sha512-/aMOAYEFXDdjG0wytpTL5YQLfZnnTmLNjn+AIrJ/6HVnTfDqLsVKUUwkDf4I4kgex36BvjuXEn/TX9B/1ESyqQ==}
-    engines: {node: '>= 10.13.0'}
-    peerDependencies:
-      webpack: ^4.0.0 || ^5.0.0
-    dependencies:
-      loader-utils: 2.0.4
-      schema-utils: 2.7.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-    dev: true
-
   /fill-range@7.0.1:
     resolution: {integrity: sha512-qOo9F+dMUmC2Lcb4BbVvnKJxTPjCm+RRpe4gDuGrzkL7mEVl/djYSu2OdQ2Pa302N4oqkSg9ir6jaLWJ2USVpQ==}
     engines: {node: '>=8'}
     dependencies:
       to-regex-range: 5.0.1
 
   /find-babel-config@2.0.0:
     resolution: {integrity: sha512-dOKT7jvF3hGzlW60Gc3ONox/0rRZ/tz7WCil0bqA1In/3I8f1BctpXahRnEKDySZqci7u+dqq93sZST9fOJpFw==}
     engines: {node: '>=16.0.0'}
     dependencies:
       json5: 2.2.3
       path-exists: 4.0.0
     dev: false
 
-  /find-cache-dir@3.3.2:
-    resolution: {integrity: sha512-wXZV5emFEjrridIgED11OoUKLxiYjAcqot/NJdAkOhlJ+vGzwhOAfcG5OX1jP+S0PcjEn8bdMJv+g2jwQ3Onig==}
-    engines: {node: '>=8'}
-    dependencies:
-      commondir: 1.0.1
-      make-dir: 3.1.0
-      pkg-dir: 4.2.0
-    dev: true
-
   /find-root@1.1.0:
     resolution: {integrity: sha512-NKfW6bec6GfKc0SGx1e07QZY9PE99u0Bft/0rzSD5k3sO/vwkVUpDUKVm5Gpp5Ue3YfShPFTX2070tDs5kB9Ng==}
     dev: true
 
   /find-up@3.0.0:
     resolution: {integrity: sha512-1yD6RmLI1XBfxugvORwlck6f75tYL+iR0jqwsOrOxMZyGYqUuDhJ0l4AXdO1iX/FTs9cBAMEk1gWSEx1kSbylg==}
     engines: {node: '>=6'}
@@ -3687,14 +3646,23 @@
     engines: {node: '>=0.4.x'}
     dev: false
 
   /fraction.js@4.2.0:
     resolution: {integrity: sha512-MhLuK+2gUcnZe8ZHlaaINnQLl0xRIGRfcGk2yl8xoQAfHrSsL3rYu6FCmBdkdbhc9EPlwyGHewaRsvwRMJtAlA==}
     dev: false
 
+  /fs-extra@10.1.0:
+    resolution: {integrity: sha512-oRXApq54ETRj4eMiFzGnHWGy+zo5raudjuxN0b8H7s/RU2oW0Wvsx9O0ACRN/kRq9E8Vu/ReskGB5o3ji+FzHQ==}
+    engines: {node: '>=12'}
+    dependencies:
+      graceful-fs: 4.2.11
+      jsonfile: 6.1.0
+      universalify: 2.0.0
+    dev: true
+
   /fs-extra@7.0.1:
     resolution: {integrity: sha512-YJDaCJZEnBmcbw13fvdAM9AwNOJwOzrE4pqMqBq5nFiEqXUqHwlK4B+3pUw6JNvfSPtX05xFHtYy/1ni01eGCw==}
     engines: {node: '>=6 <7 || >=8'}
     dependencies:
       graceful-fs: 4.2.11
       jsonfile: 4.0.0
       universalify: 0.1.2
@@ -3705,31 +3673,14 @@
     engines: {node: '>=6 <7 || >=8'}
     dependencies:
       graceful-fs: 4.2.11
       jsonfile: 4.0.0
       universalify: 0.1.2
     dev: true
 
-  /fs-extra@9.1.0:
-    resolution: {integrity: sha512-hcg3ZmepS30/7BSFqRvoo3DOMQu7IjqxO5nCDt+zM9XWjb33Wg7ziNT+Qvqbuc3+gWpzO02JubVyk2G4Zvo1OQ==}
-    engines: {node: '>=10'}
-    dependencies:
-      at-least-node: 1.0.0
-      graceful-fs: 4.2.11
-      jsonfile: 6.1.0
-      universalify: 2.0.0
-    dev: true
-
-  /fs-minipass@2.1.0:
-    resolution: {integrity: sha512-V/JgOLFCS+R6Vcq0slCuaeWEdNC3ouDlJMNIsacH2VtALiu9mV4LPrHc5cDl8k5aw6J8jwgWWpiTo5RYhmIzvg==}
-    engines: {node: '>= 8'}
-    dependencies:
-      minipass: 3.3.6
-    dev: true
-
   /fs.realpath@1.0.0:
     resolution: {integrity: sha512-OO0pH2lK6a0hZnAdau5ItzHPI6pUlvI7jMVnxUQRtw4owF2wk8lOSabtGDCTP4Ggrg2MbGnWO9X8K1t4+fGMDw==}
 
   /fsevents@2.3.2:
     resolution: {integrity: sha512-xiqMQR4xAeHTuB9uWm+fFRcIOgKBMiOBP+eXiyT7jsgVCq1bkVygt00oASowB7EdtpOHaaPgKt812P9ab+DDKA==}
     engines: {node: ^8.16.0 || ^10.6.0 || >=11.0.0}
     os: [darwin]
@@ -4046,14 +3997,23 @@
 
   /html-escaper@3.0.3:
     resolution: {integrity: sha512-RuMffC89BOWQoY0WKGpIhn5gX3iI54O6nRA0yC124NYVtzjmFWBIiFd8M0x+ZdX0P9R4lADg1mgP8C7PxGOWuQ==}
 
   /html-void-elements@2.0.1:
     resolution: {integrity: sha512-0quDb7s97CfemeJAnW9wC0hw78MtW7NU3hqtCD75g2vFlDLt36llsYD7uB7SUzojLMP24N5IatXf7ylGXiGG9A==}
 
+  /htmlparser2@8.0.2:
+    resolution: {integrity: sha512-GYdjWKDkbRLkZ5geuHs5NY1puJ+PXwP7+fHPRz06Eirsb9ugf6d8kkXav6ADhcODhFFPMIXyxkxSuMf3D6NCFA==}
+    dependencies:
+      domelementtype: 2.3.0
+      domhandler: 5.0.3
+      domutils: 3.1.0
+      entities: 4.5.0
+    dev: true
+
   /human-id@1.0.2:
     resolution: {integrity: sha512-UNopramDEhHJD+VR+ehk8rOslwSfByxPIZyJRfV739NDhN5LF1fa1MqnzKm2lGTQRjNrjK19Q5fhkgIfjlVUKw==}
     dev: true
 
   /human-signals@2.1.0:
     resolution: {integrity: sha512-B4FFZ6q/T2jhhksgkbEW3HBvWIfDW85snkQgawt07S7J5QXTk6BkNV+0yAeZrM5QpMAdYlocGoljn0sJ/WQkFw==}
     engines: {node: '>=10.17.0'}
@@ -4105,28 +4065,19 @@
       pkg-dir: 4.2.0
       resolve-cwd: 3.0.0
     dev: true
 
   /import-meta-resolve@2.2.2:
     resolution: {integrity: sha512-f8KcQ1D80V7RnqVm+/lirO9zkOxjGxhaTC1IPrBGd3MEfNgmNG67tSUO9gTi2F3Blr2Az6g1vocaxzkVnWl9MA==}
 
-  /imurmurhash@0.1.4:
-    resolution: {integrity: sha512-JmXMZ6wuvDmLiHEml9ykzqO6lwFbof0GG4IkcGaENdCRDDmMVnny7s5HsIgHCbaq0w2MyPhDqkhTUgS2LU2PHA==}
-    engines: {node: '>=0.8.19'}
-    dev: true
-
   /indent-string@4.0.0:
     resolution: {integrity: sha512-EdDDZu4A2OyIK7Lr/2zG+w5jmbuk1DVBnEwREQvBzspBJkCEbRa8GxU1lghYcaGJCnRWibjDXlq779X1/y5xwg==}
     engines: {node: '>=8'}
     dev: true
 
-  /infer-owner@1.0.4:
-    resolution: {integrity: sha512-IClj+Xz94+d7irH5qRyfJonOdfTzuDaifE6ZPWfx0N0+/ATZCbuTPq2prFl526urkQd90WyUKIh1DfBQ2hMz9A==}
-    dev: true
-
   /inflight@1.0.6:
     resolution: {integrity: sha512-k92I/b08q4wvFscXCLvqfsHCrjrF7yiXsQuIVvVE7N82W3+aqpzuUdBbfhWcy/FZR3/4IgflMgKLOsvPDrGCJA==}
     dependencies:
       once: 1.4.0
       wrappy: 1.0.2
 
   /inherits@2.0.4:
@@ -4141,17 +4092,17 @@
     engines: {node: '>= 0.4'}
     dependencies:
       get-intrinsic: 1.2.1
       has: 1.0.3
       side-channel: 1.0.4
     dev: true
 
-  /interpret@2.2.0:
-    resolution: {integrity: sha512-Ju0Bz/cEia55xDwUWEa8+olFpCiQoypjnQySseKtmjNrnps3P+xfpUmGr90T7yjlVJmOtybRvPXhKMbHr+fWnw==}
-    engines: {node: '>= 0.10'}
+  /interpret@3.1.1:
+    resolution: {integrity: sha512-6xwYfHbajpoF0xLW+iwLkhwgvLoZDfjYfoFNu8ftMoXINzwuymNLd9u/KmwtdT2GbR+/Cz66otEGEVVUHX9QLQ==}
+    engines: {node: '>=10.13.0'}
     dev: true
 
   /is-alphabetical@2.0.1:
     resolution: {integrity: sha512-FWyyY60MeTNyeSRpkM2Iry0G9hpr7/9kD40mD/cGQEuilcZYS4okz8SN2Q6rLCJ8gbCt6fN+rC+6tMGS99LaxQ==}
     dev: false
 
   /is-alphanumerical@2.0.1:
@@ -4296,14 +4247,19 @@
   /is-plain-object@2.0.4:
     resolution: {integrity: sha512-h5PpgXkWitc38BBMYawTYMWJHFZJVnBquFE57xFpjB8pJFiF6gZ+bU+WyI/yqXiFR5mdLsgYNaPe8uao6Uv9Og==}
     engines: {node: '>=0.10.0'}
     dependencies:
       isobject: 3.0.1
     dev: true
 
+  /is-plain-object@5.0.0:
+    resolution: {integrity: sha512-VRSzKkbMm5jMDoKLbltAkFQ5Qr7VDiTFGXxYFXXowVj387GeGNOCsOH6Msy00SGZ3Fp84b1Naa1psqgcCIEP5Q==}
+    engines: {node: '>=0.10.0'}
+    dev: true
+
   /is-reference@3.0.1:
     resolution: {integrity: sha512-baJJdQLiYaJdvFbJqXrcGv3WU3QCzBlUcI5QhbesIm6/xPsvmO+2CDoi/GMOFBQEQm+PXkwOPrp9KK5ozZsp2w==}
     dependencies:
       '@types/estree': 1.0.1
     dev: false
 
   /is-regex@1.1.4:
@@ -4385,23 +4341,14 @@
     resolution: {integrity: sha512-RHxMLp9lnKHGHRng9QFhRCMbYAcVpn69smSGcq3f36xjgVVWThj4qqLbTLlq7Ssj8B+fIQ1EuCEGI2lKsyQeIw==}
 
   /isobject@3.0.1:
     resolution: {integrity: sha512-WhB9zCku7EGTj/HQQRz5aUQEUeoQZH2bWcltRErOpymJ4boYE6wL9Tbr23krRPSZ+C5zqNSrSw+Cc7sZZ4b7vg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
-  /jest-worker@26.6.2:
-    resolution: {integrity: sha512-KWYVV1c4i+jbMpaBC+U++4Va0cp8OisU185o73T1vo99hqi7w8tSJfUXYswwqqrjzwxa6KpRK54WhPvwf5w6PQ==}
-    engines: {node: '>= 10.13.0'}
-    dependencies:
-      '@types/node': 18.0.0
-      merge-stream: 2.0.0
-      supports-color: 7.2.0
-    dev: true
-
   /jest-worker@27.5.1:
     resolution: {integrity: sha512-7vuh85V5cdDofPyxn58nrPjBktZo0u9x1g8WtjQol+jZDaE+fhN+cIvTj11GndBnMnyfrUOG1sZQxCdjKh+DKg==}
     engines: {node: '>= 10.13.0'}
     dependencies:
       '@types/node': 18.0.0
       merge-stream: 2.0.0
       supports-color: 8.1.1
@@ -4410,15 +4357,14 @@
   /jiti@1.18.2:
     resolution: {integrity: sha512-QAdOptna2NYiSSpv0O/BwoHBSmz4YhpzJHyi+fnMRTXFjp7B8i/YG5Z8IfusxB1ufjcD2Sre1F3R+nX3fvy7gg==}
     hasBin: true
     dev: false
 
   /jquery@3.7.0:
     resolution: {integrity: sha512-umpJ0/k8X0MvD1ds0P9SfowREz2LenHsQaxSohMZ5OMNEU2r0tf8pdeEFTHMFxWVxKNyU9rTtK3CWzUCTKJUeQ==}
-    dev: false
 
   /js-string-escape@1.0.1:
     resolution: {integrity: sha512-Smw4xcfIQ5LVjAOuJCvN/zIodzA/BBSsluuoSykP+lUvScIi4U6RJLfwHet5cxFnCswUjISV8oAXaqaJDY3chg==}
     engines: {node: '>= 0.8'}
     dev: true
 
   /js-tokens@4.0.0:
@@ -4445,19 +4391,16 @@
   /json-parse-even-better-errors@2.3.1:
     resolution: {integrity: sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==}
     dev: true
 
   /json-schema-traverse@0.4.1:
     resolution: {integrity: sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==}
 
-  /json5@1.0.2:
-    resolution: {integrity: sha512-g1MWMLBiz8FKi1e4w0UyVL3w+iJceWAFBAaBnnGKOpNa5f8TLktkbre1+s6oICydWAm+HRUGTmI+//xv2hvXYA==}
-    hasBin: true
-    dependencies:
-      minimist: 1.2.8
+  /json-schema-traverse@1.0.0:
+    resolution: {integrity: sha512-NM8/P9n3XjXhIZn1lLhkFaACTOURQXjWhV4BA/RnOv8xvgqtqpAX9IO4mRQxSx1Rlo4tqzeqb0sOlruaOy3dug==}
     dev: true
 
   /json5@2.2.3:
     resolution: {integrity: sha512-XmOWe7eyHYH14cLdVPoyg+GOH3rYX++KpzrylJwSW98t3Nk+U8XOl8FWKOgwtzdb8lXGf6zYwDUzeHMWfxasyg==}
     engines: {node: '>=6'}
     hasBin: true
 
@@ -4498,15 +4441,15 @@
     peerDependencies:
       webpack: '*'
     peerDependenciesMeta:
       webpack:
         optional: true
     dependencies:
       '@types/webpack-sources': 0.1.9
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
       webpack-sources: 1.4.3
     dev: true
 
   /lilconfig@2.1.0:
     resolution: {integrity: sha512-utWOt/GHzuUxnLKxB6dk81RoOeoNeHgbrXiuGk4yyF5qlRz+iIVWu56E2fqGHFrXz0QNUhLB/8nKqvRH66JKGQ==}
     engines: {node: '>=10'}
     dev: false
@@ -4524,23 +4467,14 @@
       strip-bom: 3.0.0
 
   /loader-runner@4.3.0:
     resolution: {integrity: sha512-3R/1M+yS3j5ou80Me59j7F9IMs4PXs3VqRrm0TU3AbKPxlmpoY1TNscJV/oGJXo8qCatFGTfDbY6W6ipGOYXfg==}
     engines: {node: '>=6.11.5'}
     dev: true
 
-  /loader-utils@1.4.2:
-    resolution: {integrity: sha512-I5d00Pd/jwMD2QCduo657+YM/6L3KZu++pmX9VFncxaxvHcru9jx1lBaFft+r4Mt2jK0Yhp41XlRAihzPxHNCg==}
-    engines: {node: '>=4.0.0'}
-    dependencies:
-      big.js: 5.2.2
-      emojis-list: 3.0.0
-      json5: 1.0.2
-    dev: true
-
   /loader-utils@2.0.4:
     resolution: {integrity: sha512-xXqpXoINfFhgua9xiqD8fPFHgkoq1mmmpE92WlDbm9rNRd/EbRb+Gqf908T2DMfuHjjJlksiK2RbHVOdD/MqSw==}
     engines: {node: '>=8.9.0'}
     dependencies:
       big.js: 5.2.2
       emojis-list: 3.0.0
       json5: 2.2.3
@@ -4628,21 +4562,14 @@
   /magic-string@0.30.0:
     resolution: {integrity: sha512-LA+31JYDJLs82r2ScLrlz1GjSgu66ZV518eyWT+S8VhyQn/JL0u9MeBOvQMGYiPk1DBiSN9DDMOcXvigJZaViQ==}
     engines: {node: '>=12'}
     dependencies:
       '@jridgewell/sourcemap-codec': 1.4.15
     dev: true
 
-  /make-dir@3.1.0:
-    resolution: {integrity: sha512-g3FeP20LNwhALb/6Cz6Dd4F2ngze0jz7tbzrD2wAV+o9FeNHe4rL+yK2md0J/fiSf1sa1ADhXqi5+oVwOM/eGw==}
-    engines: {node: '>=8'}
-    dependencies:
-      semver: 6.3.0
-    dev: true
-
   /map-obj@1.0.1:
     resolution: {integrity: sha512-7N/q3lyZ+LVCp7PzuxrJr4KMbBE2hW7BT7YNia330OFxIf4d3r5zVpicP2650l7CPN6RM9zOJRl3NGpqSiw3Eg==}
     engines: {node: '>=0.10.0'}
     dev: true
 
   /map-obj@4.3.0:
     resolution: {integrity: sha512-hdN1wVrZbb29eBGiGjJbeP8JbKjq1urkHJ/LIP/NY48MZ1QVXUsQBV1G1zvYFHn1XE06cwjBsOI2K3Ulnj1YXQ==}
@@ -5217,24 +5144,27 @@
     engines: {node: '>=12'}
 
   /min-indent@1.0.1:
     resolution: {integrity: sha512-I9jwMn07Sy/IwOj3zVkVik2JTvgpaykDZEigL6Rx6N9LbMywwUSMtxET+7lVoDLLd3O3IXwJwvuuns8UB/HeAg==}
     engines: {node: '>=4'}
     dev: true
 
-  /mini-css-extract-plugin@1.3.9(webpack@5.88.0):
-    resolution: {integrity: sha512-Ac4s+xhVbqlyhXS5J/Vh/QXUz3ycXlCqoCPpg0vdfhsIBH9eg/It/9L1r1XhSCH737M1lqcWnMuWL13zcygn5A==}
-    engines: {node: '>= 10.13.0'}
+  /mini-css-extract-plugin@2.7.6(webpack@5.88.0):
+    resolution: {integrity: sha512-Qk7HcgaPkGG6eD77mLvZS1nmxlao3j+9PkrT9Uc7HAE1id3F41+DdBRYRYkbyfNRGzm8/YWtzhw7nVPmwhqTQw==}
+    engines: {node: '>= 12.13.0'}
     peerDependencies:
-      webpack: ^4.4.0 || ^5.0.0
+      webpack: ^5.0.0
     dependencies:
-      loader-utils: 2.0.4
-      schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-      webpack-sources: 1.4.3
+      schema-utils: 4.2.0
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
+    dev: true
+
+  /mini-svg-data-uri@1.4.4:
+    resolution: {integrity: sha512-r9deDe9p5FJUPZAk3A59wGH7Ii9YrjjWw0jmw/liSbHl2CHiyXj6FcDXDu2K3TjVAXqiJdaw3xxwlZZr9E6nHg==}
+    hasBin: true
     dev: true
 
   /minimatch@3.1.2:
     resolution: {integrity: sha512-J7p63hRiAjw1NDEww1W7i37+ByIrOWO5XQQAzZ3VOcL0PNybwpfmV/N05zFAzwQ9USyEcX6t3UO+K5aqBQOIHw==}
     dependencies:
       brace-expansion: 1.1.11
 
@@ -5253,78 +5183,30 @@
       is-plain-obj: 1.1.0
       kind-of: 6.0.3
     dev: true
 
   /minimist@1.2.8:
     resolution: {integrity: sha512-2yyAR8qBkN3YuheJanUpWC5U3bb5osDywNB8RzDVlDwDHbocAJveqqj1u8+SVD7jkWT4yvsHCpWqqWqAxb0zCA==}
 
-  /minipass-collect@1.0.2:
-    resolution: {integrity: sha512-6T6lH0H8OG9kITm/Jm6tdooIbogG9e0tLgpY6mphXSm/A9u8Nq1ryBG+Qspiub9LjWlBPsPS3tWQ/Botq4FdxA==}
-    engines: {node: '>= 8'}
-    dependencies:
-      minipass: 3.3.6
-    dev: true
-
-  /minipass-flush@1.0.5:
-    resolution: {integrity: sha512-JmQSYYpPUqX5Jyn1mXaRwOda1uQ8HP5KAT/oDSLCzt1BYRhQU0/hDtsB1ufZfEEzMZ9aAVmsBw8+FWsIXlClWw==}
-    engines: {node: '>= 8'}
-    dependencies:
-      minipass: 3.3.6
-    dev: true
-
-  /minipass-pipeline@1.2.4:
-    resolution: {integrity: sha512-xuIq7cIOt09RPRJ19gdi4b+RiNvDFYe5JH+ggNvBqGqpQXcru3PcRmOZuHBKWK1Txf9+cQ+HMVN4d6z46LZP7A==}
-    engines: {node: '>=8'}
-    dependencies:
-      minipass: 3.3.6
-    dev: true
-
-  /minipass@3.3.6:
-    resolution: {integrity: sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==}
-    engines: {node: '>=8'}
-    dependencies:
-      yallist: 4.0.0
-    dev: true
-
-  /minipass@5.0.0:
-    resolution: {integrity: sha512-3FnjYuehv9k6ovOEbyOswadCDPX1piCfhV8ncmYtHOjuPwylVWsghTLo7rabjC3Rx5xD4HDx8Wm1xnMF7S5qFQ==}
-    engines: {node: '>=8'}
-    dev: true
-
-  /minizlib@2.1.2:
-    resolution: {integrity: sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==}
-    engines: {node: '>= 8'}
-    dependencies:
-      minipass: 3.3.6
-      yallist: 4.0.0
-    dev: true
-
   /mixme@0.5.9:
     resolution: {integrity: sha512-VC5fg6ySUscaWUpI4gxCBTQMH2RdUpNrk+MsbpCYtIvf9SBJdiUey4qE7BXviJsJR4nDQxCZ+3yaYNW3guz/Pw==}
     engines: {node: '>= 8.0.0'}
     dev: true
 
-  /mkdirp@1.0.4:
-    resolution: {integrity: sha512-vVqVZQyf3WLx2Shd0qJ9xuvqgAyKPLAiqITEtqW0oIUjzo3PePDd6fW9iFz30ef7Ysp/oiWqbhszeGWW2T6Gzw==}
-    engines: {node: '>=10'}
-    hasBin: true
-    dev: true
-
   /mlly@1.4.0:
     resolution: {integrity: sha512-ua8PAThnTwpprIaU47EPeZ/bPUVp2QYBbWMphUQpVdBI3Lgqzm5KZQ45Agm3YJedHXaIHl6pBGabaLSUPPSptg==}
     dependencies:
       acorn: 8.9.0
       pathe: 1.1.1
       pkg-types: 1.0.3
       ufo: 1.1.2
     dev: true
 
   /moment@2.29.4:
     resolution: {integrity: sha512-5LC9SOxjSc2HF6vO2CyuTDNivEdoz2IvyJJGj6X8DJ0eFyfszE0QiEd+iXmBvUP3WHxSjFH/vIsA0EN00cgr8w==}
-    dev: false
 
   /mri@1.2.0:
     resolution: {integrity: sha512-tzzskb3bG8LvYGFF/mDTpq3jpI6Q9wc3LEmBaghu+DdCssd1FakN7Bc0hVNmEyGq1bq3RgfkCb3cmQLpNPOroA==}
     engines: {node: '>=4'}
 
   /ms@2.1.2:
     resolution: {integrity: sha512-sGkPx+VjMtmA6MX27oA4FBFELFCZZ4S4XqeGOXCv68tT+jb3vk/RyaKWP0PTKyWtmLSM0b+adUTEvbs1PEaH2w==}
@@ -5518,21 +5400,14 @@
       p-limit: 3.1.0
 
   /p-map@2.1.0:
     resolution: {integrity: sha512-y3b8Kpd8OAN444hxfBbFfj1FY/RjtTd8tzYwhUqNYXx0fXx2iX4maP4Qr6qhIKbQXI02wTLAda4fYUbDagTUFw==}
     engines: {node: '>=6'}
     dev: true
 
-  /p-map@4.0.0:
-    resolution: {integrity: sha512-/bjOqmgETBYB5BoEeGVea8dmvHb2m9GLy1E9W43yeyfP6QQCZGFNa+XRceJEuDB6zqr+gKpIAmlLebMpykw/MQ==}
-    engines: {node: '>=10'}
-    dependencies:
-      aggregate-error: 3.1.0
-    dev: true
-
   /p-try@2.2.0:
     resolution: {integrity: sha512-R4nPAVTAU0B9D35/Gk3uJf/7XYbQcyohSKdvAxIRSNghFl4e71hVoGnBNQz9cWaXxO2I10KTC+3jMdvvoKw6dQ==}
     engines: {node: '>=6'}
 
   /parse-entities@4.0.1:
     resolution: {integrity: sha512-SWzvYcSJh4d/SGLIOQfZ/CoNv6BTlI6YEQ7Nj82oDVnRpwe/Z/F1EMx42x3JAOwGBlCjeCH0BRJQbQ/opHL17w==}
     dependencies:
@@ -5559,14 +5434,18 @@
   /parse-latin@5.0.1:
     resolution: {integrity: sha512-b/K8ExXaWC9t34kKeDV8kGXBkXZ1HCSAZRYE7HR14eA1GlXX5L8iWhs8USJNhQU9q5ci413jCKF0gOyovvyRBg==}
     dependencies:
       nlcst-to-string: 3.1.1
       unist-util-modify-children: 3.1.1
       unist-util-visit-children: 2.0.2
 
+  /parse-srcset@1.0.2:
+    resolution: {integrity: sha512-/2qh0lav6CmI15FzA3i/2Bzk2zCgQhGMkvhOhKNcBVQ1ldgpbfiNTVslmooUmWJcADi1f1kIeynbDRVzNlfR6Q==}
+    dev: true
+
   /parse5@6.0.1:
     resolution: {integrity: sha512-Ofn/CTFzRGTTxwpNEs9PP93gXShHcTq255nzRYSKe8AkVpZY7e1fpmTfOyoIvjP5HG7Z2ZM7VS9PPhQGW2pOpw==}
 
   /path-browserify@1.0.1:
     resolution: {integrity: sha512-b7uo2UCUOYZcnF/3ID0lulOJi/bafxa1xPe7ZPsammBSpjSWQkjNxlt635YGS2MiR9GjvuXCtz2emr3jbsz98g==}
     dev: true
 
@@ -5842,23 +5721,14 @@
     engines: {node: '>=6'}
 
   /process@0.11.10:
     resolution: {integrity: sha512-cdGef/drWFoydD1JsMzuFf8100nZl+GT+yacc2bEced5f9Rjk4z+WtFUTBu9PhOi9j/jfmBPu0mMEY4wIdAF8A==}
     engines: {node: '>= 0.6.0'}
     dev: true
 
-  /promise-inflight@1.0.1:
-    resolution: {integrity: sha512-6zWPyEOFaQBJYcGMHBKTKJ3u6TBsnMFOIZSa6ce1e/ZrrsOlnHRHbabMjLiBYKp+n44X9eUI6VUPaukCXHuG4g==}
-    peerDependencies:
-      bluebird: '*'
-    peerDependenciesMeta:
-      bluebird:
-        optional: true
-    dev: true
-
   /prompts@2.4.2:
     resolution: {integrity: sha512-NxNv/kLguCA7p3jE8oL2aEBsrJWgAakBpgmgK6lpPWV+WuOmY6r2/zbAVnP+T8bQlA0nzHXSJSJW0Hq7ylaD2Q==}
     engines: {node: '>= 6'}
     dependencies:
       kleur: 3.0.3
       sisteransi: 1.0.5
 
@@ -5871,15 +5741,14 @@
 
   /punycode@2.3.0:
     resolution: {integrity: sha512-rRV+zQD8tVFys26lAGR9WUuS4iUAngJScM+ZRSKtvl5tKeZ2t5bvdNFdNHBW9FWR4guGHlgmsZ1G7BSm2wTbuA==}
     engines: {node: '>=6'}
 
   /querystringify@2.2.0:
     resolution: {integrity: sha512-FIqgj2EUvTa7R50u0rGsyTftzjYmv/a3hO345bZNrqabNqjtgiDMgmo4mkUjd+nzU5oF3dClKqFIPUKybUyqoQ==}
-    dev: false
 
   /queue-microtask@1.2.3:
     resolution: {integrity: sha512-NuaNSa6flKT5JaSYQzJok04JzTL1CA6aGhv5rfLW3PgqA+M2ChpZQnAC8h8i4ZFkBS8X5RqkDBHA7r4hej3K9A==}
 
   /quick-lru@4.0.1:
     resolution: {integrity: sha512-ARhCpm70fzdcvNQfPoy49IaanKkTlRWF2JMzqhcJbhSFRZv7nPTvZJdcY7301IPmvW+/p0RgIWnQDLJxifsQ7g==}
     engines: {node: '>=8'}
@@ -5887,25 +5756,14 @@
 
   /randombytes@2.1.0:
     resolution: {integrity: sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==}
     dependencies:
       safe-buffer: 5.2.1
     dev: true
 
-  /raw-loader@4.0.2(webpack@5.88.0):
-    resolution: {integrity: sha512-ZnScIV3ag9A4wPX/ZayxL/jZH+euYb6FcUinPcgiQW0+UBtEv0O6Q3lGd3cqJ+GHH+rksEv3Pj99oxJ3u3VIKA==}
-    engines: {node: '>= 10.13.0'}
-    peerDependencies:
-      webpack: ^4.0.0 || ^5.0.0
-    dependencies:
-      loader-utils: 2.0.4
-      schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-    dev: true
-
   /react-dom@18.2.0(react@18.2.0):
     resolution: {integrity: sha512-6IMTriUmvsjHUjNtEDudZfuDQUoWXVxKHhlEGSk81n4YFS+r/Kl99wXiwlVXtPBtJenozv2P+hxDsw9eA7Xo6g==}
     peerDependencies:
       react: ^18.2.0
     dependencies:
       loose-envify: 1.4.0
       react: 18.2.0
@@ -5968,17 +5826,17 @@
 
   /readdirp@3.6.0:
     resolution: {integrity: sha512-hOS089on8RduqdbhvQ5Z37A0ESjsqz6qnRcffsMU3495FuTdqSm+7bhJ29JvIOsBDEEnan5DPu9t3To9VRlMzA==}
     engines: {node: '>=8.10.0'}
     dependencies:
       picomatch: 2.3.1
 
-  /rechoir@0.7.1:
-    resolution: {integrity: sha512-/njmZ8s1wVeR6pjTZ+0nCnv8SpZNRMT2D1RLOJQESlYFDBvwpTA4KWJpZ+sBJ4+vhjILRcK7JIFdGCdxEAAitg==}
-    engines: {node: '>= 0.10'}
+  /rechoir@0.8.0:
+    resolution: {integrity: sha512-/vxpCXddiX8NGfGO/mTafwjq4aFa/71pvamip0++IQk3zG8cbCj0fifNPrjjF1XMXUne91jL9OoxmdykoEtifQ==}
+    engines: {node: '>= 10.13.0'}
     dependencies:
       resolve: 1.22.2
     dev: true
 
   /redent@3.0.0:
     resolution: {integrity: sha512-6tDA8g98We0zd0GvVeMT9arEOnTw9qM03L9cJXaCjrip1OO764RDBLBfrB4cwzNGDj5OA5ioymC9GkizgWJDUg==}
     engines: {node: '>=8'}
@@ -6084,21 +5942,25 @@
       unist-util-visit: 4.1.2
 
   /require-directory@2.1.1:
     resolution: {integrity: sha512-fGxEI7+wsG9xrvdjsrlmL22OMTTiHRwAMroiEeMgq8gzoLC/PQr7RsRDSTLUg/bZAZtF+TVIkHc6/4RIKrui+Q==}
     engines: {node: '>=0.10.0'}
     dev: true
 
+  /require-from-string@2.0.2:
+    resolution: {integrity: sha512-Xf0nWe6RseziFMu+Ap9biiUbmplq6S9/p+7w7YXP/JBHhrUDDUhwa+vANyubuqfZWTveU//DYVGsDG7RKL/vEw==}
+    engines: {node: '>=0.10.0'}
+    dev: true
+
   /require-main-filename@2.0.0:
     resolution: {integrity: sha512-NKN5kMDylKuldxYLSUfrbo5Tuzh4hd+2E8NPPX02mZtn1VuREQToYe/ZdlJy+J3uCpfaiGF05e7B8W0iXbQHmg==}
     dev: true
 
   /requires-port@1.0.0:
     resolution: {integrity: sha512-KigOCHcocU3XODJxsu8i/j8T9tzT4adHiecwORRQ0ZZFcp7ahwXuRU1m+yuO90C5ZUyGeGfocHDI14M3L3yDAQ==}
-    dev: false
 
   /reselect@4.1.8:
     resolution: {integrity: sha512-ab9EmR80F/zQTMNeneUr4cv+jSwPJgIlvEmVwLerwrWVbpLlBuls9XHzIeTFy4cegU2NHBp3va0LKOzU5qFEYQ==}
     dev: false
 
   /resolve-cwd@3.0.0:
     resolution: {integrity: sha512-OrZaX2Mb+rJCpH/6CpSqt9xFVpN++x01XnN2ie9g6P5/3xelLAkXWVADpdz1IHD/KFfEXyE6V0U01OQ3UO2rEg==}
@@ -6158,21 +6020,14 @@
       retext-stringify: 3.1.0
       unified: 10.1.2
 
   /reusify@1.0.4:
     resolution: {integrity: sha512-U9nH88a3fc/ekCF1l0/UP1IosiuIjyTh7hBvXVMHYgVcfGvt897Xguj2UOLDeI5BG2m7/uwyaLVT6fbtCwTyzw==}
     engines: {iojs: '>=1.0.0', node: '>=0.10.0'}
 
-  /rimraf@3.0.2:
-    resolution: {integrity: sha512-JZkJMZkAGFFPP2YqXZXPbMlMBgsxzE8ILs4lMIX/2o0L9UBw9O/Y3o6wFw/i9YLapcUJWwqbi3kdxIPdC62TIA==}
-    hasBin: true
-    dependencies:
-      glob: 7.1.7
-    dev: true
-
   /rollup@3.25.1:
     resolution: {integrity: sha512-tywOR+rwIt5m2ZAWSe5AIJcTat8vGlnPFAv15ycCrw33t6iFsXZ6mzHVFh2psSjxQPmI+xgzMZZizUAukBI4aQ==}
     engines: {node: '>=14.18.0', npm: '>=8.0.0'}
     hasBin: true
     optionalDependencies:
       fsevents: 2.3.2
 
@@ -6207,14 +6062,25 @@
       is-regex: 1.1.4
     dev: true
 
   /safer-buffer@2.1.2:
     resolution: {integrity: sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==}
     dev: true
 
+  /sanitize-html@2.11.0:
+    resolution: {integrity: sha512-BG68EDHRaGKqlsNjJ2xUB7gpInPA8gVx/mvjO743hZaeMCZ2DwzW7xvsqZ+KNU4QKwj86HJ3uu2liISf2qBBUA==}
+    dependencies:
+      deepmerge: 4.3.1
+      escape-string-regexp: 4.0.0
+      htmlparser2: 8.0.2
+      is-plain-object: 5.0.0
+      parse-srcset: 1.0.2
+      postcss: 8.4.24
+    dev: true
+
   /sass-formatter@0.7.6:
     resolution: {integrity: sha512-hXdxU6PCkiV3XAiSnX+XLqz2ohHoEnVUlrd8LEVMAI80uB1+OTScIkH9n6qQwImZpTye1r1WG1rbGUteHNhoHg==}
     dependencies:
       suf-log: 2.5.3
 
   /scheduler@0.23.0:
     resolution: {integrity: sha512-CtuThmgHNg7zIZWAXi3AsyIzA3n4xx7aNyjwC2VJldO2LMVDhFK+63xGqq6CsJH4rTAt6/M+N4GhZiDYPx9eUw==}
@@ -6236,14 +6102,24 @@
     engines: {node: '>= 10.13.0'}
     dependencies:
       '@types/json-schema': 7.0.12
       ajv: 6.12.6
       ajv-keywords: 3.5.2(ajv@6.12.6)
     dev: true
 
+  /schema-utils@4.2.0:
+    resolution: {integrity: sha512-L0jRsrPpjdckP3oPug3/VxNKt2trR8TcabrM6FOAAlvC/9Phcmm+cuAgTlxBqdBR1WJx7Naj9WHw+aOmheSVbw==}
+    engines: {node: '>= 12.13.0'}
+    dependencies:
+      '@types/json-schema': 7.0.12
+      ajv: 8.12.0
+      ajv-formats: 2.1.1(ajv@8.12.0)
+      ajv-keywords: 5.1.0(ajv@8.12.0)
+    dev: true
+
   /section-matter@1.0.0:
     resolution: {integrity: sha512-vfD3pmTzGpufjScBh50YHKzEu2lxBWhVEHsNGoEXmCmn2hKGfeNLYMzCJpe8cD7gqX7TJluOVpBkAequ6dgMmA==}
     engines: {node: '>=4'}
     dependencies:
       extend-shallow: 2.0.1
       kind-of: 6.0.3
 
@@ -6252,27 +6128,21 @@
     hasBin: true
     dev: true
 
   /semver@6.3.0:
     resolution: {integrity: sha512-b39TBaTSfV6yBrapU89p5fKekE2m/NwnDocOVruQFS1/veMgdzuPcnOM34M6CwxW8jH/lxEa5rBoDeUwu5HHTw==}
     hasBin: true
 
-  /semver@7.5.2:
-    resolution: {integrity: sha512-SoftuTROv/cRjCze/scjGyiDtcUyxw1rgYQSZY7XTmtR5hX+dm76iDbTH8TkLPHCQmlbQVSSbNZCPM2hb0knnQ==}
+  /semver@7.5.3:
+    resolution: {integrity: sha512-QBlUtyVk/5EeHbi7X0fw6liDZc7BBmEaSYn01fMU1OUYbf6GPsbTtd8WmnqbI20SeycoHSeiybkE/q1Q+qlThQ==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
       lru-cache: 6.0.0
 
-  /serialize-javascript@5.0.1:
-    resolution: {integrity: sha512-SaaNal9imEO737H2c05Og0/8LUXG7EnsZyMa8MzkmuHoELfT6txuj0cMqRj6zfPKnmQ1yasR4PCJc8x+M4JSPA==}
-    dependencies:
-      randombytes: 2.1.0
-    dev: true
-
   /serialize-javascript@6.0.1:
     resolution: {integrity: sha512-owoXEFjWRllis8/M1Q+Cw5k8ZH40e3zhp/ovX+Xr/vi1qj6QesbyXXViFbpNvWvPNAD62SutwEXavefrLJWj7w==}
     dependencies:
       randombytes: 2.1.0
     dev: true
 
   /server-destroy@1.0.1:
@@ -6374,15 +6244,15 @@
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       data-urls: 2.0.0
       iconv-lite: 0.6.3
       loader-utils: 2.0.4
       schema-utils: 2.7.1
       source-map: 0.6.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
     dev: true
 
   /source-map-support@0.5.21:
     resolution: {integrity: sha512-uBHU3L3czsIyYXKX88fdrGovxdSCoTGDRZ6SYXtSRxLZUzHg5P/66Ht6uoUlHu9EZod+inXhKo3qQgwXUT/y1w==}
     dependencies:
       buffer-from: 1.1.2
       source-map: 0.6.1
@@ -6429,21 +6299,14 @@
   /spdx-license-ids@3.0.13:
     resolution: {integrity: sha512-XkD+zwiqXHikFZm4AX/7JSCXA98U5Db4AFd5XUg/+9UNtnH75+Z9KxtpYiJZx36mUDVOwH83pl7yvCer6ewM3w==}
     dev: true
 
   /sprintf-js@1.0.3:
     resolution: {integrity: sha512-D9cPgkvLlV3t3IzL0D0YLvGA9Ahk4PcvVwUbN0dSGr1aP0Nrt4AEnTUbuGvquEC0mA64Gqt1fzirlRs5ibXx8g==}
 
-  /ssri@8.0.1:
-    resolution: {integrity: sha512-97qShzy1AiyxvPNIkLWoGua7xoQzzPjQ0HAH4B0rWKo7SZ6USuPcrUiAFrws0UH8RrbWmgq3LMTObhPIHbbBeQ==}
-    engines: {node: '>= 8'}
-    dependencies:
-      minipass: 3.3.6
-    dev: true
-
   /stackback@0.0.2:
     resolution: {integrity: sha512-1XMJE5fQo1jGH6Y/7ebnwPOBEkIEnT4QF32d5R1+VXdXveM0IBMJt8zfaxX1P3QhVwrYe+576+jkANtSS2mBbw==}
     dev: true
 
   /std-env@3.3.3:
     resolution: {integrity: sha512-Rz6yejtVyWnVjC1RFvNmYL10kgjC49EOghxWn0RFqlCHGFpQx+Xe7yW3I4ceK1SGrWIGMjD5Kbue8W/udkbMJg==}
     dev: true
@@ -6557,23 +6420,21 @@
 
   /strip-literal@1.0.1:
     resolution: {integrity: sha512-QZTsipNpa2Ppr6v1AmJHESqJ3Uz247MUS0OjrnnZjFAvEoWqxuyFuXn2xLgMtRnijJShAa1HL0gtJyUs7u7n3Q==}
     dependencies:
       acorn: 8.9.0
     dev: true
 
-  /style-loader@2.0.0(webpack@5.88.0):
-    resolution: {integrity: sha512-Z0gYUJmzZ6ZdRUqpg1r8GsaFKypE+3xAzuFeMuoHgjc9KZv3wMyCRjQIWEbhoFSq7+7yoHXySDJyyWQaPajeiQ==}
-    engines: {node: '>= 10.13.0'}
+  /style-loader@3.3.3(webpack@5.88.0):
+    resolution: {integrity: sha512-53BiGLXAcll9maCYtZi2RCQZKa8NQQai5C4horqKyRmHj9H7QmcUyucrH+4KW/gBQbXM2AsB0axoEcFZPlfPcw==}
+    engines: {node: '>= 12.13.0'}
     peerDependencies:
-      webpack: ^4.0.0 || ^5.0.0
+      webpack: ^5.0.0
     dependencies:
-      loader-utils: 2.0.4
-      schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
     dev: true
 
   /style-to-object@0.4.1:
     resolution: {integrity: sha512-HFpbb5gr2ypci7Qw+IOhnP2zOU7e77b+rzM+wTzXzfi1PrtBCX0E7Pk4wL4iTLnhzZ+JgEGAhX81ebTg/aYjQw==}
     dependencies:
       inline-style-parser: 0.1.1
     dev: false
@@ -6621,24 +6482,14 @@
     dependencies:
       has-package-exports: 1.3.0
 
   /supports-preserve-symlinks-flag@1.0.0:
     resolution: {integrity: sha512-ot0WnXS9fgdkgIcePe6RHNk1WA8+muPa6cSjeR3V8K27q9BB1rTE3R1p7Hv0z1ZyAc8s6Vvv8DIyWf681MAt0w==}
     engines: {node: '>= 0.4'}
 
-  /svg-url-loader@6.0.0(webpack@5.88.0):
-    resolution: {integrity: sha512-Qr5SCKxyxKcRnvnVrO3iQj9EX/v40UiGEMshgegzV7vpo3yc+HexELOdtWcA3MKjL8IyZZ1zOdcILmDEa/8JJQ==}
-    peerDependencies:
-      webpack: ^4.0.0 || ^5.0.0
-    dependencies:
-      file-loader: 6.0.0(webpack@5.88.0)
-      loader-utils: 2.0.4
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-    dev: true
-
   /synckit@0.8.5:
     resolution: {integrity: sha512-L1dapNV6vu2s/4Sputv8xGsCdAVlb5nRDMFU/E27D44l5U6cw1g0dGd45uLc+OXjNMmF4ntiMdCimzcjFKQI8Q==}
     engines: {node: ^14.18.0 || >=16.0.0}
     dependencies:
       '@pkgr/utils': 2.4.1
       tslib: 2.5.3
 
@@ -6675,51 +6526,19 @@
     dev: false
 
   /tapable@2.2.1:
     resolution: {integrity: sha512-GNzQvQTOIP6RyTfE2Qxb8ZVlNmw0n88vp1szwWRimP02mnTsx3Wtn5qRdqY9w2XduFNUgvOwhNnQsjwCp+kqaQ==}
     engines: {node: '>=6'}
     dev: true
 
-  /tar@6.1.15:
-    resolution: {integrity: sha512-/zKt9UyngnxIT/EAGYuxaMYgOIJiP81ab9ZfkILq4oNLPFX50qyYmu7jRj9qeXoxmJHjGlbH0+cm2uy1WCs10A==}
-    engines: {node: '>=10'}
-    dependencies:
-      chownr: 2.0.0
-      fs-minipass: 2.1.0
-      minipass: 5.0.0
-      minizlib: 2.1.2
-      mkdirp: 1.0.4
-      yallist: 4.0.0
-    dev: true
-
   /term-size@2.2.1:
     resolution: {integrity: sha512-wK0Ri4fOGjv/XPy8SBHZChl8CM7uMc5VML7SqiQ0zG7+J5Vr+RMQDoHa2CNT6KHUnTGIXH34UDMkPzAUyapBZg==}
     engines: {node: '>=8'}
     dev: true
 
-  /terser-webpack-plugin@4.2.3(webpack@5.88.0):
-    resolution: {integrity: sha512-jTgXh40RnvOrLQNgIkwEKnQ8rmHjHK4u+6UBEi+W+FPmvb+uo+chJXntKe7/3lW5mNysgSWD60KyesnhW8D6MQ==}
-    engines: {node: '>= 10.13.0'}
-    peerDependencies:
-      webpack: ^4.0.0 || ^5.0.0
-    dependencies:
-      cacache: 15.3.0
-      find-cache-dir: 3.3.2
-      jest-worker: 26.6.2
-      p-limit: 3.1.0
-      schema-utils: 3.3.0
-      serialize-javascript: 5.0.1
-      source-map: 0.6.1
-      terser: 5.18.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-      webpack-sources: 1.4.3
-    transitivePeerDependencies:
-      - bluebird
-    dev: true
-
   /terser-webpack-plugin@5.3.9(esbuild@0.18.6)(webpack@5.88.0):
     resolution: {integrity: sha512-ZuXsqE07EcggTWQjXUj+Aot/OMcD0bMKGgF63f7UxYcu5/AJF53aIpK1YoP5xR9l6s/Hy2b+t1AM0bLNPRuhwA==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       '@swc/core': '*'
       esbuild: '*'
       uglify-js: '*'
@@ -6734,15 +6553,15 @@
     dependencies:
       '@jridgewell/trace-mapping': 0.3.18
       esbuild: 0.18.6
       jest-worker: 27.5.1
       schema-utils: 3.3.0
       serialize-javascript: 6.0.1
       terser: 5.18.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
     dev: true
 
   /terser@5.18.1:
     resolution: {integrity: sha512-j1n0Ao919h/Ai5r43VAnfV/7azUYW43GPxK7qSATzrsERfW7+y2QW9Cp9ufnRF5CQUWbnLSo7UJokSWCqg4tsQ==}
     engines: {node: '>=10'}
     hasBin: true
     dependencies:
@@ -6801,20 +6620,14 @@
 
   /to-regex-range@5.0.1:
     resolution: {integrity: sha512-65P7iz6X5yEr1cwcgvQxbbIw7Uk3gOy5dIdtZ4rDveLqhrdJP+Li/Hx6tyK0NEb+2GCyneCMJiGqrADCSNk8sQ==}
     engines: {node: '>=8.0'}
     dependencies:
       is-number: 7.0.0
 
-  /to-string-loader@1.2.0:
-    resolution: {integrity: sha512-KsWUL8FccgBW9FPFm4vYoQbOOcO5m6hKOGYoXjbseD9/4Ft+ravXN5jolQ9kTKYcK4zPt1j+khx97GPGnVoi6A==}
-    dependencies:
-      loader-utils: 1.4.2
-    dev: true
-
   /tr46@0.0.3:
     resolution: {integrity: sha512-N3WMsuqV66lT30CrXNbEjx4GEwlow3v6rr4mCcv6prnfwhS01rkgyFdjPNBYd9br7LpXV1+Emh01fHnq2Gdgrw==}
 
   /tr46@2.1.0:
     resolution: {integrity: sha512-15Ih7phfcdP5YxqiB+iDtLoaTz4Nd35+IiAv0kQ5FNKHzXgdWqPoTIqEDDJmXceQt4JZk6lVPT8lnDlPpGDppw==}
     engines: {node: '>=8'}
     dependencies:
@@ -6910,15 +6723,14 @@
       has-bigints: 1.0.2
       has-symbols: 1.0.3
       which-boxed-primitive: 1.0.2
     dev: true
 
   /underscore@1.13.6:
     resolution: {integrity: sha512-+A5Sja4HP1M08MaXya7p5LvjuM7K6q/2EaC0+iovj/wOcMsTzMvDFbasi/oSapiwOlt252IqsKqPjCl7huKS0A==}
-    dev: false
 
   /undici@5.22.1:
     resolution: {integrity: sha512-Ji2IJhFXZY0x/0tVBXeQwgPlLWw13GVzpsWPQ3rV50IFMMof2I55PZZxtm4P6iNq+L5znYN9nSTAq0ZyE6lSJw==}
     engines: {node: '>=14.0'}
     dependencies:
       busboy: 1.6.0
 
@@ -6932,26 +6744,14 @@
       bail: 2.0.2
       extend: 3.0.2
       is-buffer: 2.0.5
       is-plain-obj: 4.1.0
       trough: 2.1.0
       vfile: 5.3.7
 
-  /unique-filename@1.1.1:
-    resolution: {integrity: sha512-Vmp0jIp2ln35UTXuryvjzkjGdRyf9b2lTXuSYUiPmzRcl3FDtYqAwOnTJkAngD9SWhnoJzDbTKwaOrZ+STtxNQ==}
-    dependencies:
-      unique-slug: 2.0.2
-    dev: true
-
-  /unique-slug@2.0.2:
-    resolution: {integrity: sha512-zoWr9ObaxALD3DOPfjPSqxt4fnZiWblxHIgeWqW8x7UqDzEtHEQLzji2cuJYQFCU6KmoJikOYAZlrTHHebjx2w==}
-    dependencies:
-      imurmurhash: 0.1.4
-    dev: true
-
   /unist-util-generated@2.0.1:
     resolution: {integrity: sha512-qF72kLmPxAw0oN2fwpWIqbXAVyEqUzDHMsbtPvOudIlUzXYFIeQIuxXQCRCFh22B7cixvU0MG7m3MW8FTq/S+A==}
 
   /unist-util-is@5.2.1:
     resolution: {integrity: sha512-u9njyyfEh43npf1M+yGKDGVPbY/JWEemg5nH05ncKPfi+kBbKBJoTdsogMu33uhytuLlv9y0O7GH7fEdwLdLQw==}
     dependencies:
       '@types/unist': 2.0.6
@@ -7028,38 +6828,28 @@
       picocolors: 1.0.0
 
   /uri-js@4.4.1:
     resolution: {integrity: sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==}
     dependencies:
       punycode: 2.3.0
 
-  /url-loader@4.1.1(file-loader@6.0.0)(webpack@5.88.0):
-    resolution: {integrity: sha512-3BTV812+AVHHOJQO8O5MkWgZ5aosP7GnROJwvzLS9hWDj00lZ6Z0wNak423Lp9PBZN05N+Jk/N5Si8jRAlGyWA==}
-    engines: {node: '>= 10.13.0'}
-    peerDependencies:
-      file-loader: '*'
-      webpack: ^4.0.0 || ^5.0.0
-    peerDependenciesMeta:
-      file-loader:
-        optional: true
-    dependencies:
-      file-loader: 6.0.0(webpack@5.88.0)
-      loader-utils: 2.0.4
-      mime-types: 2.1.35
-      schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
-    dev: true
-
   /url-parse@1.4.7:
     resolution: {integrity: sha512-d3uaVyzDB9tQoSXFvuSUNFibTd9zxd2bkVrDRvF5TmvWWQwqE4lgYJ5m+x1DbecWkw+LK4RNl2CU1hHuOKPVlg==}
     dependencies:
       querystringify: 2.2.0
       requires-port: 1.0.0
     dev: false
 
+  /url-parse@1.5.10:
+    resolution: {integrity: sha512-WypcfiRhfeUP9vvF0j6rw0J3hrWrw6iZv3+22h6iRMJ/8z1Tj6XfLP4DsUix5MhMPnXpiHDoKyoZ/bdCkwBCiQ==}
+    dependencies:
+      querystringify: 2.2.0
+      requires-port: 1.0.0
+    dev: true
+
   /util-deprecate@1.0.2:
     resolution: {integrity: sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==}
 
   /uvu@0.5.6:
     resolution: {integrity: sha512-+g8ENReyr8YsOc6fv/NVJs2vFdHBnBNdfE49rshrTzDWOlUx4Gq7KOS2GD8eqhy2j+Ejq29+SbKH8yjkAqXqoA==}
     engines: {node: '>=8'}
     hasBin: true
@@ -7113,48 +6903,14 @@
       - sass
       - stylus
       - sugarss
       - supports-color
       - terser
     dev: true
 
-  /vite@4.1.4(@types/node@18.0.0):
-    resolution: {integrity: sha512-3knk/HsbSTKEin43zHu7jTwYWv81f8kgAL99G5NWBcA1LKvtvcVAC4JjBH1arBunO9kQka+1oGbrMKOjk4ZrBg==}
-    engines: {node: ^14.18.0 || >=16.0.0}
-    hasBin: true
-    peerDependencies:
-      '@types/node': '>= 14'
-      less: '*'
-      sass: '*'
-      stylus: '*'
-      sugarss: '*'
-      terser: ^5.4.0
-    peerDependenciesMeta:
-      '@types/node':
-        optional: true
-      less:
-        optional: true
-      sass:
-        optional: true
-      stylus:
-        optional: true
-      sugarss:
-        optional: true
-      terser:
-        optional: true
-    dependencies:
-      '@types/node': 18.0.0
-      esbuild: 0.16.17
-      postcss: 8.4.24
-      resolve: 1.22.2
-      rollup: 3.25.1
-    optionalDependencies:
-      fsevents: 2.3.2
-    dev: true
-
   /vite@4.3.9(@types/node@18.0.0):
     resolution: {integrity: sha512-qsTNZjO9NoJNW7KnOrgYwczm0WctJ8m/yqYAMAK9Lxt4SoySUfS5S8ia9K7JHpa3KEeMfyF8LoJ3c5NeBJy6pg==}
     engines: {node: ^14.18.0 || >=16.0.0}
     hasBin: true
     peerDependencies:
       '@types/node': '>= 14'
       less: '*'
@@ -7334,46 +7090,44 @@
     dev: true
 
   /webidl-conversions@7.0.0:
     resolution: {integrity: sha512-VwddBukDzu71offAQR975unBIGqfKZpM+8ZX6ySk8nYhVoo5CYaZyzt3YBvYtRtO+aoGlqxPg/B87NGVZ/fu6g==}
     engines: {node: '>=12'}
     dev: true
 
-  /webpack-cli@4.10.0(webpack@5.88.0):
-    resolution: {integrity: sha512-NLhDfH/h4O6UOy+0LSso42xvYypClINuMNBVVzX4vX98TmTaTUxwRbXdhucbFMd2qLaCTcLq/PdYrvi8onw90w==}
-    engines: {node: '>=10.13.0'}
+  /webpack-cli@5.1.4(webpack@5.88.0):
+    resolution: {integrity: sha512-pIDJHIEI9LR0yxHXQ+Qh95k2EvXpWzZ5l+d+jIo+RdSm9MiHfzazIxwwni/p7+x4eJZuvG1AJwgC4TNQ7NRgsg==}
+    engines: {node: '>=14.15.0'}
     hasBin: true
     peerDependencies:
       '@webpack-cli/generators': '*'
-      '@webpack-cli/migrate': '*'
-      webpack: 4.x.x || 5.x.x
+      webpack: 5.x.x
       webpack-bundle-analyzer: '*'
       webpack-dev-server: '*'
     peerDependenciesMeta:
       '@webpack-cli/generators':
         optional: true
-      '@webpack-cli/migrate':
-        optional: true
       webpack-bundle-analyzer:
         optional: true
       webpack-dev-server:
         optional: true
     dependencies:
       '@discoveryjs/json-ext': 0.5.7
-      '@webpack-cli/configtest': 1.2.0(webpack-cli@4.10.0)(webpack@5.88.0)
-      '@webpack-cli/info': 1.5.0(webpack-cli@4.10.0)
-      '@webpack-cli/serve': 1.7.0(webpack-cli@4.10.0)
+      '@webpack-cli/configtest': 2.1.1(webpack-cli@5.1.4)(webpack@5.88.0)
+      '@webpack-cli/info': 2.0.2(webpack-cli@5.1.4)(webpack@5.88.0)
+      '@webpack-cli/serve': 2.0.5(webpack-cli@5.1.4)(webpack@5.88.0)
       colorette: 2.0.20
-      commander: 7.2.0
+      commander: 10.0.1
       cross-spawn: 7.0.3
+      envinfo: 7.9.0
       fastest-levenshtein: 1.0.16
       import-local: 3.1.0
-      interpret: 2.2.0
-      rechoir: 0.7.1
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      interpret: 3.1.1
+      rechoir: 0.8.0
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
       webpack-merge: 5.9.0
     dev: true
 
   /webpack-merge@5.9.0:
     resolution: {integrity: sha512-6NbRQw4+Sy50vYNTw7EyOn41OZItPiXB8GNv3INSoe3PSFaHJEz3SHTrYVaRm2LilNGnFUzh0FAwqPEmU/CwDg==}
     engines: {node: '>=10.0.0'}
     dependencies:
@@ -7389,15 +7143,15 @@
     dev: true
 
   /webpack-sources@3.2.3:
     resolution: {integrity: sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==}
     engines: {node: '>=10.13.0'}
     dev: true
 
-  /webpack@5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0):
+  /webpack@5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4):
     resolution: {integrity: sha512-O3jDhG5e44qIBSi/P6KpcCcH7HD+nYIHVBhdWFxcLOcIGN8zGo5nqF3BjyNCxIh4p1vFdNnreZv2h2KkoAw3lw==}
     engines: {node: '>=10.13.0'}
     hasBin: true
     peerDependencies:
       webpack-cli: '*'
     peerDependenciesMeta:
       webpack-cli:
@@ -7422,15 +7176,15 @@
       loader-runner: 4.3.0
       mime-types: 2.1.35
       neo-async: 2.6.2
       schema-utils: 3.3.0
       tapable: 2.2.1
       terser-webpack-plugin: 5.3.9(esbuild@0.18.6)(webpack@5.88.0)
       watchpack: 2.4.0
-      webpack-cli: 4.10.0(webpack@5.88.0)
+      webpack-cli: 5.1.4(webpack@5.88.0)
       webpack-sources: 3.2.3
     transitivePeerDependencies:
       - '@swc/core'
       - esbuild
       - uglify-js
     dev: true
 
@@ -7544,15 +7298,15 @@
     resolution: {integrity: sha512-XQyQkIFeRVC7f7uRhFdNMe/iJOdO6zxAaR3EWbDp45v3mDhrTi+++oswKNxShUNjPC/1xUp5DB29YKLhFo129g==}
     engines: {node: '>= 10.13.0'}
     peerDependencies:
       webpack: ^4.0.0 || ^5.0.0
     dependencies:
       loader-utils: 2.0.4
       schema-utils: 3.3.0
-      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@4.10.0)
+      webpack: 5.88.0(esbuild@0.18.6)(webpack-cli@5.1.4)
     dev: true
 
   /wrap-ansi@6.2.0:
     resolution: {integrity: sha512-r6lPcBGxZXlIcymEu7InxDMhdW0KDxpLgoFLcguasxCaJ/SOIZwINatK9KY/tf+ZrlywOKU0UDj3ATXUBfxJXA==}
     engines: {node: '>=8'}
     dependencies:
       ansi-styles: 4.3.0
@@ -7587,15 +7341,14 @@
       bufferutil: ^4.0.1
       utf-8-validate: ^5.0.2
     peerDependenciesMeta:
       bufferutil:
         optional: true
       utf-8-validate:
         optional: true
-    dev: false
 
   /y18n@4.0.3:
     resolution: {integrity: sha512-JKhqTOwSrqNA1NY5lSztJ1GrBiUodLMmIZuLiDaMRJ+itFd+ABVE8XBjOvIWL+rSqNDC74LCSFmlb/U4UZ4hJQ==}
     dev: true
 
   /y18n@5.0.8:
     resolution: {integrity: sha512-0pfFzegeDWJHJIAmTLRP2DwHjdF5s7jo9tuztdQxAhINCdvS+3nGINqPd00AphqJR/0LhANUS6/+7SCb98YOfA==}
```

### Comparing `anywidget-0.5.3/anywidget/_descriptor.py` & `anywidget-0.6.0/anywidget/_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/anywidget/_file_contents.py` & `anywidget-0.6.0/anywidget/_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/anywidget/_protocols.py` & `anywidget-0.6.0/anywidget/_protocols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Sequence
+from typing import TYPE_CHECKING, Literal, Protocol, Sequence
 
-from typing_extensions import Literal, Protocol, TypedDict
+from typing_extensions import TypedDict
 
 if TYPE_CHECKING:
     from ._descriptor import MimeBundleDescriptor
 
 
 class UpdateData(TypedDict):
     method: Literal["update"]
```

### Comparing `anywidget-0.5.3/anywidget/_util.py` & `anywidget-0.6.0/anywidget/_util.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/anywidget/experimental.py` & `anywidget-0.6.0/anywidget/experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/anywidget/widget.py` & `anywidget-0.6.0/anywidget/widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/anywidget/labextension/package.json` & `anywidget-0.6.0/anywidget/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9314903846153846%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^4.0.2', '@jupyter-widgets/base-manager': "*

 * *                      "'^1.0.5'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.cba6b4061725caaf22a8.js'}}",*

 * * "'version'": "'0.6.0'"}*

```diff
@@ -2,15 +2,16 @@
     "author": "Trevor Manz",
     "dependencies": {
         "@anywidget/types": "workspace:~",
         "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
-        "@jupyterlab/builder": "^3.6.4"
+        "@jupyter-widgets/base-manager": "^1.0.5",
+        "@jupyterlab/builder": "^4.0.2"
     },
     "exports": {
         ".": "./dist/index.js",
         "./types": {
             "import": "./dist/types.mjs",
             "require": "./dist/types.cjs",
             "types": "./dist/types.d.ts"
@@ -22,15 +23,15 @@
     },
     "files": [
         "dist"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.06234e67efd98a0438df.js"
+            "load": "static/remoteEntry.cba6b4061725caaf22a8.js"
         },
         "extension": "src/plugin",
         "outputDir": "../../anywidget/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -44,9 +45,9 @@
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs",
         "typecheck": "tsc --noEmit"
     },
     "type": "module",
-    "version": "0.5.3"
+    "version": "0.6.0"
 }
```

### Comparing `anywidget-0.5.3/anywidget/labextension/static/138.ac38585aaafa27f6d52e.js` & `anywidget-0.6.0/anywidget/labextension/static/138.3fd6605047ad3df65a9e.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -117,11 +117,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.3"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.5.3/anywidget/labextension/static/326.cde4b6122e4ffce92951.js` & `anywidget-0.6.0/anywidget/labextension/static/326.c68678f64e2971595925.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -135,11 +135,11 @@
                             return await this._anywidget_cached_cleanup(), super.remove()
                         }
                     }
                 }
             }
         },
         147: e => {
-            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.5.3"}')
+            e.exports = JSON.parse('{"u2":"anywidget","i8":"0.6.0"}')
         }
     }
 ]);
```

### Comparing `anywidget-0.5.3/anywidget/labextension/static/remoteEntry.06234e67efd98a0438df.js` & `anywidget-0.6.0/anywidget/labextension/static/remoteEntry.cba6b4061725caaf22a8.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -41,19 +41,19 @@
         }), r
     }, m.d = (e, r) => {
         for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        138: "ac38585aaafa27f6d52e",
-        326: "cde4b6122e4ffce92951"
+        138: "3fd6605047ad3df65a9e",
+        326: "c68678f64e2971595925"
     } [e] + ".js?v=" + {
-        138: "ac38585aaafa27f6d52e",
-        326: "cde4b6122e4ffce92951"
+        138: "3fd6605047ad3df65a9e",
+        326: "c68678f64e2971595925"
     } [e], m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
@@ -104,15 +104,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => m.e(138).then((() => () => m(138))),
                         from: i,
                         eager: !1
                     })
-                })("anywidget", "0.5.3"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("anywidget", "0.6.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         m.g.importScripts && (e = m.g.location + "");
         var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `anywidget-0.5.3/anywidget/nbextension/index.js` & `anywidget-0.6.0/anywidget/nbextension/index.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 // package.json
 var name = "anywidget";
-var version = "0.5.3";
+var version = "0.6.0";
 
 // src/widget.js
 function is_href(str) {
     return str.startsWith("http://") || str.startsWith("https://");
 }
 async function load_css_href(href, anywidget_id) {
     let prev = document.querySelector(`link[id='${anywidget_id}']`);
@@ -76,14 +76,15 @@
 
 function extract_context(view) {
     let model = {
         get: view.model.get.bind(view.model),
         set: view.model.set.bind(view.model),
         save_changes: view.model.save_changes.bind(view.model),
         send: view.model.send.bind(view.model),
+        // @ts-expect-error
         on(name2, callback) {
             view.model.on(name2, callback, view);
         },
         off(name2, callback) {
             view.model.off(name2, callback, view);
         }
     };
```

### Comparing `anywidget-0.5.3/docs/README.md` & `anywidget-0.6.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/astro.config.js` & `anywidget-0.6.0/docs/astro.config.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/package.json` & `anywidget-0.6.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/anywidget-overview.png` & `anywidget-0.6.0/docs/public/anywidget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/banner-dark.png` & `anywidget-0.6.0/docs/public/banner-dark.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/banner-light.png` & `anywidget-0.6.0/docs/public/banner-light.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/banner-minimal.png` & `anywidget-0.6.0/docs/public/banner-minimal.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/client-js-diagram.png` & `anywidget-0.6.0/docs/public/client-js-diagram.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/default-og-image.png` & `anywidget-0.6.0/docs/public/default-og-image.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/favicon.svg` & `anywidget-0.6.0/docs/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/public/widget-overview.png` & `anywidget-0.6.0/docs/public/widget-overview.png`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/scripts/ipynb.mjs` & `anywidget-0.6.0/docs/scripts/ipynb.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/scripts/utils.mjs` & `anywidget-0.6.0/docs/scripts/utils.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/consts.ts` & `anywidget-0.6.0/docs/src/consts.ts`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/CodeHero.astro` & `anywidget-0.6.0/docs/src/components/CodeHero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/CounterButton.astro` & `anywidget-0.6.0/docs/src/components/CounterButton.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/HeadCommon.astro` & `anywidget-0.6.0/docs/src/components/HeadCommon.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/HeadSEO.astro` & `anywidget-0.6.0/docs/src/components/HeadSEO.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Hero.astro` & `anywidget-0.6.0/docs/src/components/Hero.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Footer/AvatarList.astro` & `anywidget-0.6.0/docs/src/components/Footer/AvatarList.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/AnyWidgetLogo.astro` & `anywidget-0.6.0/docs/src/components/Header/AnyWidgetLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/AstroLogo.astro` & `anywidget-0.6.0/docs/src/components/Header/AstroLogo.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/Header.astro` & `anywidget-0.6.0/docs/src/components/Header/Header.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/HeaderButton.css` & `anywidget-0.6.0/docs/src/components/Header/HeaderButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/LanguageSelect.css` & `anywidget-0.6.0/docs/src/components/Header/LanguageSelect.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/LanguageSelect.tsx` & `anywidget-0.6.0/docs/src/components/Header/LanguageSelect.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/Search.css` & `anywidget-0.6.0/docs/src/components/Header/Search.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/Search.tsx` & `anywidget-0.6.0/docs/src/components/Header/Search.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/SidebarToggle.tsx` & `anywidget-0.6.0/docs/src/components/Header/SidebarToggle.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/ThemeToggleButton.css` & `anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/Header/ThemeToggleButton.tsx` & `anywidget-0.6.0/docs/src/components/Header/ThemeToggleButton.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/LeftSidebar/LeftSidebar.astro` & `anywidget-0.6.0/docs/src/components/LeftSidebar/LeftSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/PageContent/PageContent.astro` & `anywidget-0.6.0/docs/src/components/PageContent/PageContent.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/RightSidebar/MoreMenu.astro` & `anywidget-0.6.0/docs/src/components/RightSidebar/MoreMenu.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/RightSidebar/RightSidebar.astro` & `anywidget-0.6.0/docs/src/components/RightSidebar/RightSidebar.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/RightSidebar/TableOfContents.tsx` & `anywidget-0.6.0/docs/src/components/RightSidebar/TableOfContents.tsx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/components/examples/Counter.astro` & `anywidget-0.6.0/docs/src/components/examples/Counter.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/layouts/MainLayout.astro` & `anywidget-0.6.0/docs/src/layouts/MainLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/layouts/SplashLayout.astro` & `anywidget-0.6.0/docs/src/layouts/SplashLayout.astro`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/blog/anywidget-02.md` & `anywidget-0.6.0/docs/src/pages/blog/anywidget-02.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/blog/introducing-anywidget.mdx` & `anywidget-0.6.0/docs/src/pages/blog/introducing-anywidget.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/en/bundling.md` & `anywidget-0.6.0/docs/src/pages/en/bundling.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/en/experimental.md` & `anywidget-0.6.0/docs/src/pages/en/experimental.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/en/getting-started.mdx` & `anywidget-0.6.0/docs/src/pages/en/getting-started.mdx`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/en/jupyter-widgets-the-good-parts.md` & `anywidget-0.6.0/docs/src/pages/en/jupyter-widgets-the-good-parts.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/pages/en/notebooks/counter.ipynb` & `anywidget-0.6.0/docs/src/pages/en/notebooks/counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/styles/index.css` & `anywidget-0.6.0/docs/src/styles/index.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/docs/src/styles/theme.css` & `anywidget-0.6.0/docs/src/styles/theme.css`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/examples/Counter.ipynb` & `anywidget-0.6.0/examples/Counter.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/examples/minimal_example.ipynb` & `anywidget-0.6.0/examples/minimal_example.ipynb`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/packages/anywidget/CHANGELOG.md` & `anywidget-0.6.0/packages/anywidget/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 # anywidget
 
+## 0.6.0
+
+### Minor Changes
+
+- feat!: Drop support for Python 3.7 ([#161](https://github.com/manzt/anywidget/pull/161))
+
+### Patch Changes
+
+- Updated dependencies [[`272782b`](https://github.com/manzt/anywidget/commit/272782bb919355854cf23ccba430c87b7cc28523)]:
+  - @anywidget/types@0.1.3
+
 ## 0.5.3
 
 ### Patch Changes
 
 - Updated dependencies [[`581e40c`](https://github.com/manzt/anywidget/commit/581e40cd10e2440c574ff0e3b51bc5fd7b85b391)]:
   - @anywidget/types@0.1.2
```

### Comparing `anywidget-0.5.3/packages/anywidget/build.mjs` & `anywidget-0.6.0/packages/anywidget/build.mjs`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/packages/anywidget/package.json` & `anywidget-0.6.0/packages/anywidget/package.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9326923076923077%*

 * *Differences: {"'devDependencies'": "{'@jupyterlab/builder': '^4.0.2', '@jupyter-widgets/base-manager': "*

 * *                      "'^1.0.5'}",*

 * * "'version'": "'0.6.0'"}*

```diff
@@ -2,15 +2,16 @@
     "author": "Trevor Manz",
     "dependencies": {
         "@anywidget/types": "workspace:~",
         "@anywidget/vite": "workspace:~",
         "@jupyter-widgets/base": "^2 || ^3 || ^4 || ^5 || ^6"
     },
     "devDependencies": {
-        "@jupyterlab/builder": "^3.6.4"
+        "@jupyter-widgets/base-manager": "^1.0.5",
+        "@jupyterlab/builder": "^4.0.2"
     },
     "exports": {
         ".": "./dist/index.js",
         "./types": {
             "import": "./dist/types.mjs",
             "require": "./dist/types.cjs",
             "types": "./dist/types.d.ts"
@@ -40,9 +41,9 @@
         "main": "dist/index.js"
     },
     "scripts": {
         "build": "node build.mjs",
         "typecheck": "tsc --noEmit"
     },
     "type": "module",
-    "version": "0.5.3"
+    "version": "0.6.0"
 }
```

### Comparing `anywidget-0.5.3/packages/anywidget/src/plugin.js` & `anywidget-0.6.0/packages/anywidget/src/plugin.js`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/packages/anywidget/src/widget.js` & `anywidget-0.6.0/packages/anywidget/src/widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -114,14 +114,15 @@
 function extract_context(view) {
     /** @type {import("@anywidget/types").AnyModel} */
     let model = {
         get: view.model.get.bind(view.model),
         set: view.model.set.bind(view.model),
         save_changes: view.model.save_changes.bind(view.model),
         send: view.model.send.bind(view.model),
+        // @ts-expect-error
         on(name, callback) {
             view.model.on(name, callback, view);
         },
         off(name, callback) {
             view.model.off(name, callback, view);
         },
     };
```

### Comparing `anywidget-0.5.3/tests/test_descriptor.py` & `anywidget-0.6.0/tests/test_descriptor.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/tests/test_experimental.py` & `anywidget-0.6.0/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/tests/test_file_contents.py` & `anywidget-0.6.0/tests/test_file_contents.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/tests/test_utils.py` & `anywidget-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/tests/test_widget.py` & `anywidget-0.6.0/tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/LICENSE` & `anywidget-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/README.md` & `anywidget-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `anywidget-0.5.3/pyproject.toml` & `anywidget-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
-requires = ["hatchling", "jupyterlab==3.*"]
+requires = ["hatchling", "jupyterlab==4.*"]
 build-backend = "hatchling.build"
 
 [project]
 name = "anywidget"
 description = "custom jupyter widgets made easy"
 authors = [
     { name = "Trevor Manz", email = "trevor.j.manz@gmail.com" }
 ]
 license = { text = "MIT" }
 dynamic = ["version"]
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "ipywidgets>=7.6.0",
-    "importlib-metadata; python_version < '3.8'",
     "typing-extensions>=4.2.0",
     "psygnal>=0.8.1",
 ]
 
 [project.optional-dependencies]
 test = [
     "black[jupyter]",
     "pydantic",
     "pytest",
     "pytest-cov",
     "ruff",
-    "msgspec; python_version > '3.7'",
+    "msgspec",
     "ipython<8.13; python_version < '3.9'",
 ]
 dev = [
     "comm>=0.1.0",
     "watchfiles>=0.18.0",
 ]
 
@@ -81,15 +80,15 @@
 fmt = "black ."
 lint = "ruff ."
 test = "pytest . --cov anywidget --cov-report term-missing"
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
-target-version = "py37"
+target-version = "py38"
 src = ["anywidget", "tests"]
 extend-select = [
     "E",    # style errors
     "F",    # flakes
     "D",    # pydocstyle
     "I",    # isort
     "UP",   # pyupgrade
```

### Comparing `anywidget-0.5.3/PKG-INFO` & `anywidget-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: anywidget
-Version: 0.5.3
+Version: 0.6.0
 Summary: custom jupyter widgets made easy
 Project-URL: homepage, https://github.com/manzt/anywidget
 Author-email: Trevor Manz <trevor.j.manz@gmail.com>
 License: MIT
 License-File: LICENSE
-Requires-Python: >=3.7
-Requires-Dist: importlib-metadata; python_version < '3.8'
+Requires-Python: >=3.8
 Requires-Dist: ipywidgets>=7.6.0
 Requires-Dist: psygnal>=0.8.1
 Requires-Dist: typing-extensions>=4.2.0
 Provides-Extra: dev
 Requires-Dist: comm>=0.1.0; extra == 'dev'
 Requires-Dist: watchfiles>=0.18.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black[jupyter]; extra == 'test'
 Requires-Dist: ipython<8.13; python_version < '3.9' and extra == 'test'
-Requires-Dist: msgspec; python_version > '3.7' and extra == 'test'
+Requires-Dist: msgspec; extra == 'test'
 Requires-Dist: pydantic; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 # anywidget <a href="https://github.com/manzt/anywidget"><img align="right" src="https://raw.githubusercontent.com/manzt/anywidget/main/docs/public/favicon.svg" height="38"></img></a>
```

