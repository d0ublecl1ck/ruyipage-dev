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
[Automation](https://0xshoulderlab.site/automation) / User Context
RuyiPage Docs
#  RuyiPage User Context
单独讲用户上下文，强调隔离运行和多环境实验。
## API 与参数说明
### page.browser_tools.get_user_contexts
`page.browser_tools.get_user_contexts()`
获取所有用户上下文列表
### page.browser_tools.create_user_context
`page.browser_tools.create_user_context()`
创建隔离的用户上下文
### page.browser_tools.remove_user_context
`page.browser_tools.remove_user_context(id)`
删除指定用户上下文
参数说明
参数 | 说明  
---|---  
id | 参数含义与默认值请结合当前 API 场景使用。  
### page.browser_tools.create_tab
`page.browser_tools.create_tab(user_context_id)`
在指定上下文中创建标签页
参数说明
参数 | 说明  
---|---  
user_context_id | 参数含义与默认值请结合当前 API 场景使用。  
## 相关示例
  * 参见示例中心：/automation/examples


## 相关示例源码
### Browser 模块：用户上下文与客户端窗口
examples/25_browser_user_context.py
Browser 模块最完整的 user context 与 client window 说明案例。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/25_browser_user_context.py) page.browser_tools.get_user_contextspage.browser_tools.create_user_contextpage.browser_tools.remove_user_contextpage.browser_tools.create_tabpage.browser_tools.get_client_windowspage.browser_tools.set_window_state
  * 读取 user context 列表
  * 创建与删除 user context
  * 在指定 user context 中创建新 tab
  * 读取 client window 列表
  * 切换窗口状态为 minimized / maximized / fullscreen


