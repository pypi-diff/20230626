# Comparing `tmp/starlette_admin-0.9.0.tar.gz` & `tmp/starlette_admin-0.9.0.dev0.tar.gz`

## Comparing `starlette_admin-0.9.0.tar` & `starlette_admin-0.9.0.dev0.tar`

### file list

```diff
@@ -1,131 +1,131 @@
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/__init__.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/_types.py
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/actions.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/auth.py
--rw-r--r--   0        0        0    21467 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/base.py
--rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/converters.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/exceptions.py
--rw-r--r--   0        0        0    40050 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/fields.py
--rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/helpers.py
--rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/i18n.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/py.typed
--rw-r--r--   0        0        0    27613 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/__init__.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/__init__.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/admin.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/converters.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/exceptions.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/fields.py
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/helpers.py
--rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/view.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/__init__.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/admin.py
--rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/converters.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/exceptions.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/helpers.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/middleware.py
--rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/odmantic/view.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/__init__.py
--rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/admin.py
--rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/converters.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/exceptions.py
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/fields.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/helpers.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/middleware.py
--rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/view.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/ext/__init__.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqla/ext/pydantic.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqlmodel/__init__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqlmodel/admin.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/contrib/sqlmodel/view.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/dt.checkboxes.css
--rw-r--r--   0        0        0    38335 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/dt.min.css
--rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/flatpickr.min.css
--rw-r--r--   0        0        0    99674 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/fontawesome.min.css
--rw-r--r--   0        0        0    35418 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/jsoneditor.min.css
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/select2.min.css
--rw-r--r--   0        0        0   498576 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/tabler.min.css
--rw-r--r--   0        0        0    31482 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/css/img/jsoneditor-icons.svg
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/i18n/dt/README.md
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/i18n/dt/en.json
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/i18n/dt/fr.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/i18n/flatpickr/fr.js
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/i18n/momentjs/fr.js
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/displays.js
--rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/form.js
--rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/list.js
--rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/render.js
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/utils.js
--rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/dt.checkboxes.js
--rw-r--r--   0        0        0   354520 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/dt.min.js
--rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/dt.searchHighlight.js
--rw-r--r--   0        0        0    50680 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/flatpickr.min.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/jquery.min.js
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/js.cookie.min.js
--rw-r--r--   0        0        0   890454 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/jsoneditor.min.js
--rw-r--r--   0        0        0    59517 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/moment.min.js
--rw-r--r--   0        0        0   970347 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/pdfmake.min.js
--rw-r--r--   0        0        0    73164 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/select2.min.js
--rw-r--r--   0        0        0   146912 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/tabler.min.js
--rw-r--r--   0        0        0   870285 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/js/vendor/vfs_fonts.js
--rw-r--r--   0        0        0   187208 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   108020 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    63952 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24948 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   394628 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150124 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/base.html
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/create.html
--rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/detail.html
--rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/edit.html
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/error.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/index.html
--rw-r--r--   0        0        0    14329 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/layout.html
--rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/list.html
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/login.html
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/_empty.html
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/_null.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/boolean.html
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/collection.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/email.html
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/file.html
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/image.html
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/json.html
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/list.html
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/relation.html
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/text.html
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/tinymce.html
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/displays/url.html
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/_delete.html
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/_error.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/_label.html
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/boolean.html
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/collection.html
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/enum.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/file.html
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/image.html
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/input.html
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/json.html
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/list.html
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/relation.html
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/tags.html
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/forms/textarea.html
--rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/macros/views.html
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/modals/actions.html
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/modals/delete.html
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/modals/error.html
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/templates/modals/loading.html
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/translations/en/LC_MESSAGES/admin.mo
--rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/translations/en/LC_MESSAGES/admin.po
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo
--rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/translations/fr/LC_MESSAGES/admin.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/utils/__init__.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/utils/countries.py
--rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/starlette_admin/utils/timezones.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/LICENSE
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/README.md
--rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7340 2020-02-02 00:00:00.000000 starlette_admin-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/__init__.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/_types.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/actions.py
+-rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/auth.py
+-rw-r--r--   0        0        0    21467 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/base.py
+-rw-r--r--   0        0        0     8179 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/converters.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/exceptions.py
+-rw-r--r--   0        0        0    40050 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/fields.py
+-rw-r--r--   0        0        0     3696 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/helpers.py
+-rw-r--r--   0        0        0     5274 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/i18n.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/py.typed
+-rw-r--r--   0        0        0    27613 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/__init__.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/admin.py
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/converters.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/exceptions.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/fields.py
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/helpers.py
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/view.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/__init__.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/admin.py
+-rw-r--r--   0        0        0     4531 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/converters.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/exceptions.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/helpers.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/middleware.py
+-rw-r--r--   0        0        0    10075 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/view.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/__init__.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/admin.py
+-rw-r--r--   0        0        0    13375 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/converters.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/exceptions.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/fields.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/helpers.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/middleware.py
+-rw-r--r--   0        0        0    16404 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/view.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/ext/__init__.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/ext/pydantic.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqlmodel/__init__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqlmodel/admin.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqlmodel/view.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/dt.checkboxes.css
+-rw-r--r--   0        0        0    38335 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/dt.min.css
+-rw-r--r--   0        0        0    16167 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/flatpickr.min.css
+-rw-r--r--   0        0        0    99674 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/fontawesome.min.css
+-rw-r--r--   0        0        0    35418 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/jsoneditor.min.css
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/select2.min.css
+-rw-r--r--   0        0        0   498576 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/tabler.min.css
+-rw-r--r--   0        0        0    31482 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/css/img/jsoneditor-icons.svg
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/dt/README.md
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/dt/en.json
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/dt/fr.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/flatpickr/fr.js
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/momentjs/fr.js
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/displays.js
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/form.js
+-rw-r--r--   0        0        0    16174 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/list.js
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/render.js
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/utils.js
+-rw-r--r--   0        0        0    13295 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/dt.checkboxes.js
+-rw-r--r--   0        0        0   354520 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/dt.min.js
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/dt.searchHighlight.js
+-rw-r--r--   0        0        0    50680 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/flatpickr.min.js
+-rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/jquery.min.js
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/js.cookie.min.js
+-rw-r--r--   0        0        0   890454 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/jsoneditor.min.js
+-rw-r--r--   0        0        0    59517 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/moment.min.js
+-rw-r--r--   0        0        0   970347 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/pdfmake.min.js
+-rw-r--r--   0        0        0    73164 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/select2.min.js
+-rw-r--r--   0        0        0   146912 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/tabler.min.js
+-rw-r--r--   0        0        0   870285 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/vfs_fonts.js
+-rw-r--r--   0        0        0   187208 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   108020 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    63952 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24948 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   394628 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150124 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10172 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/base.html
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/create.html
+-rw-r--r--   0        0        0     6509 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/detail.html
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/edit.html
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/error.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/index.html
+-rw-r--r--   0        0        0    14329 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/layout.html
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/list.html
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/login.html
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/_empty.html
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/_null.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/boolean.html
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/collection.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/email.html
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/file.html
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/image.html
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/json.html
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/list.html
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/relation.html
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/text.html
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/tinymce.html
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/url.html
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/_delete.html
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/_error.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/_label.html
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/boolean.html
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/collection.html
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/enum.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/file.html
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/image.html
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/input.html
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/json.html
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/list.html
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/relation.html
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/tags.html
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/textarea.html
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/macros/views.html
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/actions.html
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/delete.html
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/error.html
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/loading.html
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.mo
+-rw-r--r--   0        0        0     4507 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.po
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo
+-rw-r--r--   0        0        0     5214 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/utils/__init__.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/utils/countries.py
+-rw-r--r--   0        0        0    10147 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/starlette_admin/utils/timezones.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/LICENSE
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/README.md
+-rw-r--r--   0        0        0     6253 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7345 2020-02-02 00:00:00.000000 starlette_admin-0.9.0.dev0/PKG-INFO
```

