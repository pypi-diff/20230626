# Comparing `tmp/nonebot_plugin_htmlrender-0.2.0.3.tar.gz` & `tmp/nonebot_plugin_htmlrender-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_htmlrender-0.2.0.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_htmlrender-0.2.1.tar", last modified: Mon Jun 26 02:58:49 2023, max compression
```

## Comparing `nonebot_plugin_htmlrender-0.2.0.3.tar` & `nonebot_plugin_htmlrender-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1083 2022-04-05 04:23:15.883594 nonebot_plugin_htmlrender-0.2.0.3/LICENSE
--rw-r--r--   0        0        0      874 2023-01-31 11:46:51.239915 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/__init__.py
--rw-r--r--   0        0        0     3268 2023-01-31 11:46:51.241915 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/browser.py
--rw-r--r--   0        0        0      259 2022-10-07 09:07:48.076440 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/config.py
--rw-r--r--   0        0        0     7623 2023-01-31 11:46:51.241915 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/data_source.py
--rw-r--r--   0        0        0    18237 2022-04-05 04:23:15.901586 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/github-markdown-light.css
--rw-r--r--   0        0        0  1458204 2022-04-05 04:23:15.913608 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2022-04-05 04:23:15.916601 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2022-04-05 04:23:15.916601 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0      662 2022-04-05 04:23:15.918226 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/markdown.html
--rw-r--r--   0        0        0     4963 2022-04-05 04:23:15.918226 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2022-04-05 04:23:15.919239 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/text.css
--rw-r--r--   0        0        0      233 2022-04-05 04:23:15.920229 nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/text.html
--rw-r--r--   0        0        0      770 2023-01-31 11:47:51.069226 nonebot_plugin_htmlrender-0.2.0.3/pyproject.toml
--rw-r--r--   0        0        0     3274 2022-10-07 08:58:20.400527 nonebot_plugin_htmlrender-0.2.0.3/README.md
--rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 nonebot_plugin_htmlrender-0.2.0.3/setup.py
--rw-r--r--   0        0        0     4013 1970-01-01 00:00:00.000000 nonebot_plugin_htmlrender-0.2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-26 02:58:37.512265 nonebot_plugin_htmlrender-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3669 2023-06-26 02:58:37.512265 nonebot_plugin_htmlrender-0.2.1/README.md
+-rw-r--r--   0        0        0     1199 2023-06-26 02:58:37.516265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/__init__.py
+-rw-r--r--   0        0        0     3223 2023-06-26 02:58:37.516265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/browser.py
+-rw-r--r--   0        0        0      250 2023-06-26 02:58:37.516265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/config.py
+-rw-r--r--   0        0        0     8203 2023-06-26 02:58:37.516265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/data_source.py
+-rw-r--r--   0        0        0    17297 2023-06-26 02:58:37.516265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/github-markdown-light.css
+-rw-r--r--   0        0        0  1458204 2023-06-26 02:58:37.528265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0      630 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/markdown.html
+-rw-r--r--   0        0        0     4889 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/pygments-default.css
+-rw-r--r--   0        0        0      117 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/text.css
+-rw-r--r--   0        0        0      220 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/text.html
+-rw-r--r--   0        0        0      941 2023-06-26 02:58:49.528328 nonebot_plugin_htmlrender-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/tests/conftest.py
+-rw-r--r--   0        0        0     2281 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/tests/templates/markdown.css
+-rw-r--r--   0        0        0       62 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/tests/templates/mystyle.css
+-rw-r--r--   0        0        0      406 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/tests/templates/text.html
+-rw-r--r--   0        0        0     1462 2023-06-26 02:58:37.532265 nonebot_plugin_htmlrender-0.2.1/tests/test_htmlrender.py
+-rw-r--r--   0        0        0     5556 1970-01-01 00:00:00.000000 nonebot_plugin_htmlrender-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/LICENSE` & `nonebot_plugin_htmlrender-0.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 kexue
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 kexue
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/browser.py` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/browser.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-@Author         : yanyongyu
-@Date           : 2021-03-12 13:42:43
-@LastEditors    : yanyongyu
-@LastEditTime   : 2021-11-01 14:05:41
-@Description    : None
-@GitHub         : https://github.com/yanyongyu
-"""
-__author__ = "yanyongyu"
-
-from typing import Optional, AsyncIterator
-from contextlib import asynccontextmanager
-
-from nonebot import get_driver
-from nonebot.log import logger
-from playwright.async_api import Page, Error, Browser, Playwright, async_playwright
-
-from nonebot_plugin_htmlrender.config import Config
-
-
-class ConfigError(Exception):
-    pass
-
-
-config = Config.parse_obj(get_driver().config.dict())
-
-_browser: Optional[Browser] = None
-_playwright: Optional[Playwright] = None
-
-
-async def init(**kwargs) -> Browser:
-    global _browser
-    global _playwright
-    _playwright = await async_playwright().start()
-    try:
-        _browser = await launch_browser(**kwargs)
-    except Error:
-        await install_browser()
-        _browser = await launch_browser(**kwargs)
-    return _browser
-
-
-async def launch_browser(proxy=config.htmlrender_proxy_host, **kwargs) -> Browser:
-    assert _playwright is not None, "Playwright 没有安装"
-    if proxy:
-        kwargs["proxy"] = proxy
-    if config.htmlrender_browser == "firefox":
-        logger.info("使用 firefox 启动")
-        return await _playwright.firefox.launch(**kwargs)
-
-    else:
-        # 默认使用 chromium
-        logger.info("使用 chromium 启动")
-        return await _playwright.chromium.launch(**kwargs)
-
-
-async def get_browser(**kwargs) -> Browser:
-    return _browser if _browser and _browser.is_connected() else await init(**kwargs)
-
-
-@asynccontextmanager
-async def get_new_page(**kwargs) -> AsyncIterator[Page]:
-    browser = await get_browser()
-    page = await browser.new_page(**kwargs)
-    try:
-        yield page
-    finally:
-        await page.close()
-
-
-async def shutdown_browser():
-    global _browser
-    global _playwright
-    if _browser:
-        await _browser.close()
-        _browser = None
-    if _playwright:
-        await _playwright.stop()  # type: ignore
-        _playwright = None
-
-
-async def install_browser():
-    import os
-    import sys
-
-    from playwright.__main__ import main
-
-    if host := config.htmlrender_download_host:
-        logger.info("使用配置源进行下载")
-        os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = host
-    else:
-        logger.info("使用镜像源进行下载")
-        os.environ[
-            "PLAYWRIGHT_DOWNLOAD_HOST"
-        ] = "https://npmmirror.com/mirrors/playwright/"
-    success = False
-
-    if config.htmlrender_browser == "firefox":
-        logger.info("正在安装 firefox")
-        sys.argv = ["", "install", "firefox"]
-    else:
-        # 默认使用 chromium
-        logger.info("正在安装 chromium")
-        sys.argv = ["", "install", "chromium"]
-    try:
-        logger.info("正在安装依赖")
-        os.system("playwright install-deps")
-        main()
-    except SystemExit as e:
-        if e.code == 0:
-            success = True
-    if not success:
-        logger.error("浏览器更新失败, 请检查网络连通性")
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+@Author         : yanyongyu
+@Date           : 2021-03-12 13:42:43
+@LastEditors    : yanyongyu
+@LastEditTime   : 2021-11-01 14:05:41
+@Description    : None
+@GitHub         : https://github.com/yanyongyu
+"""
+__author__ = "yanyongyu"
+
+from typing import Optional, AsyncIterator
+from contextlib import asynccontextmanager
+
+from nonebot import get_driver
+from nonebot.log import logger
+from playwright.async_api import Page, Error, Browser, Playwright, async_playwright
+
+from nonebot_plugin_htmlrender.config import Config
+
+
+class ConfigError(Exception):
+    pass
+
+
+config = Config.parse_obj(get_driver().config.dict())
+
+_browser: Optional[Browser] = None
+_playwright: Optional[Playwright] = None
+
+
+async def init(**kwargs) -> Browser:
+    global _browser
+    global _playwright
+    _playwright = await async_playwright().start()
+    try:
+        _browser = await launch_browser(**kwargs)
+    except Error:
+        await install_browser()
+        _browser = await launch_browser(**kwargs)
+    return _browser
+
+
+async def launch_browser(proxy=config.htmlrender_proxy_host, **kwargs) -> Browser:
+    assert _playwright is not None, "Playwright 没有安装"
+    if proxy:
+        kwargs["proxy"] = proxy
+    if config.htmlrender_browser == "firefox":
+        logger.info("使用 firefox 启动")
+        return await _playwright.firefox.launch(**kwargs)
+
+    else:
+        # 默认使用 chromium
+        logger.info("使用 chromium 启动")
+        return await _playwright.chromium.launch(**kwargs)
+
+
+async def get_browser(**kwargs) -> Browser:
+    return _browser if _browser and _browser.is_connected() else await init(**kwargs)
+
+
+@asynccontextmanager
+async def get_new_page(device_scale_factor:float = 2,**kwargs) -> AsyncIterator[Page]:
+    browser = await get_browser()
+    page = await browser.new_page(device_scale_factor=device_scale_factor,**kwargs)
+    try:
+        yield page
+    finally:
+        await page.close()
+
+
+async def shutdown_browser():
+    global _browser
+    global _playwright
+    if _browser:
+        await _browser.close()
+        _browser = None
+    if _playwright:
+        await _playwright.stop()  # type: ignore
+        _playwright = None
+
+
+async def install_browser():
+    import os
+    import sys
+
+    from playwright.__main__ import main
+
+    if host := config.htmlrender_download_host:
+        logger.info("使用配置源进行下载")
+        os.environ["PLAYWRIGHT_DOWNLOAD_HOST"] = host
+    else:
+        logger.info("使用镜像源进行下载")
+        os.environ[
+            "PLAYWRIGHT_DOWNLOAD_HOST"
+        ] = "https://npmmirror.com/mirrors/playwright/"
+    success = False
+
+    if config.htmlrender_browser == "firefox":
+        logger.info("正在安装 firefox")
+        sys.argv = ["", "install", "firefox"]
+    else:
+        # 默认使用 chromium
+        logger.info("正在安装 chromium")
+        sys.argv = ["", "install", "chromium"]
+    try:
+        logger.info("正在安装依赖")
+        os.system("playwright install-deps")
+        main()
+    except SystemExit as e:
+        if e.code == 0:
+            success = True
+    if not success:
+        logger.error("浏览器更新失败, 请检查网络连通性")
```

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/data_source.py` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/data_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,257 +1,266 @@
-from os import getcwd
-from typing import Union, Literal
-from pathlib import Path
-
-import jinja2
-import aiofiles
-import markdown
-from nonebot.log import logger
-
-from .browser import get_new_page
-
-TEMPLATES_PATH = str(Path(__file__).parent / "templates")
-
-env = jinja2.Environment(
-    extensions=["jinja2.ext.loopcontrols"],
-    loader=jinja2.FileSystemLoader(TEMPLATES_PATH),
-    enable_async=True,
-)
-
-
-async def text_to_pic(
-    text: str,
-    css_path: str = "",
-    width: int = 500,
-    type: Literal["jpeg", "png"] = "png",
-    quality: Union[int, None] = None,
-) -> bytes:
-    """多行文本转图片
-
-    Args:
-        text (str): 纯文本, 可多行
-        css_path (str, optional): css文件
-        width (int, optional): 图片宽度，默认为 500
-        type (Literal["jpeg", "png"]): 图片类型, 默认 png
-        quality (int, optional): 图片质量 0-100 当为`png`时无效
-
-    Returns:
-        bytes: 图片, 可直接发送
-    """
-    template = env.get_template("text.html")
-
-    return await html_to_pic(
-        template_path=f"file://{css_path if css_path else TEMPLATES_PATH}",
-        html=await template.render_async(
-            text=text,
-            css=await read_file(css_path) if css_path else await read_tpl("text.css"),
-        ),
-        viewport={"width": width, "height": 10},
-        type=type,
-        quality=quality,
-    )
-
-
-async def md_to_pic(
-    md: str = "",
-    md_path: str = "",
-    css_path: str = "",
-    width: int = 500,
-    type: Literal["jpeg", "png"] = "png",
-    quality: Union[int, None] = None,
-) -> bytes:
-    """markdown 转 图片
-
-    Args:
-        md (str, optional): markdown 格式文本
-        md_path (str, optional): markdown 文件路径
-        css_path (str,  optional): css文件路径. Defaults to None.
-        width (int, optional): 图片宽度，默认为 500
-        type (Literal["jpeg", "png"]): 图片类型, 默认 png
-        quality (int, optional): 图片质量 0-100 当为`png`时无效
-
-    Returns:
-        bytes: 图片, 可直接发送
-    """
-    template = env.get_template("markdown.html")
-    if not md:
-        if md_path:
-            md = await read_file(md_path)
-        else:
-            raise Exception("必须输入 md 或 md_path")
-    logger.debug(md)
-    md = markdown.markdown(
-        md,
-        extensions=[
-            "pymdownx.tasklist",
-            "tables",
-            "fenced_code",
-            "codehilite",
-            "mdx_math",
-            "pymdownx.tilde",
-        ],
-        extension_configs={"mdx_math": {"enable_dollar_delimiter": True}},
-    )
-
-    logger.debug(md)
-    extra = ""
-    if "math/tex" in md:
-        katex_css = await read_tpl("katex/katex.min.b64_fonts.css")
-        katex_js = await read_tpl("katex/katex.min.js")
-        mathtex_js = await read_tpl("katex/mathtex-script-type.min.js")
-        extra = (
-            f'<style type="text/css">{katex_css}</style>'
-            f"<script defer>{katex_js}</script>"
-            f"<script defer>{mathtex_js}</script>"
-        )
-
-    if css_path:
-        css = await read_file(css_path)
-    else:
-        css = await read_tpl("github-markdown-light.css") + await read_tpl(
-            "pygments-default.css"
-        )
-
-    return await html_to_pic(
-        template_path=f"file://{css_path if css_path else TEMPLATES_PATH}",
-        html=await template.render_async(md=md, css=css, extra=extra),
-        viewport={"width": width, "height": 10},
-        type=type,
-        quality=quality,
-    )
-
-
-# async def read_md(md_path: str) -> str:
-#     async with aiofiles.open(str(Path(md_path).resolve()), mode="r") as f:
-#         md = await f.read()
-#     return markdown.markdown(md)
-
-
-async def read_file(path: str) -> str:
-    async with aiofiles.open(path, mode="r") as f:
-        return await f.read()
-
-
-async def read_tpl(path: str) -> str:
-    return await read_file(f"{TEMPLATES_PATH}/{path}")
-
-
-async def template_to_html(
-    template_path: str,
-    template_name: str,
-    **kwargs,
-) -> str:
-    """使用jinja2模板引擎通过html生成图片
-
-    Args:
-        template_path (str): 模板路径
-        template_name (str): 模板名
-        **kwargs: 模板内容
-
-    Returns:
-        str: html
-    """
-
-    template_env = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(template_path),
-        enable_async=True,
-    )
-    template = template_env.get_template(template_name)
-
-    return await template.render_async(**kwargs)
-
-
-async def html_to_pic(
-    html: str,
-    wait: int = 0,
-    template_path: str = f"file://{getcwd()}",
-    type: Literal["jpeg", "png"] = "png",
-    quality: Union[int, None] = None,
-    **kwargs,
-) -> bytes:
-    """html转图片
-
-    Args:
-        html (str): html文本
-        wait (int, optional): 等待时间. Defaults to 0.
-        template_path (str, optional): 模板路径 如 "file:///path/to/template/"
-        type (Literal["jpeg", "png"]): 图片类型, 默认 png
-        quality (int, optional): 图片质量 0-100 当为`png`时无效
-        **kwargs: 传入 page 的参数
-
-    Returns:
-        bytes: 图片, 可直接发送
-    """
-    # logger.debug(f"html:\n{html}")
-    if "file:" not in template_path:
-        raise Exception("template_path 应该为 file:///path/to/template")
-    async with get_new_page(**kwargs) as page:
-        await page.goto(template_path)
-        await page.set_content(html, wait_until="networkidle")
-        await page.wait_for_timeout(wait)
-        img_raw = await page.screenshot(
-            full_page=True,
-            type=type,
-            quality=quality,
-        )
-    return img_raw
-
-
-async def template_to_pic(
-    template_path: str,
-    template_name: str,
-    templates: dict,
-    pages: dict = {
-        "viewport": {"width": 500, "height": 10},
-        "base_url": f"file://{getcwd()}",
-    },
-    wait: int = 0,
-    type: Literal["jpeg", "png"] = "png",
-    quality: Union[int, None] = None,
-) -> bytes:
-    """使用jinja2模板引擎通过html生成图片
-
-    Args:
-        template_path (str): 模板路径
-        template_name (str): 模板名
-        templates (dict): 模板内参数 如: {"name": "abc"}
-        pages (dict): 网页参数 Defaults to
-            {"base_url": f"file://{getcwd()}", "viewport": {"width": 500, "height": 10}}
-        wait (int, optional): 网页载入等待时间. Defaults to 0.
-        type (Literal["jpeg", "png"]): 图片类型, 默认 png
-        quality (int, optional): 图片质量 0-100 当为`png`时无效
-
-    Returns:
-        bytes: 图片 可直接发送
-    """
-
-    template_env = jinja2.Environment(
-        loader=jinja2.FileSystemLoader(template_path),
-        enable_async=True,
-    )
-    template = template_env.get_template(template_name)
-
-    return await html_to_pic(
-        template_path=f"file://{template_path}",
-        html=await template.render_async(**templates),
-        wait=wait,
-        type=type,
-        quality=quality,
-        **pages,
-    )
-
-
-async def capture_element(
-    url: str,
-    element: str,
-    timeout: float = 0,
-    type: Literal["jpeg", "png"] = "png",
-    quality: Union[int, None] = None,
-    **kwargs,
-) -> bytes:
-    async with get_new_page(**kwargs) as page:
-        await page.goto(url, timeout=timeout)
-        img_raw = await page.locator(element).screenshot(
-            type=type,
-            quality=quality,
-        )
-    return img_raw
+from os import getcwd
+from typing import Union, Literal
+from pathlib import Path
+
+import jinja2
+import aiofiles
+import markdown
+from nonebot.log import logger
+
+from .browser import get_new_page
+
+TEMPLATES_PATH = str(Path(__file__).parent / "templates")
+
+env = jinja2.Environment(
+    extensions=["jinja2.ext.loopcontrols"],
+    loader=jinja2.FileSystemLoader(TEMPLATES_PATH),
+    enable_async=True,
+)
+
+
+async def text_to_pic(
+    text: str,
+    css_path: str = "",
+    width: int = 500,
+    type: Literal["jpeg", "png"] = "png",
+    quality: Union[int, None] = None,
+    device_scale_factor: float=2
+) -> bytes:
+    """多行文本转图片
+
+    Args:
+        text (str): 纯文本, 可多行
+        css_path (str, optional): css文件
+        width (int, optional): 图片宽度，默认为 500
+        type (Literal["jpeg", "png"]): 图片类型, 默认 png
+        quality (int, optional): 图片质量 0-100 当为`png`时无效
+        device_scale_factor: 缩放比例,类型为float,值越大越清晰(真正想让图片清晰更优先请调整此选项)
+        
+    Returns:
+        bytes: 图片, 可直接发送
+    """
+    template = env.get_template("text.html")
+
+    return await html_to_pic(
+        template_path=f"file://{css_path if css_path else TEMPLATES_PATH}",
+        html=await template.render_async(
+            text=text,
+            css=await read_file(css_path) if css_path else await read_tpl("text.css"),
+        ),
+        viewport={"width": width, "height": 10},
+        type=type,
+        quality=quality,
+        device_scale_factor=device_scale_factor
+    )
+
+
+async def md_to_pic(
+    md: str = "",
+    md_path: str = "",
+    css_path: str = "",
+    width: int = 500,
+    type: Literal["jpeg", "png"] = "png",
+    quality: Union[int, None] = None,
+    device_scale_factor:float = 2
+) -> bytes:
+    """markdown 转 图片
+    
+    Args:
+        md (str, optional): markdown 格式文本
+        md_path (str, optional): markdown 文件路径
+        css_path (str,  optional): css文件路径. Defaults to None.
+        width (int, optional): 图片宽度，默认为 500
+        type (Literal["jpeg", "png"]): 图片类型, 默认 png
+        quality (int, optional): 图片质量 0-100 当为`png`时无效
+        device_scale_factor: 缩放比例,类型为float,值越大越清晰(真正想让图片清晰更优先请调整此选项)
+        
+    Returns:
+        bytes: 图片, 可直接发送
+    """
+    template = env.get_template("markdown.html")
+    if not md:
+        if md_path:
+            md = await read_file(md_path)
+        else:
+            raise Exception("必须输入 md 或 md_path")
+    logger.debug(md)
+    md = markdown.markdown(
+        md,
+        extensions=[
+            "pymdownx.tasklist",
+            "tables",
+            "fenced_code",
+            "codehilite",
+            "mdx_math",
+            "pymdownx.tilde",
+        ],
+        extension_configs={"mdx_math": {"enable_dollar_delimiter": True}},
+    )
+
+    logger.debug(md)
+    extra = ""
+    if "math/tex" in md:
+        katex_css = await read_tpl("katex/katex.min.b64_fonts.css")
+        katex_js = await read_tpl("katex/katex.min.js")
+        mathtex_js = await read_tpl("katex/mathtex-script-type.min.js")
+        extra = (
+            f'<style type="text/css">{katex_css}</style>'
+            f"<script defer>{katex_js}</script>"
+            f"<script defer>{mathtex_js}</script>"
+        )
+
+    if css_path:
+        css = await read_file(css_path)
+    else:
+        css = await read_tpl("github-markdown-light.css") + await read_tpl(
+            "pygments-default.css"
+        )
+
+    return await html_to_pic(
+        template_path=f"file://{css_path if css_path else TEMPLATES_PATH}",
+        html=await template.render_async(md=md, css=css, extra=extra),
+        viewport={"width": width, "height": 10},
+        type=type,
+        quality=quality,
+        device_scale_factor = device_scale_factor
+    )
+
+
+# async def read_md(md_path: str) -> str:
+#     async with aiofiles.open(str(Path(md_path).resolve()), mode="r") as f:
+#         md = await f.read()
+#     return markdown.markdown(md)
+
+
+async def read_file(path: str) -> str:
+    async with aiofiles.open(path, mode="r") as f:
+        return await f.read()
+
+
+async def read_tpl(path: str) -> str:
+    return await read_file(f"{TEMPLATES_PATH}/{path}")
+
+
+async def template_to_html(
+    template_path: str,
+    template_name: str,
+    **kwargs,
+) -> str:
+    """使用jinja2模板引擎通过html生成图片
+
+    Args:
+        template_path (str): 模板路径
+        template_name (str): 模板名
+        **kwargs: 模板内容
+    Returns:
+        str: html
+    """
+
+    template_env = jinja2.Environment(
+        loader=jinja2.FileSystemLoader(template_path),
+        enable_async=True,
+    )
+    template = template_env.get_template(template_name)
+
+    return await template.render_async(**kwargs)
+
+
+async def html_to_pic(
+    html: str,
+    wait: int = 0,
+    template_path: str = f"file://{getcwd()}",
+    type: Literal["jpeg", "png"] = "png",
+    quality: Union[int, None] = None,
+    device_scale_factor:float = 2,
+    **kwargs,
+) -> bytes:
+    """html转图片
+
+    Args:
+        html (str): html文本
+        wait (int, optional): 等待时间. Defaults to 0.
+        template_path (str, optional): 模板路径 如 "file:///path/to/template/"
+        type (Literal["jpeg", "png"]): 图片类型, 默认 png
+        quality (int, optional): 图片质量 0-100 当为`png`时无效
+        device_scale_factor: 缩放比例,类型为float,值越大越清晰(真正想让图片清晰更优先请调整此选项)
+        **kwargs: 传入 page 的参数
+
+    Returns:
+        bytes: 图片, 可直接发送
+    """
+    # logger.debug(f"html:\n{html}")
+    if "file:" not in template_path:
+        raise Exception("template_path 应该为 file:///path/to/template")
+    async with get_new_page(device_scale_factor,**kwargs) as page:
+        await page.goto(template_path)
+        await page.set_content(html, wait_until="networkidle")
+        await page.wait_for_timeout(wait)
+        img_raw = await page.screenshot(
+            full_page=True,
+            type=type,
+            quality=quality,
+        )
+    return img_raw
+
+
+async def template_to_pic(
+    template_path: str,
+    template_name: str,
+    templates: dict,
+    pages: dict = {
+        "viewport": {"width": 500, "height": 10},
+        "base_url": f"file://{getcwd()}",
+    },
+    wait: int = 0,
+    type: Literal["jpeg", "png"] = "png",
+    quality: Union[int, None] = None,
+    device_scale_factor:float = 2
+) -> bytes:
+    """使用jinja2模板引擎通过html生成图片
+
+    Args:
+        template_path (str): 模板路径
+        template_name (str): 模板名
+        templates (dict): 模板内参数 如: {"name": "abc"}
+        pages (dict): 网页参数 Defaults to
+            {"base_url": f"file://{getcwd()}", "viewport": {"width": 500, "height": 10}}
+        wait (int, optional): 网页载入等待时间. Defaults to 0.
+        type (Literal["jpeg", "png"]): 图片类型, 默认 png
+        quality (int, optional): 图片质量 0-100 当为`png`时无效
+        device_scale_factor: 缩放比例,类型为float,值越大越清晰(真正想让图片清晰更优先请调整此选项)
+    Returns:
+        bytes: 图片 可直接发送
+    """
+
+    template_env = jinja2.Environment(
+        loader=jinja2.FileSystemLoader(template_path),
+        enable_async=True,
+    )
+    template = template_env.get_template(template_name)
+
+    return await html_to_pic(
+        template_path=f"file://{template_path}",
+        html=await template.render_async(**templates),
+        wait=wait,
+        type=type,
+        quality=quality,
+        device_scale_factor=device_scale_factor,
+        **pages,
+    )
+
+
+async def capture_element(
+    url: str,
+    element: str,
+    timeout: float = 0,
+    type: Literal["jpeg", "png"] = "png",
+    quality: Union[int, None] = None,
+    **kwargs,
+) -> bytes:
+    async with get_new_page(**kwargs) as page:
+        await page.goto(url, timeout=timeout)
+        img_raw = await page.locator(element).screenshot(
+            type=type,
+            quality=quality,
+        )
+    return img_raw
```