源码文件：`app/content/ruyipage_examples/25_browser_user_context.py` · 仓库：[25_browser_user_context.py](https://github.com/LoseNine/ruyipage/blob/main/examples/25_browser_user_context.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
#!/usr/bin/env python
# =============================
# RuyiPage 示例注释版
# 标题: Browser 模块：用户上下文与客户端窗口
# 说明: Browser 模块最完整的 user context 与 client window 说明案例。
# 你会学到:
#   1. 读取 user context 列表
#   2. 创建与删除 user context
#   3. 在指定 user context 中创建新 tab
#   4. 读取 client window 列表
#   5. 切换窗口状态为 minimized / maximized / fullscreen
# 相关 API: page.browser_tools.get_user_contexts, page.browser_tools.create_user_context, page.browser_tools.remove_user_context, page.browser_tools.create_tab, page.browser_tools.get_client_windows, page.browser_tools.set_window_state
# =============================

# -*- coding: utf-8 -*-
"""示例25: Browser 模块（用户上下文 + 客户端窗口）严格结果版"""

import io
import sys
import time
from typing import Dict, List

if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

from ruyipage import FirefoxPage


def add_result(
    results: List[Dict[str, str]], item: str, status: str, note: str
) -> None:
    """记录结构化结果。"""
    results.append({"item": item, "status": status, "note": note})


def print_results(results: List[Dict[str, str]]) -> None:
    """打印固定格式结果表。"""
    print("\n| 项目 | 状态 | 说明 |")
    print("| --- | --- | --- |")
    for row in results:
        print(f"| {row['item']} | {row['status']} | {row['note']} |")


def main() -> None:
    print("=" * 70)
    print("测试 25: Browser 用户上下文与窗口管理")
    print("=" * 70)

    page = FirefoxPage()
    results: List[Dict[str, str]] = []
    user_context_id = None
    new_tab_ctx = None

    try:
        page.get("https://www.example.com")

        # 1. user context 生命周期
        before = page.browser_tools.get_user_contexts()
        before_ids = [i.get("userContext") for i in before]
        add_result(
            results,
            "browser.getUserContexts before",
            "成功",
            f"创建前数量: {len(before)}",
        )

        user_context_id = page.browser_tools.create_user_context()
        if user_context_id:
            add_result(
                results,
                "browser.createUserContext",
                "成功",
                f"userContext={user_context_id}",
            )
        else:
            add_result(
                results, "browser.createUserContext", "失败", "未返回 userContext ID"
            )

        after_create = page.browser_tools.get_user_contexts()
        after_create_ids = [i.get("userContext") for i in after_create]
        if user_context_id in after_create_ids and len(after_create) == len(before) + 1:
            add_result(
                results,
                "browser.getUserContexts after create",
                "成功",
                f"数量变为 {len(after_create)}",
            )
        else:
            add_result(
                results,
                "browser.getUserContexts after create",
                "失败",
                "创建后数量或ID校验不通过",
            )

        if user_context_id:
            new_tab_ctx = page.browser_tools.create_tab(user_context=user_context_id)
            if new_tab_ctx:
                add_result(
                    results,
                    "browsingContext.create tab in user context",
                    "成功",
                    f"context={new_tab_ctx}",
                )
            else:
                add_result(
                    results,
                    "browsingContext.create tab in user context",
                    "失败",
                    "未返回新 tab context",
                )

        if new_tab_ctx:
            try:
                page.contexts.close(new_tab_ctx)
                add_result(
                    results, "browsingContext.close new tab", "成功", "新 tab 已关闭"
                )
                new_tab_ctx = None
            except Exception as e:
                add_result(
                    results, "browsingContext.close new tab", "跳过", str(e)[:120]
                )

        if user_context_id:
            page.browser_tools.remove_user_context(user_context_id)
            add_result(
                results,
                "browser.removeUserContext",
                "成功",
                f"已删除 {user_context_id}",
            )

            after_remove = page.browser_tools.get_user_contexts()
            after_remove_ids = [i.get("userContext") for i in after_remove]
            if user_context_id not in after_remove_ids and len(after_remove) == len(
                before_ids
            ):
                add_result(
                    results,
                    "browser.getUserContexts after remove",
                    "成功",
                    f"数量回到 {len(after_remove)}",
                )
            else:
                add_result(
                    results,
                    "browser.getUserContexts after remove",
                    "失败",
                    "删除后数量或ID校验不通过",
                )
            user_context_id = None

        # 2. client window 状态流
        windows = page.browser_tools.get_client_windows()
        if not windows:
            add_result(
                results, "browser.getClientWindows", "失败", "未返回任何 client window"
            )
        else:
            add_result(
                results, "browser.getClientWindows", "成功", f"窗口数量: {len(windows)}"
            )
            win = windows[0]
            win_id = win.get("clientWindow")
            states = ["minimized", "normal", "maximized", "fullscreen", "normal"]
            state_notes = []
            state_failed = False
            for state in states:
                page.browser_tools.set_window_state(win_id, state=state)
                time.sleep(0.4)
                current_windows = page.browser_tools.get_client_windows()
                current = current_windows[0] if current_windows else {}
                current_state = current.get("state")
                state_notes.append(f"{state}->{current_state}")
                if current_state != state:
                    state_failed = True

            if state_failed:
                add_result(
                    results,
                    "browser.setClientWindowState",
                    "失败",
                    ", ".join(state_notes),
                )
            else:
                add_result(
                    results,
                    "browser.setClientWindowState",
                    "成功",
                    ", ".join(state_notes),
                )

        print_results(results)

    except Exception as e:
        add_result(results, "示例执行", "失败", str(e)[:120])
        print_results(results)
        raise
    finally:
        if new_tab_ctx:
            try:
                page.contexts.close(new_tab_ctx)
            except Exception:
                pass
        if user_context_id:
            try:
                page.browser_tools.remove_user_context(user_context_id)
            except Exception:
                pass
        try:
            page.quit()
        except Exception:
            pass


if __name__ == "__main__":
    main()

```

```
#!/usr/bin/env python
# -*- coding: utf-8 -*-
"""示例25: Browser 模块（用户上下文 + 客户端窗口）严格结果版"""

import io
import sys
import time
from typing import Dict, List

if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

from ruyipage import FirefoxPage


def add_result(
    results: List[Dict[str, str]], item: str, status: str, note: str
) -> None:
    """记录结构化结果。"""
    results.append({"item": item, "status": status, "note": note})


def print_results(results: List[Dict[str, str]]) -> None:
    """打印固定格式结果表。"""
    print("\n| 项目 | 状态 | 说明 |")
    print("| --- | --- | --- |")
    for row in results:
        print(f"| {row['item']} | {row['status']} | {row['note']} |")


def main() -> None:
    print("=" * 70)
    print("测试 25: Browser 用户上下文与窗口管理")
    print("=" * 70)

    page = FirefoxPage()
    results: List[Dict[str, str]] = []
    user_context_id = None
    new_tab_ctx = None

    try:
        page.get("https://www.example.com")

        # 1. user context 生命周期
        before = page.browser_tools.get_user_contexts()
        before_ids = [i.get("userContext") for i in before]
        add_result(
            results,
            "browser.getUserContexts before",
            "成功",
            f"创建前数量: {len(before)}",
        )

        user_context_id = page.browser_tools.create_user_context()
        if user_context_id:
            add_result(
                results,
                "browser.createUserContext",
                "成功",
                f"userContext={user_context_id}",
            )
        else:
            add_result(
                results, "browser.createUserContext", "失败", "未返回 userContext ID"
            )

        after_create = page.browser_tools.get_user_contexts()
        after_create_ids = [i.get("userContext") for i in after_create]
        if user_context_id in after_create_ids and len(after_create) == len(before) + 1:
            add_result(
                results,
                "browser.getUserContexts after create",
                "成功",
                f"数量变为 {len(after_create)}",
            )
        else:
            add_result(
                results,
                "browser.getUserContexts after create",
                "失败",
                "创建后数量或ID校验不通过",
            )

        if user_context_id:
            new_tab_ctx = page.browser_tools.create_tab(user_context=user_context_id)
            if new_tab_ctx:
                add_result(
                    results,
                    "browsingContext.create tab in user context",
                    "成功",
                    f"context={new_tab_ctx}",
                )
            else:
                add_result(
                    results,
                    "browsingContext.create tab in user context",
                    "失败",
                    "未返回新 tab context",
                )

        if new_tab_ctx:
            try:
                page.contexts.close(new_tab_ctx)
                add_result(
                    results, "browsingContext.close new tab", "成功", "新 tab 已关闭"
                )
                new_tab_ctx = None
            except Exception as e:
                add_result(
                    results, "browsingContext.close new tab", "跳过", str(e)[:120]
                )

        if user_context_id:
            page.browser_tools.remove_user_context(user_context_id)
            add_result(
                results,
                "browser.removeUserContext",
                "成功",
                f"已删除 {user_context_id}",
            )

            after_remove = page.browser_tools.get_user_contexts()
            after_remove_ids = [i.get("userContext") for i in after_remove]
            if user_context_id not in after_remove_ids and len(after_remove) == len(
                before_ids
            ):
                add_result(
                    results,
                    "browser.getUserContexts after remove",
                    "成功",
                    f"数量回到 {len(after_remove)}",
                )
            else:
                add_result(
                    results,
                    "browser.getUserContexts after remove",
                    "失败",
                    "删除后数量或ID校验不通过",
                )
            user_context_id = None

        # 2. client window 状态流
        windows = page.browser_tools.get_client_windows()
        if not windows:
            add_result(
                results, "browser.getClientWindows", "失败", "未返回任何 client window"
            )
        else:
            add_result(
                results, "browser.getClientWindows", "成功", f"窗口数量: {len(windows)}"
            )
            win = windows[0]
            win_id = win.get("clientWindow")
            states = ["minimized", "normal", "maximized", "fullscreen", "normal"]
            state_notes = []
            state_failed = False
            for state in states:
                page.browser_tools.set_window_state(win_id, state=state)
                time.sleep(0.4)
                current_windows = page.browser_tools.get_client_windows()
                current = current_windows[0] if current_windows else {}
                current_state = current.get("state")
                state_notes.append(f"{state}->{current_state}")
                if current_state != state:
                    state_failed = True

            if state_failed:
                add_result(
                    results,
                    "browser.setClientWindowState",
                    "失败",
                    ", ".join(state_notes),
                )
            else:
                add_result(
                    results,
                    "browser.setClientWindowState",
                    "成功",
                    ", ".join(state_notes),
                )

        print_results(results)

    except Exception as e:
        add_result(results, "示例执行", "失败", str(e)[:120])
        print_results(results)
        raise
    finally:
        if new_tab_ctx:
            try:
                page.contexts.close(new_tab_ctx)
            except Exception:
                pass
        if user_context_id:
            try:
                page.browser_tools.remove_user_context(user_context_id)
            except Exception:
                pass
        try:
            page.quit()
        except Exception:
            pass


if __name__ == "__main__":
    main()

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