### Comparing `starlette_admin-0.9.0/starlette_admin/__init__.py` & `starlette_admin-0.9.0.dev0/starlette_admin/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0"
+__version__ = "0.9.0.dev0"
 
 from ._types import ExportType, RequestAction
 from .actions import action
 from .base import BaseAdmin
 from .fields import (
     ArrowField,
     BaseField,
```

### Comparing `starlette_admin-0.9.0/starlette_admin/_types.py` & `starlette_admin-0.9.0.dev0/starlette_admin/_types.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/actions.py` & `starlette_admin-0.9.0.dev0/starlette_admin/actions.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/auth.py` & `starlette_admin-0.9.0.dev0/starlette_admin/auth.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/base.py` & `starlette_admin-0.9.0.dev0/starlette_admin/base.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/converters.py` & `starlette_admin-0.9.0.dev0/starlette_admin/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/exceptions.py` & `starlette_admin-0.9.0.dev0/starlette_admin/exceptions.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/fields.py` & `starlette_admin-0.9.0.dev0/starlette_admin/fields.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/helpers.py` & `starlette_admin-0.9.0.dev0/starlette_admin/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/i18n.py` & `starlette_admin-0.9.0.dev0/starlette_admin/i18n.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/views.py` & `starlette_admin-0.9.0.dev0/starlette_admin/views.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/admin.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/converters.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/fields.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/helpers.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/mongoengine/view.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/mongoengine/view.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/odmantic/admin.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/odmantic/converters.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/odmantic/helpers.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/odmantic/middleware.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/odmantic/view.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/odmantic/view.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/admin.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/admin.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/converters.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/converters.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/fields.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/fields.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/helpers.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/helpers.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/middleware.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/middleware.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/view.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/view.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqla/ext/pydantic.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqla/ext/pydantic.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/contrib/sqlmodel/view.py` & `starlette_admin-0.9.0.dev0/starlette_admin/contrib/sqlmodel/view.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/dt.checkboxes.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/dt.checkboxes.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/dt.min.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/dt.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/flatpickr.min.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/flatpickr.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/fontawesome.min.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/jsoneditor.min.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/jsoneditor.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/select2.min.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/tabler.min.css` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/tabler.min.css`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/css/img/jsoneditor-icons.svg` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/css/img/jsoneditor-icons.svg`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/i18n/dt/en.json` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/dt/en.json`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/i18n/dt/fr.json` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/dt/fr.json`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/i18n/flatpickr/fr.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/flatpickr/fr.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/i18n/momentjs/fr.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/i18n/momentjs/fr.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/form.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/form.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/list.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/list.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/render.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/render.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/utils.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/utils.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/dt.checkboxes.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/dt.checkboxes.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/dt.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/dt.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/dt.searchHighlight.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/dt.searchHighlight.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/flatpickr.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/flatpickr.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/jquery.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/jquery.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/js.cookie.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/js.cookie.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/jsoneditor.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/jsoneditor.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/moment.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/moment.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/pdfmake.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/pdfmake.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/select2.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/select2.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/tabler.min.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/tabler.min.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/js/vendor/vfs_fonts.js` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/js/vendor/vfs_fonts.js`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-brands-400.ttf` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-brands-400.woff2` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-regular-400.ttf` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-regular-400.woff2` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-solid-900.ttf` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-solid-900.woff2` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-v4compatibility.ttf` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/statics/webfonts/fa-v4compatibility.woff2` & `starlette_admin-0.9.0.dev0/starlette_admin/statics/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/base.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/base.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/create.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/create.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/detail.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/detail.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/edit.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/edit.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/error.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/error.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/layout.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/layout.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/list.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/list.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/login.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/displays/collection.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/displays/collection.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/_delete.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/_delete.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/collection.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/collection.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/enum.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/enum.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/file.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/file.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/image.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/image.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/list.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/list.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/relation.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/relation.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/forms/tags.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/forms/tags.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/macros/views.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/macros/views.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/modals/actions.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/actions.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/modals/delete.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/delete.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/modals/error.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/error.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/templates/modals/loading.html` & `starlette_admin-0.9.0.dev0/starlette_admin/templates/modals/loading.html`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/translations/en/LC_MESSAGES/admin.mo` & `starlette_admin-0.9.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.mo`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/translations/en/LC_MESSAGES/admin.po` & `starlette_admin-0.9.0.dev0/starlette_admin/translations/en/LC_MESSAGES/admin.po`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo` & `starlette_admin-0.9.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.mo`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/translations/fr/LC_MESSAGES/admin.po` & `starlette_admin-0.9.0.dev0/starlette_admin/translations/fr/LC_MESSAGES/admin.po`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/utils/countries.py` & `starlette_admin-0.9.0.dev0/starlette_admin/utils/countries.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/starlette_admin/utils/timezones.py` & `starlette_admin-0.9.0.dev0/starlette_admin/utils/timezones.py`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/LICENSE` & `starlette_admin-0.9.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/README.md` & `starlette_admin-0.9.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/pyproject.toml` & `starlette_admin-0.9.0.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starlette_admin-0.9.0/PKG-INFO` & `starlette_admin-0.9.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-admin
-Version: 0.9.0
+Version: 0.9.0.dev0
 Summary: Fast, beautiful and extensible administrative interface framework for Starlette/FastApi applications
 Project-URL: Homepage, https://github.com/jowilf/starlette-admin
 Project-URL: Documentation, https://jowilf.github.io/starlette-admin
 Project-URL: Repository, https://github.com/jowilf/starlette-admin
 Project-URL: Changelog, https://jowilf.github.io/starlette-admin/changelog/
 Author-email: Jocelin Hounon <hounonj@gmail.com>
 License-Expression: MIT
```

