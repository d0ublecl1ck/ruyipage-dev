[ 小肩膀教育 ](https://0xshoulderlab.site/)
[首页](https://0xshoulderlab.site/) [实战课程](https://0xshoulderlab.site/courses) [公告](https://0xshoulderlab.site/news) [代理IP和爬虫数据](https://0xshoulderlab.site/proxy) [自动化框架](https://0xshoulderlab.site/automation) [招聘内推](https://0xshoulderlab.site/jobs) [指纹检测](https://0xshoulderlab.site/fingerprint) [关于我们](https://0xshoulderlab.site/about) [联系我们](https://0xshoulderlab.site/contact) [立即咨询](https://0xshoulderlab.site/contact)
[首页](https://0xshoulderlab.site/) [实战课程](https://0xshoulderlab.site/courses) [公告](https://0xshoulderlab.site/news) [代理IP和爬虫数据](https://0xshoulderlab.site/proxy) [自动化框架](https://0xshoulderlab.site/automation) [招聘内推](https://0xshoulderlab.site/jobs) [指纹检测](https://0xshoulderlab.site/fingerprint) [关于我们](https://0xshoulderlab.site/about) [联系我们](https://0xshoulderlab.site/contact) [立即咨询](https://0xshoulderlab.site/contact)
概览
[文档首页](https://0xshoulderlab.site/automation) [框架概览](https://0xshoulderlab.site/automation/overview)
快速开始
[安装](https://0xshoulderlab.site/automation/installation) [快速上手](https://0xshoulderlab.site/automation/quickstart)
基础能力
[页面对象](https://0xshoulderlab.site/automation/page) [页面导航](https://0xshoulderlab.site/automation/navigation) [等待机制](https://0xshoulderlab.site/automation/waits) [元素定位](https://0xshoulderlab.site/automation/elements) [选择器](https://0xshoulderlab.site/automation/selectors) [表单能力](https://0xshoulderlab.site/automation/forms)
输入与交互
[动作链](https://0xshoulderlab.site/automation/actions) [拖拽](https://0xshoulderlab.site/automation/drag-drop) [滚动](https://0xshoulderlab.site/automation/scrolling) [触摸输入](https://0xshoulderlab.site/automation/touch) [isTrusted](https://0xshoulderlab.site/automation/is-trusted)
页面结构
[iframe](https://0xshoulderlab.site/automation/iframe) [Shadow DOM](https://0xshoulderlab.site/automation/shadow-dom) [复杂边界](https://0xshoulderlab.site/automation/page-structure/complex-boundaries)
脚本与调试
[JavaScript](https://0xshoulderlab.site/automation/javascript) [Script 模块](https://0xshoulderlab.site/automation/script) [Preload Script](https://0xshoulderlab.site/automation/preload-scripts) [Console](https://0xshoulderlab.site/automation/console)
浏览器能力
[Cookies](https://0xshoulderlab.site/automation/cookies) [标签页](https://0xshoulderlab.site/automation/tabs) [窗口](https://0xshoulderlab.site/automation/window) [Browser 模块](https://0xshoulderlab.site/automation/browser) [User Context](https://0xshoulderlab.site/automation/user-contexts) [Browsing Context](https://0xshoulderlab.site/automation/browsing-context) [下载](https://0xshoulderlab.site/automation/downloads) [截图](https://0xshoulderlab.site/automation/screenshots) [PDF](https://0xshoulderlab.site/automation/pdf) [弹窗](https://0xshoulderlab.site/automation/prompts) [WebExtension](https://0xshoulderlab.site/automation/extensions)
网络与事件
[网络能力](https://0xshoulderlab.site/automation/network) [请求拦截](https://0xshoulderlab.site/automation/intercept) [网络事件](https://0xshoulderlab.site/automation/network-events) [导航事件](https://0xshoulderlab.site/automation/navigation-events) [Data Collector](https://0xshoulderlab.site/automation/data-collector) [认证](https://0xshoulderlab.site/automation/auth)
仿真与高风控
[Emulation](https://0xshoulderlab.site/automation/emulation) [移动端](https://0xshoulderlab.site/automation/mobile) [高风控场景](https://0xshoulderlab.site/automation/anti-bot)
规范与工具
[BiDi 对照](https://0xshoulderlab.site/automation/bidi) [测试工具](https://0xshoulderlab.site/automation/testing)
示例中心
[全部示例](https://0xshoulderlab.site/automation/examples)
[Automation](https://0xshoulderlab.site/automation) / Cookies
RuyiPage Docs
#  RuyiPage Cookies
Cookie 是会话和登录态管理的核心，这里讲读取、设置、过滤和删除。
## API 与参数说明
### page.get_cookies
`page.get_cookies()`
获取当前页面所有 Cookie
### page.set_cookies
`page.set_cookies(cookies)`
设置 Cookie（列表或单个）
参数说明
参数 | 说明  
---|---  
cookies | Cookie 对象或列表。  
### page.get_cookies_filtered
`page.get_cookies_filtered(**kwargs)`
按条件过滤 Cookie
参数说明
参数 | 说明  
---|---  
**kwargs | 参数含义与默认值请结合当前 API 场景使用。  
### page.delete_cookies
`page.delete_cookies(name)`
删除指定名称的 Cookie
参数说明
参数 | 说明  
---|---  
name | 名称参数（如 cookie 名称）。  
### page.browser.cookies
`page.browser.cookies`
浏览器级 Cookie 视图
## 相关示例
  * 参见示例中心：/automation/examples


## 相关示例源码
### Cookie 管理：读取、设置、过滤、删除
examples/08_cookies.py
围绕登录态和会话管理的核心示例。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/08_cookies.py) page.get_cookiespage.set_cookiespage.get_cookies_filteredpage.delete_cookiespage.browser.cookies
  * 读取服务端下发 Cookie
  * 通过 API 设置 Cookie
  * 按 name 等条件过滤 Cookie
  * 删除指定 Cookie 或清空全部 Cookie
  * 读取浏览器级 Cookie 视图


源码文件：`app/content/ruyipage_examples/08_cookies.py` · 仓库：[08_cookies.py](https://github.com/LoseNine/ruyipage/blob/main/examples/08_cookies.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
# =============================
# RuyiPage 示例注释版
# 标题: Cookie 管理：读取、设置、过滤、删除
# 说明: 围绕登录态和会话管理的核心示例。
# 你会学到:
#   1. 读取服务端下发 Cookie
#   2. 通过 API 设置 Cookie
#   3. 按 name 等条件过滤 Cookie
#   4. 删除指定 Cookie 或清空全部 Cookie
#   5. 读取浏览器级 Cookie 视图
# 相关 API: page.get_cookies, page.set_cookies, page.get_cookies_filtered, page.delete_cookies, page.browser.cookies
# =============================

# -*- coding: utf-8 -*-
"""
示例8: Cookie管理
测试功能：
- 获取Cookie
- 设置Cookie
- 删除Cookie
- 清空所有Cookie
"""

import os
import sys
import io
import time

# 设置控制台输出编码为UTF-8（Windows兼容）
if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))
sys.path.insert(0, os.path.dirname(__file__))

from ruyipage import FirefoxPage, FirefoxOptions
from test_server import TestServer


def test_cookies():
    """测试Cookie管理功能"""
    print("=" * 60)
    print("测试8: Cookie管理")
    print("=" * 60)

    # 启动测试服务器
    server = TestServer(port=8888)
    server.start()

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        # 访问测试服务器的Cookie设置页面
        print("\n访问测试服务器...")
        page.get(server.get_url("/set-cookie"))
        page.wait(2)

        # 1. 获取服务器设置的Cookie
        print("\n1. 获取服务器设置的Cookie:")
        all_cookies = page.get_cookies(all_info=True)
        print(f"   共有 {len(all_cookies)} 个Cookie")
        for cookie in all_cookies:
            name = cookie.name
            value = cookie.value
            print(f"   - {name}: {value}")

        # 2. 通过API设置Cookie
        print("\n2. 通过API设置Cookie:")
        page.set_cookies(
            {
                "name": "api_cookie",
                "value": "api_value",
                "domain": "127.0.0.1",
                "path": "/",
            }
        )
        page.set_cookies(
            {"name": "user_id", "value": "12345", "domain": "127.0.0.1", "path": "/"}
        )
        print(f"   ✓ 已通过API设置2个Cookie")

        # 3. 验证Cookie已设置
        print("\n3. 验证Cookie已设置:")
        page.refresh()
        page.wait(1)
        all_cookies = page.get_cookies(all_info=True)
        print(f"   刷新后共有 {len(all_cookies)} 个Cookie")

        # 转换为字典方便查找
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "api_cookie" in cookies_dict:
            print(f"   ✓ api_cookie = {cookies_dict['api_cookie']}")
        if "user_id" in cookies_dict:
            print(f"   ✓ user_id = {cookies_dict['user_id']}")

        # 4. 设置带过期时间的Cookie
        print("\n4. 设置带过期时间的Cookie:")
        expire_time = int(time.time()) + 3600  # 1小时后过期
        page.set_cookies(
            {
                "name": "expire_cookie",
                "value": "will_expire",
                "domain": "127.0.0.1",
                "path": "/",
                "expiry": expire_time,
            }
        )
        print(f"   ✓ 已设置带过期时间的Cookie（1小时后过期）")

        # 5. 设置HttpOnly和Secure Cookie
        print("\n5. 设置HttpOnly和Secure Cookie:")
        page.set_cookies(
            {
                "name": "secure_cookie",
                "value": "secure_value",
                "domain": "127.0.0.1",
                "path": "/",
                "httpOnly": True,
                "secure": False,  # HTTP不能用secure=True
            }
        )
        print(f"   ✓ 已设置HttpOnly Cookie")

        # 6. 获取特定Cookie
        print("\n6. 获取特定Cookie:")
        all_cookies = page.get_cookies(all_info=True)
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "user_id" in cookies_dict:
            print(f"   user_id = {cookies_dict['user_id']}")
        if "expire_cookie" in cookies_dict:
            print(f"   expire_cookie = {cookies_dict['expire_cookie']}")

        # 6.1 简单 cookies 属性
        print("\n6.1 当前页面 cookies 属性:")
        simple_cookies = page.cookies
        print(f"   page.cookies 数量: {len(simple_cookies)}")

        # 6.2 setter 风格 Cookie API
        print("\n6.2 通过 page.set.cookies 设置Cookie:")
        page.set.cookies(
            {
                "name": "setter_cookie",
                "value": "setter_value",
                "domain": "127.0.0.1",
                "path": "/",
            }
        )
        page.wait(0.5)
        setter_cookies = {c.name: c.value for c in page.get_cookies()}
        print(f"   setter_cookie = {setter_cookies.get('setter_cookie')}")

        # 6.3 通过高层过滤 API 读取 Cookie
        print("\n6.3 通过高层过滤 API 读取Cookie:")
        filtered_cookies = page.get_cookies_filtered(name="user_id", all_info=True)
        print(f"   过滤结果数量: {len(filtered_cookies)}")
        if filtered_cookies:
            value = filtered_cookies[0].value
            print(f"   user_id(filtered) = {value}")

        # 7. 删除特定Cookie
        print("\n7. 删除特定Cookie:")
        page.delete_cookies(name="api_cookie")
        print(f"   ✓ 已删除 api_cookie")

        # 验证删除
        page.wait(0.5)
        all_cookies = page.get_cookies(all_info=True)
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "api_cookie" not in cookies_dict:
            print(f"   ✓ 确认 api_cookie 已被删除")
        else:
            print(f"   ⚠ api_cookie 仍然存在")

        # 7.1 通过公开删除接口删除 setter_cookie
        print("\n7.1 删除 setter_cookie:")
        page.delete_cookies(name="setter_cookie", domain="127.0.0.1")
        page.wait(0.5)
        cookies_after_remove = {c.name: c.value for c in page.get_cookies()}
        print(f"   setter_cookie 是否存在: {'setter_cookie' in cookies_after_remove}")

        # 8. 访问API验证Cookie发送
        print("\n8. 访问API验证Cookie发送:")
        page.get(server.get_url("/get-cookie"))
        page.wait(1)
        body_text = page.ele("tag:body").text
        print(f"   服务器收到的Cookie: {body_text[:100]}")

        # 9. 清空所有Cookie
        print("\n9. 清空所有Cookie:")
        page.delete_cookies()
        print(f"   ✓ 已清空所有Cookie")

        # 验证清空
        all_cookies = page.get_cookies()
        print(f"   清空后Cookie数量: {len(all_cookies)}")

        # 9.1 浏览器级 Cookie 读取
        print("\n9.1 浏览器级 cookies 读取:")
        browser_cookies = page.browser.cookies(all_info=False)
        print(f"   browser.cookies 数量: {len(browser_cookies)}")

        # 10. 重新设置并测试
        print("\n10. 重新设置Cookie并测试:")
        page.set_cookies(
            {
                "name": "final_cookie",
                "value": "final_value",
                "domain": "127.0.0.1",
                "path": "/",
            }
        )
        page.refresh()
        page.wait(1)

        all_cookies = page.get_cookies(all_info=True)
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "final_cookie" in cookies_dict:
            print(f"   ✓ final_cookie = {cookies_dict['final_cookie']}")
            print(f"   ✓ Cookie持久性测试通过")

        print("\n" + "=" * 60)
        print("✓ 所有Cookie管理测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(2)
        page.quit()
        server.stop()


if __name__ == "__main__":
    test_cookies()

```

```
# -*- coding: utf-8 -*-
"""
示例8: Cookie管理
测试功能：
- 获取Cookie
- 设置Cookie
- 删除Cookie
- 清空所有Cookie
"""

import os
import sys
import io
import time

# 设置控制台输出编码为UTF-8（Windows兼容）
if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))
sys.path.insert(0, os.path.dirname(__file__))

from ruyipage import FirefoxPage, FirefoxOptions
from test_server import TestServer


def test_cookies():
    """测试Cookie管理功能"""
    print("=" * 60)
    print("测试8: Cookie管理")
    print("=" * 60)

    # 启动测试服务器
    server = TestServer(port=8888)
    server.start()

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        # 访问测试服务器的Cookie设置页面
        print("\n访问测试服务器...")
        page.get(server.get_url("/set-cookie"))
        page.wait(2)

        # 1. 获取服务器设置的Cookie
        print("\n1. 获取服务器设置的Cookie:")
        all_cookies = page.get_cookies(all_info=True)
        print(f"   共有 {len(all_cookies)} 个Cookie")
        for cookie in all_cookies:
            name = cookie.name
            value = cookie.value
            print(f"   - {name}: {value}")

        # 2. 通过API设置Cookie
        print("\n2. 通过API设置Cookie:")
        page.set_cookies(
            {
                "name": "api_cookie",
                "value": "api_value",
                "domain": "127.0.0.1",
                "path": "/",
            }
        )
        page.set_cookies(
            {"name": "user_id", "value": "12345", "domain": "127.0.0.1", "path": "/"}
        )
        print(f"   ✓ 已通过API设置2个Cookie")

        # 3. 验证Cookie已设置
        print("\n3. 验证Cookie已设置:")
        page.refresh()
        page.wait(1)
        all_cookies = page.get_cookies(all_info=True)
        print(f"   刷新后共有 {len(all_cookies)} 个Cookie")

        # 转换为字典方便查找
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "api_cookie" in cookies_dict:
            print(f"   ✓ api_cookie = {cookies_dict['api_cookie']}")
        if "user_id" in cookies_dict:
            print(f"   ✓ user_id = {cookies_dict['user_id']}")

        # 4. 设置带过期时间的Cookie
        print("\n4. 设置带过期时间的Cookie:")
        expire_time = int(time.time()) + 3600  # 1小时后过期
        page.set_cookies(
            {
                "name": "expire_cookie",
                "value": "will_expire",
                "domain": "127.0.0.1",
                "path": "/",
                "expiry": expire_time,
            }
        )
        print(f"   ✓ 已设置带过期时间的Cookie（1小时后过期）")

        # 5. 设置HttpOnly和Secure Cookie
        print("\n5. 设置HttpOnly和Secure Cookie:")
        page.set_cookies(
            {
                "name": "secure_cookie",
                "value": "secure_value",
                "domain": "127.0.0.1",
                "path": "/",
                "httpOnly": True,
                "secure": False,  # HTTP不能用secure=True
            }
        )
        print(f"   ✓ 已设置HttpOnly Cookie")

        # 6. 获取特定Cookie
        print("\n6. 获取特定Cookie:")
        all_cookies = page.get_cookies(all_info=True)
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "user_id" in cookies_dict:
            print(f"   user_id = {cookies_dict['user_id']}")
        if "expire_cookie" in cookies_dict:
            print(f"   expire_cookie = {cookies_dict['expire_cookie']}")

        # 6.1 简单 cookies 属性
        print("\n6.1 当前页面 cookies 属性:")
        simple_cookies = page.cookies
        print(f"   page.cookies 数量: {len(simple_cookies)}")

        # 6.2 setter 风格 Cookie API
        print("\n6.2 通过 page.set.cookies 设置Cookie:")
        page.set.cookies(
            {
                "name": "setter_cookie",
                "value": "setter_value",
                "domain": "127.0.0.1",
                "path": "/",
            }
        )
        page.wait(0.5)
        setter_cookies = {c.name: c.value for c in page.get_cookies()}
        print(f"   setter_cookie = {setter_cookies.get('setter_cookie')}")

        # 6.3 通过高层过滤 API 读取 Cookie
        print("\n6.3 通过高层过滤 API 读取Cookie:")
        filtered_cookies = page.get_cookies_filtered(name="user_id", all_info=True)
        print(f"   过滤结果数量: {len(filtered_cookies)}")
        if filtered_cookies:
            value = filtered_cookies[0].value
            print(f"   user_id(filtered) = {value}")

        # 7. 删除特定Cookie
        print("\n7. 删除特定Cookie:")
        page.delete_cookies(name="api_cookie")
        print(f"   ✓ 已删除 api_cookie")

        # 验证删除
        page.wait(0.5)
        all_cookies = page.get_cookies(all_info=True)
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "api_cookie" not in cookies_dict:
            print(f"   ✓ 确认 api_cookie 已被删除")
        else:
            print(f"   ⚠ api_cookie 仍然存在")

        # 7.1 通过公开删除接口删除 setter_cookie
        print("\n7.1 删除 setter_cookie:")
        page.delete_cookies(name="setter_cookie", domain="127.0.0.1")
        page.wait(0.5)
        cookies_after_remove = {c.name: c.value for c in page.get_cookies()}
        print(f"   setter_cookie 是否存在: {'setter_cookie' in cookies_after_remove}")

        # 8. 访问API验证Cookie发送
        print("\n8. 访问API验证Cookie发送:")
        page.get(server.get_url("/get-cookie"))
        page.wait(1)
        body_text = page.ele("tag:body").text
        print(f"   服务器收到的Cookie: {body_text[:100]}")

        # 9. 清空所有Cookie
        print("\n9. 清空所有Cookie:")
        page.delete_cookies()
        print(f"   ✓ 已清空所有Cookie")

        # 验证清空
        all_cookies = page.get_cookies()
        print(f"   清空后Cookie数量: {len(all_cookies)}")

        # 9.1 浏览器级 Cookie 读取
        print("\n9.1 浏览器级 cookies 读取:")
        browser_cookies = page.browser.cookies(all_info=False)
        print(f"   browser.cookies 数量: {len(browser_cookies)}")

        # 10. 重新设置并测试
        print("\n10. 重新设置Cookie并测试:")
        page.set_cookies(
            {
                "name": "final_cookie",
                "value": "final_value",
                "domain": "127.0.0.1",
                "path": "/",
            }
        )
        page.refresh()
        page.wait(1)

        all_cookies = page.get_cookies(all_info=True)
        cookies_dict = {}
        for c in all_cookies:
            cookies_dict[c.name] = c.value

        if "final_cookie" in cookies_dict:
            print(f"   ✓ final_cookie = {cookies_dict['final_cookie']}")
            print(f"   ✓ Cookie持久性测试通过")

        print("\n" + "=" * 60)
        print("✓ 所有Cookie管理测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(2)
        page.quit()
        server.stop()


if __name__ == "__main__":
    test_cookies()

```

### Cloudflare / Copilot 快速开始
quickstart_cloudfare.py
面向高风控站点的快速开始示例，覆盖挑战处理、输入框识别和 Cookie 提取。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/quickstart_cloudfare.py) FirefoxOptionsFirefoxPagepage.getpage.elepage.handle_cloudflare_challengepage.get_cookies
  * 访问高风控站点并等待页面完成首屏加载
  * 自动尝试处理 Cloudflare 挑战
  * 定位输入框并发送问题
  * 提取 document.cookie 与完整 Cookie 信息


源码文件：`app/content/ruyipage_examples/quickstart_cloudfare.py` · 仓库：[quickstart_cloudfare.py](https://github.com/LoseNine/ruyipage/blob/main/examples/quickstart_cloudfare.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
# =============================
# RuyiPage 示例注释版
# 标题: Cloudflare / Copilot 快速开始
# 说明: 面向高风控站点的快速开始示例，覆盖挑战处理、输入框识别和 Cookie 提取。
# 你会学到:
#   1. 访问高风控站点并等待页面完成首屏加载
#   2. 自动尝试处理 Cloudflare 挑战
#   3. 定位输入框并发送问题
#   4. 提取 document.cookie 与完整 Cookie 信息
# 相关 API: FirefoxOptions, FirefoxPage, page.get, page.ele, page.handle_cloudflare_challenge, page.get_cookies
# =============================

# -*- coding: utf-8 -*-
"""快速开始：访问 Copilot，自动尝试通过 Cloudflare，并打印完整 Cookie。"""

from ruyipage import FirefoxOptions, FirefoxPage, Keys


QUESTION = "你好，今天天气怎么样？"


def find_input_box(page: FirefoxPage):
    for _ in range(30):
        box = page.ele("css:textarea")
        if not box:
            box = page.ele('css:[contenteditable="true"]')
        if not box:
            box = page.ele("css:.input-area")
        if box:
            return box
        page.wait(1)
    return None


def print_full_cookies(page: FirefoxPage) -> None:
    print("\n" + "=" * 60)
    print("Cloudflare / 页面 Cookie")
    print("=" * 60)

    raw_cookie = page.run_js("return document.cookie") or ""
    print(f"document.cookie: {raw_cookie}")

    cookies = page.get_cookies(all_info=True)
    print(f"Cookie 数量: {len(cookies)}")
    for i, cookie in enumerate(cookies, 1):
        print(f"[{i}] name={cookie.name}")
        print(f"    value={cookie.value}")
        print(f"    domain={cookie.domain}")
        print(f"    path={cookie.path}")
        print(f"    httpOnly={cookie.http_only}")
        print(f"    secure={cookie.secure}")
        print(f"    sameSite={cookie.same_site}")
        print(f"    expiry={cookie.expiry}")


opts = FirefoxOptions()
# 如果 Firefox 不在默认安装目录，可以取消注释并指定路径。
# opts.set_browser_path(r"D:\Firefox\firefox.exe")

# 如果你想复用登录状态、Cookie、扩展，可以取消注释并指定 userdir。
# opts.set_user_dir(r"D:\ruyipage_userdir")

page = FirefoxPage(opts)

try:
    print("=" * 60)
    print("copilot.microsoft.com Cloudflare 测试")
    print("=" * 60)

    print("\n-> 访问 https://copilot.microsoft.com/ ...")
    page.get("https://copilot.microsoft.com/", wait="none")
    page.wait(5)

    print("-> 等待输入框...")
    input_box = find_input_box(page)

    if input_box:
        print("-> 找到输入框，开始输入问题...")
        try:
            input_box.click()
            page.wait(0.8)
            input_box.input(QUESTION, clear=True)
            page.wait(0.8)

            send_btn = page.ele('css:button[aria-label*="Send"]')
            if not send_btn:
                send_btn = page.ele('css:button[type="submit"]')

            if send_btn:
                print("-> 点击发送按钮...")
                send_btn.click()
            else:
                print("-> 按 Enter 发送...")
                page.actions.press(Keys.ENTER).perform()

            print("-> 已发送问题，等待 Cloudflare 触发...")
            page.wait(15)
        except Exception as e:
            print(f"-> 发送失败: {e}")
            page.wait(5)
    else:
        print("-> 未找到输入框，直接等待 Cloudflare...")
        page.wait(5)

    print("\n-> 开始自动处理 Cloudflare...")
    passed = page.handle_cloudflare_challenge(timeout=120, check_interval=2)

    print("\n" + "=" * 60)
    if passed:
        print("✅ 成功通过 Cloudflare！")
        print_full_cookies(page)
    else:
        print("❌ 超时未通过")

    print("\n[+] 保持浏览器打开 500 秒...")
    page.wait(500)

finally:
    page.quit()

```

```
# -*- coding: utf-8 -*-
"""快速开始：访问 Copilot，自动尝试通过 Cloudflare，并打印完整 Cookie。"""

from ruyipage import FirefoxOptions, FirefoxPage, Keys


QUESTION = "你好，今天天气怎么样？"


def find_input_box(page: FirefoxPage):
    for _ in range(30):
        box = page.ele("css:textarea")
        if not box:
            box = page.ele('css:[contenteditable="true"]')
        if not box:
            box = page.ele("css:.input-area")
        if box:
            return box
        page.wait(1)
    return None


def print_full_cookies(page: FirefoxPage) -> None:
    print("\n" + "=" * 60)
    print("Cloudflare / 页面 Cookie")
    print("=" * 60)

    raw_cookie = page.run_js("return document.cookie") or ""
    print(f"document.cookie: {raw_cookie}")

    cookies = page.get_cookies(all_info=True)
    print(f"Cookie 数量: {len(cookies)}")
    for i, cookie in enumerate(cookies, 1):
        print(f"[{i}] name={cookie.name}")
        print(f"    value={cookie.value}")
        print(f"    domain={cookie.domain}")
        print(f"    path={cookie.path}")
        print(f"    httpOnly={cookie.http_only}")
        print(f"    secure={cookie.secure}")
        print(f"    sameSite={cookie.same_site}")
        print(f"    expiry={cookie.expiry}")


opts = FirefoxOptions()
# 如果 Firefox 不在默认安装目录，可以取消注释并指定路径。
# opts.set_browser_path(r"D:\Firefox\firefox.exe")

# 如果你想复用登录状态、Cookie、扩展，可以取消注释并指定 userdir。
# opts.set_user_dir(r"D:\ruyipage_userdir")

page = FirefoxPage(opts)

try:
    print("=" * 60)
    print("copilot.microsoft.com Cloudflare 测试")
    print("=" * 60)

    print("\n-> 访问 https://copilot.microsoft.com/ ...")
    page.get("https://copilot.microsoft.com/", wait="none")
    page.wait(5)

    print("-> 等待输入框...")
    input_box = find_input_box(page)

    if input_box:
        print("-> 找到输入框，开始输入问题...")
        try:
            input_box.click()
            page.wait(0.8)
            input_box.input(QUESTION, clear=True)
            page.wait(0.8)

            send_btn = page.ele('css:button[aria-label*="Send"]')
            if not send_btn:
                send_btn = page.ele('css:button[type="submit"]')

            if send_btn:
                print("-> 点击发送按钮...")
                send_btn.click()
            else:
                print("-> 按 Enter 发送...")
                page.actions.press(Keys.ENTER).perform()

            print("-> 已发送问题，等待 Cloudflare 触发...")
            page.wait(15)
        except Exception as e:
            print(f"-> 发送失败: {e}")
            page.wait(5)
    else:
        print("-> 未找到输入框，直接等待 Cloudflare...")
        page.wait(5)

    print("\n-> 开始自动处理 Cloudflare...")
    passed = page.handle_cloudflare_challenge(timeout=120, check_interval=2)

    print("\n" + "=" * 60)
    if passed:
        print("✅ 成功通过 Cloudflare！")
        print_full_cookies(page)
    else:
        print("❌ 超时未通过")

    print("\n[+] 保持浏览器打开 500 秒...")
    page.wait(500)

finally:
    page.quit()

```

#### 小肩膀教育
专注逆向工程与安全开发，实战驱动教学，帮助有志向的年轻人通过努力学习获得体面工作。
#### 课程方向
  * [网络爬虫](https://0xshoulderlab.site/courses?category=crawler)
  * [安卓逆向](https://0xshoulderlab.site/courses?category=android-reverse)
  * [iOS逆向](https://0xshoulderlab.site/courses?category=ios-reverse)
  * [AI逆向](https://0xshoulderlab.site/courses?category=ai-reverse)
  * [浏览器内核开发](https://0xshoulderlab.site/courses?category=browser-kernel)
  * [自动化框架](https://0xshoulderlab.site/automation)


#### 快速链接
  * [关于我们](https://0xshoulderlab.site/about)
  * [联系我们](https://0xshoulderlab.site/contact)
  * [B站·小肩膀教育](https://space.bilibili.com/534838862)
  * [B站·如意浏览器开发](https://space.bilibili.com/172381477)


#### 联系方式
  * 微信：xiaojianbang8888
  * 微信：Charleval
  * 公众号：非攻Code / 如意私塾


© 2016-2026 小肩膀教育 保留所有权利 · 十年专注逆向安全培训 