#### html2text {}

```diff
@@ -1,84 +1,97 @@
 from os import getcwd from typing import Union, Literal from pathlib import
 Path import jinja2 import aiofiles import markdown from nonebot.log import
 logger from .browser import get_new_page TEMPLATES_PATH = str(Path
 (__file__).parent / "templates") env = jinja2.Environment( extensions=
 ["jinja2.ext.loopcontrols"], loader=jinja2.FileSystemLoader(TEMPLATES_PATH),
 enable_async=True, ) async def text_to_pic( text: str, css_path: str = "",
 width: int = 500, type: Literal["jpeg", "png"] = "png", quality: Union[int,
-None] = None, ) -> bytes: """å¤è¡ææ¬è½¬å¾ç Args: text (str): çº¯ææ¬,
-å¯å¤è¡ css_path (str, optional): cssæä»¶ width (int, optional):
-å¾çå®½åº¦ï¼é»è®¤ä¸º 500 type (Literal["jpeg", "png"]): å¾çç±»å,
-é»è®¤ png quality (int, optional): å¾çè´¨é 0-100 å½ä¸º`png`æ¶æ æ
-Returns: bytes: å¾ç, å¯ç´æ¥åé """ template = env.get_template
-("text.html") return await html_to_pic( template_path=f"file://{css_path if
-css_path else TEMPLATES_PATH}", html=await template.render_async( text=text,
-css=await read_file(css_path) if css_path else await read_tpl("text.css"), ),
-viewport={"width": width, "height": 10}, type=type, quality=quality, ) async
-def md_to_pic( md: str = "", md_path: str = "", css_path: str = "", width: int
-= 500, type: Literal["jpeg", "png"] = "png", quality: Union[int, None] = None,
+None] = None, device_scale_factor: float=2 ) -> bytes: """å¤è¡ææ¬è½¬å¾ç
+Args: text (str): çº¯ææ¬, å¯å¤è¡ css_path (str, optional): cssæä»¶
+width (int, optional): å¾çå®½åº¦ï¼é»è®¤ä¸º 500 type (Literal["jpeg",
+"png"]): å¾çç±»å, é»è®¤ png quality (int, optional): å¾çè´¨é 0-100
+å½ä¸º`png`æ¶æ æ device_scale_factor:
+ç¼©æ¾æ¯ä¾,ç±»åä¸ºfloat,å¼è¶å¤§è¶æ¸æ°
+(çæ­£æ³è®©å¾çæ¸æ°æ´ä¼åè¯·è°æ´æ­¤éé¡¹) Returns: bytes: å¾ç,
+å¯ç´æ¥åé """ template = env.get_template("text.html") return await
+html_to_pic( template_path=f"file://{css_path if css_path else
+TEMPLATES_PATH}", html=await template.render_async( text=text, css=await
+read_file(css_path) if css_path else await read_tpl("text.css"), ), viewport=
+{"width": width, "height": 10}, type=type, quality=quality,
+device_scale_factor=device_scale_factor ) async def md_to_pic( md: str = "",
+md_path: str = "", css_path: str = "", width: int = 500, type: Literal["jpeg",
+"png"] = "png", quality: Union[int, None] = None, device_scale_factor:float = 2
 ) -> bytes: """markdown è½¬ å¾ç Args: md (str, optional): markdown
 æ ¼å¼ææ¬ md_path (str, optional): markdown æä»¶è·¯å¾ css_path (str,
 optional): cssæä»¶è·¯å¾. Defaults to None. width (int, optional):
 å¾çå®½åº¦ï¼é»è®¤ä¸º 500 type (Literal["jpeg", "png"]): å¾çç±»å,
 é»è®¤ png quality (int, optional): å¾çè´¨é 0-100 å½ä¸º`png`æ¶æ æ
-Returns: bytes: å¾ç, å¯ç´æ¥åé """ template = env.get_template
-("markdown.html") if not md: if md_path: md = await read_file(md_path) else:
-raise Exception("å¿é¡»è¾å¥ md æ md_path") logger.debug(md) md =
-markdown.markdown( md, extensions=[ "pymdownx.tasklist", "tables",
-"fenced_code", "codehilite", "mdx_math", "pymdownx.tilde", ],
-extension_configs={"mdx_math": {"enable_dollar_delimiter": True}}, )
-logger.debug(md) extra = "" if "math/tex" in md: katex_css = await read_tpl
-("katex/katex.min.b64_fonts.css") katex_js = await read_tpl("katex/
+device_scale_factor: ç¼©æ¾æ¯ä¾,ç±»åä¸ºfloat,å¼è¶å¤§è¶æ¸æ°
+(çæ­£æ³è®©å¾çæ¸æ°æ´ä¼åè¯·è°æ´æ­¤éé¡¹) Returns: bytes: å¾ç,
+å¯ç´æ¥åé """ template = env.get_template("markdown.html") if not md: if
+md_path: md = await read_file(md_path) else: raise Exception("å¿é¡»è¾å¥ md
+æ md_path") logger.debug(md) md = markdown.markdown( md, extensions=
+[ "pymdownx.tasklist", "tables", "fenced_code", "codehilite", "mdx_math",
+"pymdownx.tilde", ], extension_configs={"mdx_math": {"enable_dollar_delimiter":
+True}}, ) logger.debug(md) extra = "" if "math/tex" in md: katex_css = await
+read_tpl("katex/katex.min.b64_fonts.css") katex_js = await read_tpl("katex/
 katex.min.js") mathtex_js = await read_tpl("katex/mathtex-script-type.min.js")
 extra = ( f'
 ' f"
 " f"
 " ) if css_path: css = await read_file(css_path) else: css = await read_tpl
 ("github-markdown-light.css") + await read_tpl( "pygments-default.css" ) return
 await html_to_pic( template_path=f"file://{css_path if css_path else
 TEMPLATES_PATH}", html=await template.render_async(md=md, css=css,
 extra=extra), viewport={"width": width, "height": 10}, type=type,
-quality=quality, ) # async def read_md(md_path: str) -> str: # async with
-aiofiles.open(str(Path(md_path).resolve()), mode="r") as f: # md = await f.read
-() # return markdown.markdown(md) async def read_file(path: str) -> str: async
-with aiofiles.open(path, mode="r") as f: return await f.read() async def
-read_tpl(path: str) -> str: return await read_file(f"{TEMPLATES_PATH}/{path}")
-async def template_to_html( template_path: str, template_name: str, **kwargs, )
--> str: """ä½¿ç¨jinja2æ¨¡æ¿å¼æéè¿htmlçæå¾ç Args: template_path
+quality=quality, device_scale_factor = device_scale_factor ) # async def
+read_md(md_path: str) -> str: # async with aiofiles.open(str(Path
+(md_path).resolve()), mode="r") as f: # md = await f.read() # return
+markdown.markdown(md) async def read_file(path: str) -> str: async with
+aiofiles.open(path, mode="r") as f: return await f.read() async def read_tpl
+(path: str) -> str: return await read_file(f"{TEMPLATES_PATH}/{path}") async
+def template_to_html( template_path: str, template_name: str, **kwargs, ) -
+> str: """ä½¿ç¨jinja2æ¨¡æ¿å¼æéè¿htmlçæå¾ç Args: template_path
 (str): æ¨¡æ¿è·¯å¾ template_name (str): æ¨¡æ¿å **kwargs: æ¨¡æ¿åå®¹
 Returns: str: html """ template_env = jinja2.Environment
 ( loader=jinja2.FileSystemLoader(template_path), enable_async=True, ) template
 = template_env.get_template(template_name) return await template.render_async
 (**kwargs) async def html_to_pic( html: str, wait: int = 0, template_path: str
 = f"file://{getcwd()}", type: Literal["jpeg", "png"] = "png", quality: Union
-[int, None] = None, **kwargs, ) -> bytes: """htmlè½¬å¾ç Args: html (str):
-htmlææ¬ wait (int, optional): ç­å¾æ¶é´. Defaults to 0. template_path
-(str, optional): æ¨¡æ¿è·¯å¾ å¦ "file:///path/to/template/" type (Literal
-["jpeg", "png"]): å¾çç±»å, é»è®¤ png quality (int, optional):
-å¾çè´¨é 0-100 å½ä¸º`png`æ¶æ æ **kwargs: ä¼ å¥ page çåæ°
-Returns: bytes: å¾ç, å¯ç´æ¥åé """ # logger.debug(f"html:\n{html}") if
-"file:" not in template_path: raise Exception("template_path åºè¯¥ä¸º file:///
-path/to/template") async with get_new_page(**kwargs) as page: await page.goto
-(template_path) await page.set_content(html, wait_until="networkidle") await
-page.wait_for_timeout(wait) img_raw = await page.screenshot( full_page=True,
-type=type, quality=quality, ) return img_raw async def template_to_pic
-( template_path: str, template_name: str, templates: dict, pages: dict =
-{ "viewport": {"width": 500, "height": 10}, "base_url": f"file://{getcwd()}",
-}, wait: int = 0, type: Literal["jpeg", "png"] = "png", quality: Union[int,
-None] = None, ) -> bytes: """ä½¿ç¨jinja2æ¨¡æ¿å¼æéè¿htmlçæå¾ç
-Args: template_path (str): æ¨¡æ¿è·¯å¾ template_name (str): æ¨¡æ¿å
-templates (dict): æ¨¡æ¿ååæ° å¦: {"name": "abc"} pages (dict):
-ç½é¡µåæ° Defaults to {"base_url": f"file://{getcwd()}", "viewport":
-{"width": 500, "height": 10}} wait (int, optional): ç½é¡µè½½å¥ç­å¾æ¶é´.
-Defaults to 0. type (Literal["jpeg", "png"]): å¾çç±»å, é»è®¤ png quality
-(int, optional): å¾çè´¨é 0-100 å½ä¸º`png`æ¶æ æ Returns: bytes: å¾ç
+[int, None] = None, device_scale_factor:float = 2, **kwargs, ) -> bytes:
+"""htmlè½¬å¾ç Args: html (str): htmlææ¬ wait (int, optional):
+ç­å¾æ¶é´. Defaults to 0. template_path (str, optional): æ¨¡æ¿è·¯å¾ å¦
+"file:///path/to/template/" type (Literal["jpeg", "png"]): å¾çç±»å, é»è®¤
+png quality (int, optional): å¾çè´¨é 0-100 å½ä¸º`png`æ¶æ æ
+device_scale_factor: ç¼©æ¾æ¯ä¾,ç±»åä¸ºfloat,å¼è¶å¤§è¶æ¸æ°
+(çæ­£æ³è®©å¾çæ¸æ°æ´ä¼åè¯·è°æ´æ­¤éé¡¹) **kwargs: ä¼ å¥ page
+çåæ° Returns: bytes: å¾ç, å¯ç´æ¥åé """ # logger.debug(f"html:\n
+{html}") if "file:" not in template_path: raise Exception("template_path
+åºè¯¥ä¸º file:///path/to/template") async with get_new_page
+(device_scale_factor,**kwargs) as page: await page.goto(template_path) await
+page.set_content(html, wait_until="networkidle") await page.wait_for_timeout
+(wait) img_raw = await page.screenshot( full_page=True, type=type,
+quality=quality, ) return img_raw async def template_to_pic( template_path:
+str, template_name: str, templates: dict, pages: dict = { "viewport": {"width":
+500, "height": 10}, "base_url": f"file://{getcwd()}", }, wait: int = 0, type:
+Literal["jpeg", "png"] = "png", quality: Union[int, None] = None,
+device_scale_factor:float = 2 ) -> bytes:
+"""ä½¿ç¨jinja2æ¨¡æ¿å¼æéè¿htmlçæå¾ç Args: template_path (str):
+æ¨¡æ¿è·¯å¾ template_name (str): æ¨¡æ¿å templates (dict): æ¨¡æ¿ååæ°
+å¦: {"name": "abc"} pages (dict): ç½é¡µåæ° Defaults to {"base_url":
+f"file://{getcwd()}", "viewport": {"width": 500, "height": 10}} wait (int,
+optional): ç½é¡µè½½å¥ç­å¾æ¶é´. Defaults to 0. type (Literal["jpeg",
+"png"]): å¾çç±»å, é»è®¤ png quality (int, optional): å¾çè´¨é 0-100
+å½ä¸º`png`æ¶æ æ device_scale_factor:
+ç¼©æ¾æ¯ä¾,ç±»åä¸ºfloat,å¼è¶å¤§è¶æ¸æ°
+(çæ­£æ³è®©å¾çæ¸æ°æ´ä¼åè¯·è°æ´æ­¤éé¡¹) Returns: bytes: å¾ç
 å¯ç´æ¥åé """ template_env = jinja2.Environment
 ( loader=jinja2.FileSystemLoader(template_path), enable_async=True, ) template
 = template_env.get_template(template_name) return await html_to_pic
 ( template_path=f"file://{template_path}", html=await template.render_async
-(**templates), wait=wait, type=type, quality=quality, **pages, ) async def
-capture_element( url: str, element: str, timeout: float = 0, type: Literal
-["jpeg", "png"] = "png", quality: Union[int, None] = None, **kwargs, ) -
-> bytes: async with get_new_page(**kwargs) as page: await page.goto(url,
-timeout=timeout) img_raw = await page.locator(element).screenshot( type=type,
-quality=quality, ) return img_raw
+(**templates), wait=wait, type=type, quality=quality,
+device_scale_factor=device_scale_factor, **pages, ) async def capture_element
+( url: str, element: str, timeout: float = 0, type: Literal["jpeg", "png"] =
+"png", quality: Union[int, None] = None, **kwargs, ) -> bytes: async with
+get_new_page(**kwargs) as page: await page.goto(url, timeout=timeout) img_raw =
+await page.locator(element).screenshot( type=type, quality=quality, ) return
+img_raw
```

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/github-markdown-light.css` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/github-markdown-light.css`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,940 +1,940 @@
-.markdown-body {
-  -ms-text-size-adjust: 100%;
-  -webkit-text-size-adjust: 100%;
-  margin: 0;
-  color: #24292f;
-  background-color: #ffffff;
-  font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji";
-  font-size: 16px;
-  line-height: 1.5;
-  word-wrap: break-word;
-}
-
-.markdown-body .octicon {
-  display: inline-block;
-  fill: currentColor;
-  vertical-align: text-bottom;
-}
-
-.markdown-body h1:hover .anchor .octicon-link:before,
-.markdown-body h2:hover .anchor .octicon-link:before,
-.markdown-body h3:hover .anchor .octicon-link:before,
-.markdown-body h4:hover .anchor .octicon-link:before,
-.markdown-body h5:hover .anchor .octicon-link:before,
-.markdown-body h6:hover .anchor .octicon-link:before {
-  width: 16px;
-  height: 16px;
-  content: ' ';
-  display: inline-block;
-  background-color: currentColor;
-  -webkit-mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
-  mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
-}
-
-.markdown-body details,
-.markdown-body figcaption,
-.markdown-body figure {
-  display: block;
-}
-
-.markdown-body summary {
-  display: list-item;
-}
-
-.markdown-body [hidden] {
-  display: none !important;
-}
-
-.markdown-body a {
-  background-color: transparent;
-  color: #0969da;
-  text-decoration: none;
-}
-
-.markdown-body a:active,
-.markdown-body a:hover {
-  outline-width: 0;
-}
-
-.markdown-body abbr[title] {
-  border-bottom: none;
-  text-decoration: underline dotted;
-}
-
-.markdown-body b,
-.markdown-body strong {
-  font-weight: 600;
-}
-
-.markdown-body dfn {
-  font-style: italic;
-}
-
-.markdown-body h1 {
-  margin: .67em 0;
-  font-weight: 600;
-  padding-bottom: .3em;
-  font-size: 2em;
-  border-bottom: 1px solid hsla(210,18%,87%,1);
-}
-
-.markdown-body mark {
-  background-color: #fff8c5;
-  color: #24292f;
-}
-
-.markdown-body small {
-  font-size: 90%;
-}
-
-.markdown-body sub,
-.markdown-body sup {
-  font-size: 75%;
-  line-height: 0;
-  position: relative;
-  vertical-align: baseline;
-}
-
-.markdown-body sub {
-  bottom: -0.25em;
-}
-
-.markdown-body sup {
-  top: -0.5em;
-}
-
-.markdown-body img {
-  border-style: none;
-  max-width: 100%;
-  box-sizing: content-box;
-  background-color: #ffffff;
-}
-
-.markdown-body code,
-.markdown-body kbd,
-.markdown-body pre,
-.markdown-body samp {
-  font-family: monospace,monospace;
-  font-size: 1em;
-}
-
-.markdown-body figure {
-  margin: 1em 40px;
-}
-
-.markdown-body hr {
-  box-sizing: content-box;
-  overflow: hidden;
-  background: transparent;
-  border-bottom: 1px solid hsla(210,18%,87%,1);
-  height: .25em;
-  padding: 0;
-  margin: 24px 0;
-  background-color: #d0d7de;
-  border: 0;
-}
-
-.markdown-body input {
-  font: inherit;
-  margin: 0;
-  overflow: visible;
-  font-family: inherit;
-  font-size: inherit;
-  line-height: inherit;
-}
-
-.markdown-body [type=button],
-.markdown-body [type=reset],
-.markdown-body [type=submit] {
-  -webkit-appearance: button;
-}
-
-.markdown-body [type=button]::-moz-focus-inner,
-.markdown-body [type=reset]::-moz-focus-inner,
-.markdown-body [type=submit]::-moz-focus-inner {
-  border-style: none;
-  padding: 0;
-}
-
-.markdown-body [type=button]:-moz-focusring,
-.markdown-body [type=reset]:-moz-focusring,
-.markdown-body [type=submit]:-moz-focusring {
-  outline: 1px dotted ButtonText;
-}
-
-.markdown-body [type=checkbox],
-.markdown-body [type=radio] {
-  box-sizing: border-box;
-  padding: 0;
-}
-
-.markdown-body [type=number]::-webkit-inner-spin-button,
-.markdown-body [type=number]::-webkit-outer-spin-button {
-  height: auto;
-}
-
-.markdown-body [type=search] {
-  -webkit-appearance: textfield;
-  outline-offset: -2px;
-}
-
-.markdown-body [type=search]::-webkit-search-cancel-button,
-.markdown-body [type=search]::-webkit-search-decoration {
-  -webkit-appearance: none;
-}
-
-.markdown-body ::-webkit-input-placeholder {
-  color: inherit;
-  opacity: .54;
-}
-
-.markdown-body ::-webkit-file-upload-button {
-  -webkit-appearance: button;
-  font: inherit;
-}
-
-.markdown-body a:hover {
-  text-decoration: underline;
-}
-
-.markdown-body hr::before {
-  display: table;
-  content: "";
-}
-
-.markdown-body hr::after {
-  display: table;
-  clear: both;
-  content: "";
-}
-
-.markdown-body table {
-  border-spacing: 0;
-  border-collapse: collapse;
-  display: block;
-  width: max-content;
-  max-width: 100%;
-  overflow: auto;
-}
-
-.markdown-body td,
-.markdown-body th {
-  padding: 0;
-}
-
-.markdown-body details summary {
-  cursor: pointer;
-}
-
-.markdown-body details:not([open])>*:not(summary) {
-  display: none !important;
-}
-
-.markdown-body kbd {
-  display: inline-block;
-  padding: 3px 5px;
-  font: 11px ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
-  line-height: 10px;
-  color: #24292f;
-  vertical-align: middle;
-  background-color: #f6f8fa;
-  border: solid 1px rgba(175,184,193,0.2);
-  border-bottom-color: rgba(175,184,193,0.2);
-  border-radius: 6px;
-  box-shadow: inset 0 -1px 0 rgba(175,184,193,0.2);
-}
-
-.markdown-body h1,
-.markdown-body h2,
-.markdown-body h3,
-.markdown-body h4,
-.markdown-body h5,
-.markdown-body h6 {
-  margin-top: 24px;
-  margin-bottom: 16px;
-  font-weight: 600;
-  line-height: 1.25;
-}
-
-.markdown-body h2 {
-  font-weight: 600;
-  padding-bottom: .3em;
-  font-size: 1.5em;
-  border-bottom: 1px solid hsla(210,18%,87%,1);
-}
-
-.markdown-body h3 {
-  font-weight: 600;
-  font-size: 1.25em;
-}
-
-.markdown-body h4 {
-  font-weight: 600;
-  font-size: 1em;
-}
-
-.markdown-body h5 {
-  font-weight: 600;
-  font-size: .875em;
-}
-
-.markdown-body h6 {
-  font-weight: 600;
-  font-size: .85em;
-  color: #57606a;
-}
-
-.markdown-body p {
-  margin-top: 0;
-  margin-bottom: 10px;
-}
-
-.markdown-body blockquote {
-  margin: 0;
-  padding: 0 1em;
-  color: #57606a;
-  border-left: .25em solid #d0d7de;
-}
-
-.markdown-body ul,
-.markdown-body ol {
-  margin-top: 0;
-  margin-bottom: 0;
-  padding-left: 2em;
-}
-
-.markdown-body ol ol,
-.markdown-body ul ol {
-  list-style-type: lower-roman;
-}
-
-.markdown-body ul ul ol,
-.markdown-body ul ol ol,
-.markdown-body ol ul ol,
-.markdown-body ol ol ol {
-  list-style-type: lower-alpha;
-}
-
-.markdown-body dd {
-  margin-left: 0;
-}
-
-.markdown-body tt,
-.markdown-body code {
-  font-family: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
-  font-size: 12px;
-}
-
-.markdown-body pre {
-  margin-top: 0;
-  margin-bottom: 0;
-  font-family: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
-  font-size: 12px;
-  word-wrap: normal;
-}
-
-.markdown-body .octicon {
-  display: inline-block;
-  overflow: visible !important;
-  vertical-align: text-bottom;
-  fill: currentColor;
-}
-
-.markdown-body ::placeholder {
-  color: #6e7781;
-  opacity: 1;
-}
-
-.markdown-body input::-webkit-outer-spin-button,
-.markdown-body input::-webkit-inner-spin-button {
-  margin: 0;
-  -webkit-appearance: none;
-  appearance: none;
-}
-
-.markdown-body .pl-c {
-  color: #6e7781;
-}
-
-.markdown-body .pl-c1,
-.markdown-body .pl-s .pl-v {
-  color: #0550ae;
-}
-
-.markdown-body .pl-e,
-.markdown-body .pl-en {
-  color: #8250df;
-}
-
-.markdown-body .pl-smi,
-.markdown-body .pl-s .pl-s1 {
-  color: #24292f;
-}
-
-.markdown-body .pl-ent {
-  color: #116329;
-}
-
-.markdown-body .pl-k {
-  color: #cf222e;
-}
-
-.markdown-body .pl-s,
-.markdown-body .pl-pds,
-.markdown-body .pl-s .pl-pse .pl-s1,
-.markdown-body .pl-sr,
-.markdown-body .pl-sr .pl-cce,
-.markdown-body .pl-sr .pl-sre,
-.markdown-body .pl-sr .pl-sra {
-  color: #0a3069;
-}
-
-.markdown-body .pl-v,
-.markdown-body .pl-smw {
-  color: #953800;
-}
-
-.markdown-body .pl-bu {
-  color: #82071e;
-}
-
-.markdown-body .pl-ii {
-  color: #f6f8fa;
-  background-color: #82071e;
-}
-
-.markdown-body .pl-c2 {
-  color: #f6f8fa;
-  background-color: #cf222e;
-}
-
-.markdown-body .pl-sr .pl-cce {
-  font-weight: bold;
-  color: #116329;
-}
-
-.markdown-body .pl-ml {
-  color: #3b2300;
-}
-
-.markdown-body .pl-mh,
-.markdown-body .pl-mh .pl-en,
-.markdown-body .pl-ms {
-  font-weight: bold;
-  color: #0550ae;
-}
-
-.markdown-body .pl-mi {
-  font-style: italic;
-  color: #24292f;
-}
-
-.markdown-body .pl-mb {
-  font-weight: bold;
-  color: #24292f;
-}
-
-.markdown-body .pl-md {
-  color: #82071e;
-  background-color: #FFEBE9;
-}
-
-.markdown-body .pl-mi1 {
-  color: #116329;
-  background-color: #dafbe1;
-}
-
-.markdown-body .pl-mc {
-  color: #953800;
-  background-color: #ffd8b5;
-}
-
-.markdown-body .pl-mi2 {
-  color: #eaeef2;
-  background-color: #0550ae;
-}
-
-.markdown-body .pl-mdr {
-  font-weight: bold;
-  color: #8250df;
-}
-
-.markdown-body .pl-ba {
-  color: #57606a;
-}
-
-.markdown-body .pl-sg {
-  color: #8c959f;
-}
-
-.markdown-body .pl-corl {
-  text-decoration: underline;
-  color: #0a3069;
-}
-
-.markdown-body [data-catalyst] {
-  display: block;
-}
-
-.markdown-body g-emoji {
-  font-family: "Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
-  font-size: 1em;
-  font-style: normal !important;
-  font-weight: 400;
-  line-height: 1;
-  vertical-align: -0.075em;
-}
-
-.markdown-body g-emoji img {
-  width: 1em;
-  height: 1em;
-}
-
-.markdown-body::before {
-  display: table;
-  content: "";
-}
-
-.markdown-body::after {
-  display: table;
-  clear: both;
-  content: "";
-}
-
-.markdown-body>*:first-child {
-  margin-top: 0 !important;
-}
-
-.markdown-body>*:last-child {
-  margin-bottom: 0 !important;
-}
-
-.markdown-body a:not([href]) {
-  color: inherit;
-  text-decoration: none;
-}
-
-.markdown-body .absent {
-  color: #cf222e;
-}
-
-.markdown-body .anchor {
-  float: left;
-  padding-right: 4px;
-  margin-left: -20px;
-  line-height: 1;
-}
-
-.markdown-body .anchor:focus {
-  outline: none;
-}
-
-.markdown-body p,
-.markdown-body blockquote,
-.markdown-body ul,
-.markdown-body ol,
-.markdown-body dl,
-.markdown-body table,
-.markdown-body pre,
-.markdown-body details {
-  margin-top: 0;
-  margin-bottom: 16px;
-}
-
-.markdown-body blockquote>:first-child {
-  margin-top: 0;
-}
-
-.markdown-body blockquote>:last-child {
-  margin-bottom: 0;
-}
-
-.markdown-body sup>a::before {
-  content: "[";
-}
-
-.markdown-body sup>a::after {
-  content: "]";
-}
-
-.markdown-body h1 .octicon-link,
-.markdown-body h2 .octicon-link,
-.markdown-body h3 .octicon-link,
-.markdown-body h4 .octicon-link,
-.markdown-body h5 .octicon-link,
-.markdown-body h6 .octicon-link {
-  color: #24292f;
-  vertical-align: middle;
-  visibility: hidden;
-}
-
-.markdown-body h1:hover .anchor,
-.markdown-body h2:hover .anchor,
-.markdown-body h3:hover .anchor,
-.markdown-body h4:hover .anchor,
-.markdown-body h5:hover .anchor,
-.markdown-body h6:hover .anchor {
-  text-decoration: none;
-}
-
-.markdown-body h1:hover .anchor .octicon-link,
-.markdown-body h2:hover .anchor .octicon-link,
-.markdown-body h3:hover .anchor .octicon-link,
-.markdown-body h4:hover .anchor .octicon-link,
-.markdown-body h5:hover .anchor .octicon-link,
-.markdown-body h6:hover .anchor .octicon-link {
-  visibility: visible;
-}
-
-.markdown-body h1 tt,
-.markdown-body h1 code,
-.markdown-body h2 tt,
-.markdown-body h2 code,
-.markdown-body h3 tt,
-.markdown-body h3 code,
-.markdown-body h4 tt,
-.markdown-body h4 code,
-.markdown-body h5 tt,
-.markdown-body h5 code,
-.markdown-body h6 tt,
-.markdown-body h6 code {
-  padding: 0 .2em;
-  font-size: inherit;
-}
-
-.markdown-body ul.no-list,
-.markdown-body ol.no-list {
-  padding: 0;
-  list-style-type: none;
-}
-
-.markdown-body ol[type="1"] {
-  list-style-type: decimal;
-}
-
-.markdown-body ol[type=a] {
-  list-style-type: lower-alpha;
-}
-
-.markdown-body ol[type=i] {
-  list-style-type: lower-roman;
-}
-
-.markdown-body div>ol:not([type]) {
-  list-style-type: decimal;
-}
-
-.markdown-body ul ul,
-.markdown-body ul ol,
-.markdown-body ol ol,
-.markdown-body ol ul {
-  margin-top: 0;
-  margin-bottom: 0;
-}
-
-.markdown-body li>p {
-  margin-top: 16px;
-}
-
-.markdown-body li+li {
-  margin-top: .25em;
-}
-
-.markdown-body dl {
-  padding: 0;
-}
-
-.markdown-body dl dt {
-  padding: 0;
-  margin-top: 16px;
-  font-size: 1em;
-  font-style: italic;
-  font-weight: 600;
-}
-
-.markdown-body dl dd {
-  padding: 0 16px;
-  margin-bottom: 16px;
-}
-
-.markdown-body table th {
-  font-weight: 600;
-}
-
-.markdown-body table th,
-.markdown-body table td {
-  padding: 6px 13px;
-  border: 1px solid #d0d7de;
-}
-
-.markdown-body table tr {
-  background-color: #ffffff;
-  border-top: 1px solid hsla(210,18%,87%,1);
-}
-
-.markdown-body table tr:nth-child(2n) {
-  background-color: #f6f8fa;
-}
-
-.markdown-body table img {
-  background-color: transparent;
-}
-
-.markdown-body img[align=right] {
-  padding-left: 20px;
-}
-
-.markdown-body img[align=left] {
-  padding-right: 20px;
-}
-
-.markdown-body .emoji {
-  max-width: none;
-  vertical-align: text-top;
-  background-color: transparent;
-}
-
-.markdown-body span.frame {
-  display: block;
-  overflow: hidden;
-}
-
-.markdown-body span.frame>span {
-  display: block;
-  float: left;
-  width: auto;
-  padding: 7px;
-  margin: 13px 0 0;
-  overflow: hidden;
-  border: 1px solid #d0d7de;
-}
-
-.markdown-body span.frame span img {
-  display: block;
-  float: left;
-}
-
-.markdown-body span.frame span span {
-  display: block;
-  padding: 5px 0 0;
-  clear: both;
-  color: #24292f;
-}
-
-.markdown-body span.align-center {
-  display: block;
-  overflow: hidden;
-  clear: both;
-}
-
-.markdown-body span.align-center>span {
-  display: block;
-  margin: 13px auto 0;
-  overflow: hidden;
-  text-align: center;
-}
-
-.markdown-body span.align-center span img {
-  margin: 0 auto;
-  text-align: center;
-}
-
-.markdown-body span.align-right {
-  display: block;
-  overflow: hidden;
-  clear: both;
-}
-
-.markdown-body span.align-right>span {
-  display: block;
-  margin: 13px 0 0;
-  overflow: hidden;
-  text-align: right;
-}
-
-.markdown-body span.align-right span img {
-  margin: 0;
-  text-align: right;
-}
-
-.markdown-body span.float-left {
-  display: block;
-  float: left;
-  margin-right: 13px;
-  overflow: hidden;
-}
-
-.markdown-body span.float-left span {
-  margin: 13px 0 0;
-}
-
-.markdown-body span.float-right {
-  display: block;
-  float: right;
-  margin-left: 13px;
-  overflow: hidden;
-}
-
-.markdown-body span.float-right>span {
-  display: block;
-  margin: 13px auto 0;
-  overflow: hidden;
-  text-align: right;
-}
-
-.markdown-body code,
-.markdown-body tt {
-  padding: .2em .4em;
-  margin: 0;
-  font-size: 85%;
-  background-color: rgba(175,184,193,0.2);
-  border-radius: 6px;
-}
-
-.markdown-body code br,
-.markdown-body tt br {
-  display: none;
-}
-
-.markdown-body del code {
-  text-decoration: inherit;
-}
-
-.markdown-body pre code {
-  font-size: 100%;
-}
-
-.markdown-body pre>code {
-  padding: 0;
-  margin: 0;
-  word-break: normal;
-  white-space: pre;
-  background: transparent;
-  border: 0;
-}
-
-.markdown-body .highlight {
-  margin-bottom: 16px;
-}
-
-.markdown-body .highlight pre {
-  margin-bottom: 0;
-  word-break: normal;
-}
-
-.markdown-body .highlight pre,
-.markdown-body pre {
-  padding: 16px;
-  overflow: auto;
-  font-size: 85%;
-  line-height: 1.45;
-  background-color: #f6f8fa;
-  border-radius: 6px;
-}
-
-.markdown-body pre code,
-.markdown-body pre tt {
-  display: inline;
-  max-width: auto;
-  padding: 0;
-  margin: 0;
-  overflow: visible;
-  line-height: inherit;
-  word-wrap: normal;
-  background-color: transparent;
-  border: 0;
-}
-
-.markdown-body .csv-data td,
-.markdown-body .csv-data th {
-  padding: 5px;
-  overflow: hidden;
-  font-size: 12px;
-  line-height: 1;
-  text-align: left;
-  white-space: nowrap;
-}
-
-.markdown-body .csv-data .blob-num {
-  padding: 10px 8px 9px;
-  text-align: right;
-  background: #ffffff;
-  border: 0;
-}
-
-.markdown-body .csv-data tr {
-  border-top: 0;
-}
-
-.markdown-body .csv-data th {
-  font-weight: 600;
-  background: #f6f8fa;
-  border-top: 0;
-}
-
-.markdown-body .footnotes {
-  font-size: 12px;
-  color: #57606a;
-  border-top: 1px solid #d0d7de;
-}
-
-.markdown-body .footnotes ol {
-  padding-left: 16px;
-}
-
-.markdown-body .footnotes li {
-  position: relative;
-}
-
-.markdown-body .footnotes li:target::before {
-  position: absolute;
-  top: -8px;
-  right: -8px;
-  bottom: -8px;
-  left: -24px;
-  pointer-events: none;
-  content: "";
-  border: 2px solid #0969da;
-  border-radius: 6px;
-}
-
-.markdown-body .footnotes li:target {
-  color: #24292f;
-}
-
-.markdown-body .footnotes .data-footnote-backref g-emoji {
-  font-family: monospace;
-}
-
-.markdown-body .task-list-item {
-  list-style-type: none;
-}
-
-.markdown-body .task-list-item label {
-  font-weight: 400;
-}
-
-.markdown-body .task-list-item.enabled label {
-  cursor: pointer;
-}
-
-.markdown-body .task-list-item+.task-list-item {
-  margin-top: 3px;
-}
-
-.markdown-body .task-list-item .handle {
-  display: none;
-}
-
-.markdown-body .task-list-item-checkbox {
-  margin: 0 .2em .25em -1.6em;
-  vertical-align: middle;
-}
-
-.markdown-body .contains-task-list:dir(rtl) .task-list-item-checkbox {
-  margin: 0 -1.6em .25em .2em;
-}
-
-.markdown-body ::-webkit-calendar-picker-indicator {
-  filter: invert(50%);
-}
+.markdown-body {
+  -ms-text-size-adjust: 100%;
+  -webkit-text-size-adjust: 100%;
+  margin: 0;
+  color: #24292f;
+  background-color: #ffffff;
+  font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Helvetica,Arial,sans-serif,"Apple Color Emoji","Segoe UI Emoji";
+  font-size: 16px;
+  line-height: 1.5;
+  word-wrap: break-word;
+}
+
+.markdown-body .octicon {
+  display: inline-block;
+  fill: currentColor;
+  vertical-align: text-bottom;
+}
+
+.markdown-body h1:hover .anchor .octicon-link:before,
+.markdown-body h2:hover .anchor .octicon-link:before,
+.markdown-body h3:hover .anchor .octicon-link:before,
+.markdown-body h4:hover .anchor .octicon-link:before,
+.markdown-body h5:hover .anchor .octicon-link:before,
+.markdown-body h6:hover .anchor .octicon-link:before {
+  width: 16px;
+  height: 16px;
+  content: ' ';
+  display: inline-block;
+  background-color: currentColor;
+  -webkit-mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
+  mask-image: url("data:image/svg+xml,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16' version='1.1' aria-hidden='true'><path fill-rule='evenodd' d='M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z'></path></svg>");
+}
+
+.markdown-body details,
+.markdown-body figcaption,
+.markdown-body figure {
+  display: block;
+}
+
+.markdown-body summary {
+  display: list-item;
+}
+
+.markdown-body [hidden] {
+  display: none !important;
+}
+
+.markdown-body a {
+  background-color: transparent;
+  color: #0969da;
+  text-decoration: none;
+}
+
+.markdown-body a:active,
+.markdown-body a:hover {
+  outline-width: 0;
+}
+
+.markdown-body abbr[title] {
+  border-bottom: none;
+  text-decoration: underline dotted;
+}
+
+.markdown-body b,
+.markdown-body strong {
+  font-weight: 600;
+}
+
+.markdown-body dfn {
+  font-style: italic;
+}
+
+.markdown-body h1 {
+  margin: .67em 0;
+  font-weight: 600;
+  padding-bottom: .3em;
+  font-size: 2em;
+  border-bottom: 1px solid hsla(210,18%,87%,1);
+}
+
+.markdown-body mark {
+  background-color: #fff8c5;
+  color: #24292f;
+}
+
+.markdown-body small {
+  font-size: 90%;
+}
+
+.markdown-body sub,
+.markdown-body sup {
+  font-size: 75%;
+  line-height: 0;
+  position: relative;
+  vertical-align: baseline;
+}
+
+.markdown-body sub {
+  bottom: -0.25em;
+}
+
+.markdown-body sup {
+  top: -0.5em;
+}
+
+.markdown-body img {
+  border-style: none;
+  max-width: 100%;
+  box-sizing: content-box;
+  background-color: #ffffff;
+}
+
+.markdown-body code,
+.markdown-body kbd,
+.markdown-body pre,
+.markdown-body samp {
+  font-family: monospace,monospace;
+  font-size: 1em;
+}
+
+.markdown-body figure {
+  margin: 1em 40px;
+}
+
+.markdown-body hr {
+  box-sizing: content-box;
+  overflow: hidden;
+  background: transparent;
+  border-bottom: 1px solid hsla(210,18%,87%,1);
+  height: .25em;
+  padding: 0;
+  margin: 24px 0;
+  background-color: #d0d7de;
+  border: 0;
+}
+
+.markdown-body input {
+  font: inherit;
+  margin: 0;
+  overflow: visible;
+  font-family: inherit;
+  font-size: inherit;
+  line-height: inherit;
+}
+
+.markdown-body [type=button],
+.markdown-body [type=reset],
+.markdown-body [type=submit] {
+  -webkit-appearance: button;
+}
+
+.markdown-body [type=button]::-moz-focus-inner,
+.markdown-body [type=reset]::-moz-focus-inner,
+.markdown-body [type=submit]::-moz-focus-inner {
+  border-style: none;
+  padding: 0;
+}
+
+.markdown-body [type=button]:-moz-focusring,
+.markdown-body [type=reset]:-moz-focusring,
+.markdown-body [type=submit]:-moz-focusring {
+  outline: 1px dotted ButtonText;
+}
+
+.markdown-body [type=checkbox],
+.markdown-body [type=radio] {
+  box-sizing: border-box;
+  padding: 0;
+}
+
+.markdown-body [type=number]::-webkit-inner-spin-button,
+.markdown-body [type=number]::-webkit-outer-spin-button {
+  height: auto;
+}
+
+.markdown-body [type=search] {
+  -webkit-appearance: textfield;
+  outline-offset: -2px;
+}
+
+.markdown-body [type=search]::-webkit-search-cancel-button,
+.markdown-body [type=search]::-webkit-search-decoration {
+  -webkit-appearance: none;
+}
+
+.markdown-body ::-webkit-input-placeholder {
+  color: inherit;
+  opacity: .54;
+}
+
+.markdown-body ::-webkit-file-upload-button {
+  -webkit-appearance: button;
+  font: inherit;
+}
+
+.markdown-body a:hover {
+  text-decoration: underline;
+}
+
+.markdown-body hr::before {
+  display: table;
+  content: "";
+}
+
+.markdown-body hr::after {
+  display: table;
+  clear: both;
+  content: "";
+}
+
+.markdown-body table {
+  border-spacing: 0;
+  border-collapse: collapse;
+  display: block;
+  width: max-content;
+  max-width: 100%;
+  overflow: auto;
+}
+
+.markdown-body td,
+.markdown-body th {
+  padding: 0;
+}
+
+.markdown-body details summary {
+  cursor: pointer;
+}
+
+.markdown-body details:not([open])>*:not(summary) {
+  display: none !important;
+}
+
+.markdown-body kbd {
+  display: inline-block;
+  padding: 3px 5px;
+  font: 11px ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
+  line-height: 10px;
+  color: #24292f;
+  vertical-align: middle;
+  background-color: #f6f8fa;
+  border: solid 1px rgba(175,184,193,0.2);
+  border-bottom-color: rgba(175,184,193,0.2);
+  border-radius: 6px;
+  box-shadow: inset 0 -1px 0 rgba(175,184,193,0.2);
+}
+
+.markdown-body h1,
+.markdown-body h2,
+.markdown-body h3,
+.markdown-body h4,
+.markdown-body h5,
+.markdown-body h6 {
+  margin-top: 24px;
+  margin-bottom: 16px;
+  font-weight: 600;
+  line-height: 1.25;
+}
+
+.markdown-body h2 {
+  font-weight: 600;
+  padding-bottom: .3em;
+  font-size: 1.5em;
+  border-bottom: 1px solid hsla(210,18%,87%,1);
+}
+
+.markdown-body h3 {
+  font-weight: 600;
+  font-size: 1.25em;
+}
+
+.markdown-body h4 {
+  font-weight: 600;
+  font-size: 1em;
+}
+
+.markdown-body h5 {
+  font-weight: 600;
+  font-size: .875em;
+}
+
+.markdown-body h6 {
+  font-weight: 600;
+  font-size: .85em;
+  color: #57606a;
+}
+
+.markdown-body p {
+  margin-top: 0;
+  margin-bottom: 10px;
+}
+
+.markdown-body blockquote {
+  margin: 0;
+  padding: 0 1em;
+  color: #57606a;
+  border-left: .25em solid #d0d7de;
+}
+
+.markdown-body ul,
+.markdown-body ol {
+  margin-top: 0;
+  margin-bottom: 0;
+  padding-left: 2em;
+}
+
+.markdown-body ol ol,
+.markdown-body ul ol {
+  list-style-type: lower-roman;
+}
+
+.markdown-body ul ul ol,
+.markdown-body ul ol ol,
+.markdown-body ol ul ol,
+.markdown-body ol ol ol {
+  list-style-type: lower-alpha;
+}
+
+.markdown-body dd {
+  margin-left: 0;
+}
+
+.markdown-body tt,
+.markdown-body code {
+  font-family: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
+  font-size: 12px;
+}
+
+.markdown-body pre {
+  margin-top: 0;
+  margin-bottom: 0;
+  font-family: ui-monospace,SFMono-Regular,SF Mono,Menlo,Consolas,Liberation Mono,monospace;
+  font-size: 12px;
+  word-wrap: normal;
+}
+
+.markdown-body .octicon {
+  display: inline-block;
+  overflow: visible !important;
+  vertical-align: text-bottom;
+  fill: currentColor;
+}
+
+.markdown-body ::placeholder {
+  color: #6e7781;
+  opacity: 1;
+}
+
+.markdown-body input::-webkit-outer-spin-button,
+.markdown-body input::-webkit-inner-spin-button {
+  margin: 0;
+  -webkit-appearance: none;
+  appearance: none;
+}
+
+.markdown-body .pl-c {
+  color: #6e7781;
+}
+
+.markdown-body .pl-c1,
+.markdown-body .pl-s .pl-v {
+  color: #0550ae;
+}
+
+.markdown-body .pl-e,
+.markdown-body .pl-en {
+  color: #8250df;
+}
+
+.markdown-body .pl-smi,
+.markdown-body .pl-s .pl-s1 {
+  color: #24292f;
+}
+
+.markdown-body .pl-ent {
+  color: #116329;
+}
+
+.markdown-body .pl-k {
+  color: #cf222e;
+}
+
+.markdown-body .pl-s,
+.markdown-body .pl-pds,
+.markdown-body .pl-s .pl-pse .pl-s1,
+.markdown-body .pl-sr,
+.markdown-body .pl-sr .pl-cce,
+.markdown-body .pl-sr .pl-sre,
+.markdown-body .pl-sr .pl-sra {
+  color: #0a3069;
+}
+
+.markdown-body .pl-v,
+.markdown-body .pl-smw {
+  color: #953800;
+}
+
+.markdown-body .pl-bu {
+  color: #82071e;
+}
+
+.markdown-body .pl-ii {
+  color: #f6f8fa;
+  background-color: #82071e;
+}
+
+.markdown-body .pl-c2 {
+  color: #f6f8fa;
+  background-color: #cf222e;
+}
+
+.markdown-body .pl-sr .pl-cce {
+  font-weight: bold;
+  color: #116329;
+}
+
+.markdown-body .pl-ml {
+  color: #3b2300;
+}
+
+.markdown-body .pl-mh,
+.markdown-body .pl-mh .pl-en,
+.markdown-body .pl-ms {
+  font-weight: bold;
+  color: #0550ae;
+}
+
+.markdown-body .pl-mi {
+  font-style: italic;
+  color: #24292f;
+}
+
+.markdown-body .pl-mb {
+  font-weight: bold;
+  color: #24292f;
+}
+
+.markdown-body .pl-md {
+  color: #82071e;
+  background-color: #FFEBE9;
+}
+
+.markdown-body .pl-mi1 {
+  color: #116329;
+  background-color: #dafbe1;
+}
+
+.markdown-body .pl-mc {
+  color: #953800;
+  background-color: #ffd8b5;
+}
+
+.markdown-body .pl-mi2 {
+  color: #eaeef2;
+  background-color: #0550ae;
+}
+
+.markdown-body .pl-mdr {
+  font-weight: bold;
+  color: #8250df;
+}
+
+.markdown-body .pl-ba {
+  color: #57606a;
+}
+
+.markdown-body .pl-sg {
+  color: #8c959f;
+}
+
+.markdown-body .pl-corl {
+  text-decoration: underline;
+  color: #0a3069;
+}
+
+.markdown-body [data-catalyst] {
+  display: block;
+}
+
+.markdown-body g-emoji {
+  font-family: "Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
+  font-size: 1em;
+  font-style: normal !important;
+  font-weight: 400;
+  line-height: 1;
+  vertical-align: -0.075em;
+}
+
+.markdown-body g-emoji img {
+  width: 1em;
+  height: 1em;
+}
+
+.markdown-body::before {
+  display: table;
+  content: "";
+}
+
+.markdown-body::after {
+  display: table;
+  clear: both;
+  content: "";
+}
+
+.markdown-body>*:first-child {
+  margin-top: 0 !important;
+}
+
+.markdown-body>*:last-child {
+  margin-bottom: 0 !important;
+}
+
+.markdown-body a:not([href]) {
+  color: inherit;
+  text-decoration: none;
+}
+
+.markdown-body .absent {
+  color: #cf222e;
+}
+
+.markdown-body .anchor {
+  float: left;
+  padding-right: 4px;
+  margin-left: -20px;
+  line-height: 1;
+}
+
+.markdown-body .anchor:focus {
+  outline: none;
+}
+
+.markdown-body p,
+.markdown-body blockquote,
+.markdown-body ul,
+.markdown-body ol,
+.markdown-body dl,
+.markdown-body table,
+.markdown-body pre,
+.markdown-body details {
+  margin-top: 0;
+  margin-bottom: 16px;
+}
+
+.markdown-body blockquote>:first-child {
+  margin-top: 0;
+}
+
+.markdown-body blockquote>:last-child {
+  margin-bottom: 0;
+}
+
+.markdown-body sup>a::before {
+  content: "[";
+}
+
+.markdown-body sup>a::after {
+  content: "]";
+}
+
+.markdown-body h1 .octicon-link,
+.markdown-body h2 .octicon-link,
+.markdown-body h3 .octicon-link,
+.markdown-body h4 .octicon-link,
+.markdown-body h5 .octicon-link,
+.markdown-body h6 .octicon-link {
+  color: #24292f;
+  vertical-align: middle;
+  visibility: hidden;
+}
+
+.markdown-body h1:hover .anchor,
+.markdown-body h2:hover .anchor,
+.markdown-body h3:hover .anchor,
+.markdown-body h4:hover .anchor,
+.markdown-body h5:hover .anchor,
+.markdown-body h6:hover .anchor {
+  text-decoration: none;
+}
+
+.markdown-body h1:hover .anchor .octicon-link,
+.markdown-body h2:hover .anchor .octicon-link,
+.markdown-body h3:hover .anchor .octicon-link,
+.markdown-body h4:hover .anchor .octicon-link,
+.markdown-body h5:hover .anchor .octicon-link,
+.markdown-body h6:hover .anchor .octicon-link {
+  visibility: visible;
+}
+
+.markdown-body h1 tt,
+.markdown-body h1 code,
+.markdown-body h2 tt,
+.markdown-body h2 code,
+.markdown-body h3 tt,
+.markdown-body h3 code,
+.markdown-body h4 tt,
+.markdown-body h4 code,
+.markdown-body h5 tt,
+.markdown-body h5 code,
+.markdown-body h6 tt,
+.markdown-body h6 code {
+  padding: 0 .2em;
+  font-size: inherit;
+}
+
+.markdown-body ul.no-list,
+.markdown-body ol.no-list {
+  padding: 0;
+  list-style-type: none;
+}
+
+.markdown-body ol[type="1"] {
+  list-style-type: decimal;
+}
+
+.markdown-body ol[type=a] {
+  list-style-type: lower-alpha;
+}
+
+.markdown-body ol[type=i] {
+  list-style-type: lower-roman;
+}
+
+.markdown-body div>ol:not([type]) {
+  list-style-type: decimal;
+}
+
+.markdown-body ul ul,
+.markdown-body ul ol,
+.markdown-body ol ol,
+.markdown-body ol ul {
+  margin-top: 0;
+  margin-bottom: 0;
+}
+
+.markdown-body li>p {
+  margin-top: 16px;
+}
+
+.markdown-body li+li {
+  margin-top: .25em;
+}
+
+.markdown-body dl {
+  padding: 0;
+}
+
+.markdown-body dl dt {
+  padding: 0;
+  margin-top: 16px;
+  font-size: 1em;
+  font-style: italic;
+  font-weight: 600;
+}
+
+.markdown-body dl dd {
+  padding: 0 16px;
+  margin-bottom: 16px;
+}
+
+.markdown-body table th {
+  font-weight: 600;
+}
+
+.markdown-body table th,
+.markdown-body table td {
+  padding: 6px 13px;
+  border: 1px solid #d0d7de;
+}
+
+.markdown-body table tr {
+  background-color: #ffffff;
+  border-top: 1px solid hsla(210,18%,87%,1);
+}
+
+.markdown-body table tr:nth-child(2n) {
+  background-color: #f6f8fa;
+}
+
+.markdown-body table img {
+  background-color: transparent;
+}
+
+.markdown-body img[align=right] {
+  padding-left: 20px;
+}
+
+.markdown-body img[align=left] {
+  padding-right: 20px;
+}
+
+.markdown-body .emoji {
+  max-width: none;
+  vertical-align: text-top;
+  background-color: transparent;
+}
+
+.markdown-body span.frame {
+  display: block;
+  overflow: hidden;
+}
+
+.markdown-body span.frame>span {
+  display: block;
+  float: left;
+  width: auto;
+  padding: 7px;
+  margin: 13px 0 0;
+  overflow: hidden;
+  border: 1px solid #d0d7de;
+}
+
+.markdown-body span.frame span img {
+  display: block;
+  float: left;
+}
+
+.markdown-body span.frame span span {
+  display: block;
+  padding: 5px 0 0;
+  clear: both;
+  color: #24292f;
+}
+
+.markdown-body span.align-center {
+  display: block;
+  overflow: hidden;
+  clear: both;
+}
+
+.markdown-body span.align-center>span {
+  display: block;
+  margin: 13px auto 0;
+  overflow: hidden;
+  text-align: center;
+}
+
+.markdown-body span.align-center span img {
+  margin: 0 auto;
+  text-align: center;
+}
+
+.markdown-body span.align-right {
+  display: block;
+  overflow: hidden;
+  clear: both;
+}
+
+.markdown-body span.align-right>span {
+  display: block;
+  margin: 13px 0 0;
+  overflow: hidden;
+  text-align: right;
+}
+
+.markdown-body span.align-right span img {
+  margin: 0;
+  text-align: right;
+}
+
+.markdown-body span.float-left {
+  display: block;
+  float: left;
+  margin-right: 13px;
+  overflow: hidden;
+}
+
+.markdown-body span.float-left span {
+  margin: 13px 0 0;
+}
+
+.markdown-body span.float-right {
+  display: block;
+  float: right;
+  margin-left: 13px;
+  overflow: hidden;
+}
+
+.markdown-body span.float-right>span {
+  display: block;
+  margin: 13px auto 0;
+  overflow: hidden;
+  text-align: right;
+}
+
+.markdown-body code,
+.markdown-body tt {
+  padding: .2em .4em;
+  margin: 0;
+  font-size: 85%;
+  background-color: rgba(175,184,193,0.2);
+  border-radius: 6px;
+}
+
+.markdown-body code br,
+.markdown-body tt br {
+  display: none;
+}
+
+.markdown-body del code {
+  text-decoration: inherit;
+}
+
+.markdown-body pre code {
+  font-size: 100%;
+}
+
+.markdown-body pre>code {
+  padding: 0;
+  margin: 0;
+  word-break: normal;
+  white-space: pre;
+  background: transparent;
+  border: 0;
+}
+
+.markdown-body .highlight {
+  margin-bottom: 16px;
+}
+
+.markdown-body .highlight pre {
+  margin-bottom: 0;
+  word-break: normal;
+}
+
+.markdown-body .highlight pre,
+.markdown-body pre {
+  padding: 16px;
+  overflow: auto;
+  font-size: 85%;
+  line-height: 1.45;
+  background-color: #f6f8fa;
+  border-radius: 6px;
+}
+
+.markdown-body pre code,
+.markdown-body pre tt {
+  display: inline;
+  max-width: auto;
+  padding: 0;
+  margin: 0;
+  overflow: visible;
+  line-height: inherit;
+  word-wrap: normal;
+  background-color: transparent;
+  border: 0;
+}
+
+.markdown-body .csv-data td,
+.markdown-body .csv-data th {
+  padding: 5px;
+  overflow: hidden;
+  font-size: 12px;
+  line-height: 1;
+  text-align: left;
+  white-space: nowrap;
+}
+
+.markdown-body .csv-data .blob-num {
+  padding: 10px 8px 9px;
+  text-align: right;
+  background: #ffffff;
+  border: 0;
+}
+
+.markdown-body .csv-data tr {
+  border-top: 0;
+}
+
+.markdown-body .csv-data th {
+  font-weight: 600;
+  background: #f6f8fa;
+  border-top: 0;
+}
+
+.markdown-body .footnotes {
+  font-size: 12px;
+  color: #57606a;
+  border-top: 1px solid #d0d7de;
+}
+
+.markdown-body .footnotes ol {
+  padding-left: 16px;
+}
+
+.markdown-body .footnotes li {
+  position: relative;
+}
+
+.markdown-body .footnotes li:target::before {
+  position: absolute;
+  top: -8px;
+  right: -8px;
+  bottom: -8px;
+  left: -24px;
+  pointer-events: none;
+  content: "";
+  border: 2px solid #0969da;
+  border-radius: 6px;
+}
+
+.markdown-body .footnotes li:target {
+  color: #24292f;
+}
+
+.markdown-body .footnotes .data-footnote-backref g-emoji {
+  font-family: monospace;
+}
+
+.markdown-body .task-list-item {
+  list-style-type: none;
+}
+
+.markdown-body .task-list-item label {
+  font-weight: 400;
+}
+
+.markdown-body .task-list-item.enabled label {
+  cursor: pointer;
+}
+
+.markdown-body .task-list-item+.task-list-item {
+  margin-top: 3px;
+}
+
+.markdown-body .task-list-item .handle {
+  display: none;
+}
+
+.markdown-body .task-list-item-checkbox {
+  margin: 0 .2em .25em -1.6em;
+  vertical-align: middle;
+}
+
+.markdown-body .contains-task-list:dir(rtl) .task-list-item-checkbox {
+  margin: 0 -1.6em .25em .2em;
+}
+
+.markdown-body ::-webkit-calendar-picker-indicator {
+  filter: invert(50%);
+}
```

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/katex/katex.min.js` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/nonebot_plugin_htmlrender/templates/pygments-default.css` & `nonebot_plugin_htmlrender-0.2.1/nonebot_plugin_htmlrender/templates/pygments-default.css`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-pre { line-height: 125%; }
-td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
-span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
-td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
-span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
-.codehilite .hll { background-color: #ffffcc }
-.codehilite { background: #f8f8f8; }
-.codehilite .c { color: #408080; font-style: italic } /* Comment */
-.codehilite .err { border: 1px solid #FF0000 } /* Error */
-.codehilite .k { color: #008000; font-weight: bold } /* Keyword */
-.codehilite .o { color: #666666 } /* Operator */
-.codehilite .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
-.codehilite .cm { color: #408080; font-style: italic } /* Comment.Multiline */
-.codehilite .cp { color: #BC7A00 } /* Comment.Preproc */
-.codehilite .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
-.codehilite .c1 { color: #408080; font-style: italic } /* Comment.Single */
-.codehilite .cs { color: #408080; font-style: italic } /* Comment.Special */
-.codehilite .gd { color: #A00000 } /* Generic.Deleted */
-.codehilite .ge { font-style: italic } /* Generic.Emph */
-.codehilite .gr { color: #FF0000 } /* Generic.Error */
-.codehilite .gh { color: #000080; font-weight: bold } /* Generic.Heading */
-.codehilite .gi { color: #00A000 } /* Generic.Inserted */
-.codehilite .go { color: #888888 } /* Generic.Output */
-.codehilite .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
-.codehilite .gs { font-weight: bold } /* Generic.Strong */
-.codehilite .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
-.codehilite .gt { color: #0044DD } /* Generic.Traceback */
-.codehilite .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
-.codehilite .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
-.codehilite .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
-.codehilite .kp { color: #008000 } /* Keyword.Pseudo */
-.codehilite .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
-.codehilite .kt { color: #B00040 } /* Keyword.Type */
-.codehilite .m { color: #666666 } /* Literal.Number */
-.codehilite .s { color: #BA2121 } /* Literal.String */
-.codehilite .na { color: #7D9029 } /* Name.Attribute */
-.codehilite .nb { color: #008000 } /* Name.Builtin */
-.codehilite .nc { color: #0000FF; font-weight: bold } /* Name.Class */
-.codehilite .no { color: #880000 } /* Name.Constant */
-.codehilite .nd { color: #AA22FF } /* Name.Decorator */
-.codehilite .ni { color: #999999; font-weight: bold } /* Name.Entity */
-.codehilite .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
-.codehilite .nf { color: #0000FF } /* Name.Function */
-.codehilite .nl { color: #A0A000 } /* Name.Label */
-.codehilite .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
-.codehilite .nt { color: #008000; font-weight: bold } /* Name.Tag */
-.codehilite .nv { color: #19177C } /* Name.Variable */
-.codehilite .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
-.codehilite .w { color: #bbbbbb } /* Text.Whitespace */
-.codehilite .mb { color: #666666 } /* Literal.Number.Bin */
-.codehilite .mf { color: #666666 } /* Literal.Number.Float */
-.codehilite .mh { color: #666666 } /* Literal.Number.Hex */
-.codehilite .mi { color: #666666 } /* Literal.Number.Integer */
-.codehilite .mo { color: #666666 } /* Literal.Number.Oct */
-.codehilite .sa { color: #BA2121 } /* Literal.String.Affix */
-.codehilite .sb { color: #BA2121 } /* Literal.String.Backtick */
-.codehilite .sc { color: #BA2121 } /* Literal.String.Char */
-.codehilite .dl { color: #BA2121 } /* Literal.String.Delimiter */
-.codehilite .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
-.codehilite .s2 { color: #BA2121 } /* Literal.String.Double */
-.codehilite .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
-.codehilite .sh { color: #BA2121 } /* Literal.String.Heredoc */
-.codehilite .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
-.codehilite .sx { color: #008000 } /* Literal.String.Other */
-.codehilite .sr { color: #BB6688 } /* Literal.String.Regex */
-.codehilite .s1 { color: #BA2121 } /* Literal.String.Single */
-.codehilite .ss { color: #19177C } /* Literal.String.Symbol */
-.codehilite .bp { color: #008000 } /* Name.Builtin.Pseudo */
-.codehilite .fm { color: #0000FF } /* Name.Function.Magic */
-.codehilite .vc { color: #19177C } /* Name.Variable.Class */
-.codehilite .vg { color: #19177C } /* Name.Variable.Global */
-.codehilite .vi { color: #19177C } /* Name.Variable.Instance */
-.codehilite .vm { color: #19177C } /* Name.Variable.Magic */
-.codehilite .il { color: #666666 } /* Literal.Number.Integer.Long */
+pre { line-height: 125%; }
+td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
+td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
+span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
+.codehilite .hll { background-color: #ffffcc }
+.codehilite { background: #f8f8f8; }
+.codehilite .c { color: #408080; font-style: italic } /* Comment */
+.codehilite .err { border: 1px solid #FF0000 } /* Error */
+.codehilite .k { color: #008000; font-weight: bold } /* Keyword */
+.codehilite .o { color: #666666 } /* Operator */
+.codehilite .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
+.codehilite .cm { color: #408080; font-style: italic } /* Comment.Multiline */
+.codehilite .cp { color: #BC7A00 } /* Comment.Preproc */
+.codehilite .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
+.codehilite .c1 { color: #408080; font-style: italic } /* Comment.Single */
+.codehilite .cs { color: #408080; font-style: italic } /* Comment.Special */
+.codehilite .gd { color: #A00000 } /* Generic.Deleted */
+.codehilite .ge { font-style: italic } /* Generic.Emph */
+.codehilite .gr { color: #FF0000 } /* Generic.Error */
+.codehilite .gh { color: #000080; font-weight: bold } /* Generic.Heading */
+.codehilite .gi { color: #00A000 } /* Generic.Inserted */
+.codehilite .go { color: #888888 } /* Generic.Output */
+.codehilite .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
+.codehilite .gs { font-weight: bold } /* Generic.Strong */
+.codehilite .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
+.codehilite .gt { color: #0044DD } /* Generic.Traceback */
+.codehilite .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
+.codehilite .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
+.codehilite .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
+.codehilite .kp { color: #008000 } /* Keyword.Pseudo */
+.codehilite .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
+.codehilite .kt { color: #B00040 } /* Keyword.Type */
+.codehilite .m { color: #666666 } /* Literal.Number */
+.codehilite .s { color: #BA2121 } /* Literal.String */
+.codehilite .na { color: #7D9029 } /* Name.Attribute */
+.codehilite .nb { color: #008000 } /* Name.Builtin */
+.codehilite .nc { color: #0000FF; font-weight: bold } /* Name.Class */
+.codehilite .no { color: #880000 } /* Name.Constant */
+.codehilite .nd { color: #AA22FF } /* Name.Decorator */
+.codehilite .ni { color: #999999; font-weight: bold } /* Name.Entity */
+.codehilite .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
+.codehilite .nf { color: #0000FF } /* Name.Function */
+.codehilite .nl { color: #A0A000 } /* Name.Label */
+.codehilite .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
+.codehilite .nt { color: #008000; font-weight: bold } /* Name.Tag */
+.codehilite .nv { color: #19177C } /* Name.Variable */
+.codehilite .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
+.codehilite .w { color: #bbbbbb } /* Text.Whitespace */
+.codehilite .mb { color: #666666 } /* Literal.Number.Bin */
+.codehilite .mf { color: #666666 } /* Literal.Number.Float */
+.codehilite .mh { color: #666666 } /* Literal.Number.Hex */
+.codehilite .mi { color: #666666 } /* Literal.Number.Integer */
+.codehilite .mo { color: #666666 } /* Literal.Number.Oct */
+.codehilite .sa { color: #BA2121 } /* Literal.String.Affix */
+.codehilite .sb { color: #BA2121 } /* Literal.String.Backtick */
+.codehilite .sc { color: #BA2121 } /* Literal.String.Char */
+.codehilite .dl { color: #BA2121 } /* Literal.String.Delimiter */
+.codehilite .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
+.codehilite .s2 { color: #BA2121 } /* Literal.String.Double */
+.codehilite .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
+.codehilite .sh { color: #BA2121 } /* Literal.String.Heredoc */
+.codehilite .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
+.codehilite .sx { color: #008000 } /* Literal.String.Other */
+.codehilite .sr { color: #BB6688 } /* Literal.String.Regex */
+.codehilite .s1 { color: #BA2121 } /* Literal.String.Single */
+.codehilite .ss { color: #19177C } /* Literal.String.Symbol */
+.codehilite .bp { color: #008000 } /* Name.Builtin.Pseudo */
+.codehilite .fm { color: #0000FF } /* Name.Function.Magic */
+.codehilite .vc { color: #19177C } /* Name.Variable.Class */
+.codehilite .vg { color: #19177C } /* Name.Variable.Global */
+.codehilite .vi { color: #19177C } /* Name.Variable.Instance */
+.codehilite .vm { color: #19177C } /* Name.Variable.Magic */
+.codehilite .il { color: #666666 } /* Literal.Number.Integer.Long */
```

### Comparing `nonebot_plugin_htmlrender-0.2.0.3/README.md` & `nonebot_plugin_htmlrender-0.2.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,117 @@
-# nonebot-plugin-htmlrender
-
-- 通过浏览器渲染图片
-- 可通过查看`example`参考使用实例
-- 如果有安装浏览器等问题，先查看文档最底下的`常见问题`再去看 issue 有没有已经存在的
-
-# ✨ 功能
-
-- 通过 html 和浏览器生成图片
-- 支持`纯文本` `markdown` 和 `jinja2` 模板输入
-- 通过 CSS 来控制样式
-
-# 使用
-
-参考[example/plugins/render/**init**.py](example/plugins/render/__init__.py)
-
-# 配置
-
-```ini
-# 默认情况 可不写
-htmlrender_browser = "chromium"
-# 使用 firefox
-htmlrender_browser = "firefox"
-```
-
-## markdown 转 图片
-
-- 使用 `GitHub-light` 样式
-- 支持绝大部分 md 语法
-- 代码高亮
-- latex 数学公式 （感谢@[MeetWq](https://github.com/MeetWq)）
-  - 使用 `$$...$$` 来输入独立公式
-  - 使用 `$...$` 来输入行内公式
-- 图片需要使用外部连接并使用`html`格式 否则文末会超出截图范围
-- 图片可使用 md 语法 路径可为 `绝对路径`(建议), 或 `相对于template_path` 的路径
-
-## 模板 转 图片
-
-- 使用 jinja2 模板引擎
-- 页面参数可自定义
-
-# 🌰 栗子
-
-[example.md](docs/example.md)
-
-## 文本转图片（同时文本里面可以包括 html 图片）
-
-![](docs/text2pic.png)
-
-## markdown 转图片（同时文本里面可以包括 html 图片）
-
-![](docs/md2pic.png)
-
-## 纯 html 转图片
-
-![](docs/html2pic.png)
-
-## jinja2 模板转图片
-
-![](docs/template2pic.png)
-
-# 特别感谢
-
-- [MeetWq](https://github.com/MeetWq) 提供数学公式支持代码和代码高亮
-
-# 常见疑难杂症
-
-## `playwright._impl._api_types.Error:` 初次运行时报错
-
-- 一般为缺少必要的运行环境，如中文字体等
-
-### Ubuntu 使用 `apt`
-
-- 参考[Dao-bot Dockerfile](https://github.com/kexue-z/Dao-bot/blob/a7b35d6877b24b2bbd72039195bd1b3afebb5cf6/Dockerfile#L12-L15)
-
-```sh
-apt update && apt install -y locales locales-all fonts-noto libnss3-dev libxss1 libasound2 libxrandr2 libatk1.0-0 libgtk-3-0 libgbm-dev libxshmfence1
-```
-
-- 然后设置 ENV local
-
-```sh
-LANG zh_CN.UTF-8
-LANGUAGE zh_CN.UTF-8
-LC_ALL zh_CN.UTF-8
-```
-
-### CentOS 使用 `yum`
-
-- ~~小心 CentOS~~
-- 参考[CentOS Dockerfile](https://github.com/kumaraditya303/playwright-centos/blob/master/Dockerfile)
-- 添加中文字体库
-- ~~最佳解决办法~~
-  - 使用 Docker 然后用 Python 镜像 按照上面 Ubuntu 的写 `dockerfile`
-
-下面这个依赖运行一下 也许就可以用了
-
-```sh
-dnf install -y alsa-lib at-spi2-atk at-spi2-core atk cairo cups-libs dbus-libs expat flac-libs gdk-pixbuf2 glib2 glibc gtk3 libX11 libXcomposite libXdamage libXext libXfixes libXrandr libXtst libcanberra-gtk3 libdrm libgcc libstdc++ libxcb libxkbcommon libxshmfence libxslt mesa-libgbm nspr nss nss-util pango policycoreutils policycoreutils-python-utils zlib cairo-gobject centos-indexhtml dbus-glib fontconfig freetype gtk2 libXcursor libXi libXrender libXt liberation-fonts-common liberation-sans-fonts libffi mozilla-filesystem p11-kit-trust pipewire-libs harfbuzz-icu libglvnd-glx libglvnd-egl libnotify opus woff2 gstreamer1-plugins-base gstreamer1-plugins-bad-free openjpeg2 libwebp enchant libsecret hyphen libglvnd-gles
-```
+# nonebot-plugin-htmlrender
+
+- 通过浏览器渲染图片
+- 可通过查看`example`参考使用实例
+- 如果有安装浏览器等问题，先查看文档最底下的`常见问题`再去看 issue 有没有已经存在的
+
+# ✨ 功能
+
+- 通过 html 和浏览器生成图片
+- 支持`纯文本` `markdown` 和 `jinja2` 模板输入
+- 通过 CSS 来控制样式
+
+# 使用
+
+参考[example/plugins/render/**init**.py](example/plugins/render/__init__.py)
+
+```py
+from nonebot import require
+require("nonebot_plugin_htmlrender")
+# 注意顺序，先require再 from ... import ...
+# 注意顺序，先require再 from ... import ...
+# 注意顺序，先require再 from ... import ...
+from nonebot_plugin_htmlrender import (
+    text_to_pic,
+    md_to_pic,
+    template_to_pic,
+    get_new_page,
+)
+# 注意顺序，先require再 from ... import ...
+# 注意顺序，先require再 from ... import ...
+# 注意顺序，先require再 from ... import ...
+```
+
+# 配置
+
+```ini
+# 默认情况 可不写
+htmlrender_browser = "chromium"
+# 使用 firefox
+htmlrender_browser = "firefox"
+```
+
+## markdown 转 图片
+
+- 使用 `GitHub-light` 样式
+- 支持绝大部分 md 语法
+- 代码高亮
+- latex 数学公式 （感谢@[MeetWq](https://github.com/MeetWq)）
+  - 使用 `$$...$$` 来输入独立公式
+  - 使用 `$...$` 来输入行内公式
+- 图片需要使用外部连接并使用`html`格式 否则文末会超出截图范围
+- 图片可使用 md 语法 路径可为 `绝对路径`(建议), 或 `相对于template_path` 的路径
+
+## 模板 转 图片
+
+- 使用 jinja2 模板引擎
+- 页面参数可自定义
+
+# 🌰 栗子
+
+[example.md](docs/example.md)
+
+## 文本转图片（同时文本里面可以包括 html 图片）
+
+![](docs/text2pic.png)
+
+## markdown 转图片（同时文本里面可以包括 html 图片）
+
+![](docs/md2pic.png)
+
+## 纯 html 转图片
+
+![](docs/html2pic.png)
+
+## jinja2 模板转图片
+
+![](docs/template2pic.png)
+
+# 特别感谢
+
+- [MeetWq](https://github.com/MeetWq) 提供数学公式支持代码和代码高亮
+
+# 常见疑难杂症
+
+## `playwright._impl._api_types.Error:` 初次运行时报错
+
+- 一般为缺少必要的运行环境，如中文字体等
+
+### Ubuntu 使用 `apt`
+
+- 参考[Dao-bot Dockerfile](https://github.com/kexue-z/Dao-bot/blob/a7b35d6877b24b2bbd72039195bd1b3afebb5cf6/Dockerfile#L12-L15)
+
+```sh
+apt update && apt install -y locales locales-all fonts-noto libnss3-dev libxss1 libasound2 libxrandr2 libatk1.0-0 libgtk-3-0 libgbm-dev libxshmfence1
+```
+
+- 然后设置 ENV local
+
+```sh
+LANG zh_CN.UTF-8
+LANGUAGE zh_CN.UTF-8
+LC_ALL zh_CN.UTF-8
+```
+
+### CentOS 使用 `yum`
+
+- ~~小心 CentOS~~
+- 参考[CentOS Dockerfile](https://github.com/kumaraditya303/playwright-centos/blob/master/Dockerfile)
+- 添加中文字体库
+- ~~最佳解决办法~~
+  - 使用 Docker 然后用 Python 镜像 按照上面 Ubuntu 的写 `dockerfile`
+
+下面这个依赖运行一下 也许就可以用了
+
+```sh
+dnf install -y alsa-lib at-spi2-atk at-spi2-core atk cairo cups-libs dbus-libs expat flac-libs gdk-pixbuf2 glib2 glibc gtk3 libX11 libXcomposite libXdamage libXext libXfixes libXrandr libXtst libcanberra-gtk3 libdrm libgcc libstdc++ libxcb libxkbcommon libxshmfence libxslt mesa-libgbm nspr nss nss-util pango policycoreutils policycoreutils-python-utils zlib cairo-gobject centos-indexhtml dbus-glib fontconfig freetype gtk2 libXcursor libXi libXrender libXt liberation-fonts-common liberation-sans-fonts libffi mozilla-filesystem p11-kit-trust pipewire-libs harfbuzz-icu libglvnd-glx libglvnd-egl libnotify opus woff2 gstreamer1-plugins-base gstreamer1-plugins-bad-free openjpeg2 libwebp enchant libsecret hyphen libglvnd-gles
+```
```

