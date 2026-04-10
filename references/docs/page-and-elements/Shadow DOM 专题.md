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
[Automation](https://0xshoulderlab.site/automation) / Shadow DOM 专题
RuyiPage Docs
#  RuyiPage Shadow DOM 专题
重点讲 open shadow 和 closed shadow 的区别，以及 with_shadow 的使用方式。
## API 与参数说明
### ele.with_shadow
`ele.with_shadow()`
进入元素的 shadow root（open 或 closed）
### shadow_root.ele
`shadow_root.ele(locator)`
在 shadow root 内查找元素
参数说明
参数 | 说明  
---|---  
locator | 定位表达式，支持 css/xpath/text/tag/属性组合。  
### page.with_frame
`page.with_frame(locator)`
配合 iframe 使用时切换上下文
参数说明
参数 | 说明  
---|---  
locator | 定位表达式，支持 css/xpath/text/tag/属性组合。  
### frame.ele
`frame.ele(locator)`
在 iframe 内查找元素
参数说明
参数 | 说明  
---|---  
locator | 定位表达式，支持 css/xpath/text/tag/属性组合。  
## 相关示例
  * 参见示例中心：/automation/examples


## 相关示例源码
### Shadow DOM 与嵌套 iframe：open / closed shadow 全场景
examples/14_shadow_dom.py
这是 shadow DOM 与复杂边界专题的主示例，必须在文档中单列。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/14_shadow_dom.py) ele.with_shadowshadow_root.elepage.with_frameframe.ele
  * 进入主页面 open shadow root
  * 进入主页面 closed shadow root
  * 在 iframe 内访问 open shadow
  * 在 iframe 内访问 closed shadow
  * 组合使用 with_frame 和 with_shadow
  * 处理复杂边界后恢复主页面上下文


源码文件：`app/content/ruyipage_examples/14_shadow_dom.py` · 仓库：[14_shadow_dom.py](https://github.com/LoseNine/ruyipage/blob/main/examples/14_shadow_dom.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
# =============================
# RuyiPage 示例注释版
# 标题: Shadow DOM 与嵌套 iframe：open / closed shadow 全场景
# 说明: 这是 shadow DOM 与复杂边界专题的主示例，必须在文档中单列。
# 你会学到:
#   1. 进入主页面 open shadow root
#   2. 进入主页面 closed shadow root
#   3. 在 iframe 内访问 open shadow
#   4. 在 iframe 内访问 closed shadow
#   5. 组合使用 with_frame 和 with_shadow
# 相关 API: ele.with_shadow, shadow_root.ele, page.with_frame, frame.ele
# =============================

# -*- coding: utf-8 -*-
"""示例14: Shadow DOM + 嵌套 iframe（open/closed 完整场景）

覆盖点：
1) 主页面 open shadow
2) 主页面 closed shadow（桥接函数）
3) 进入 iframe 后 open shadow
4) 进入 iframe 后 closed shadow（桥接函数）
5) with_frame / with_shadow 简洁 API
"""

import io
import os
import sys


if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")


sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))

from ruyipage import FirefoxOptions, FirefoxPage


def test_shadow_dom():
    print("=" * 60)
    print("测试14: Shadow DOM + 嵌套iframe")
    print("=" * 60)

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        test_page = os.path.join(
            os.path.dirname(__file__), "test_pages", "complex_shadow_iframe.html"
        )
        test_url = "file:///" + os.path.abspath(test_page).replace("\\", "/")
        page.get(test_url)
        page.wait(1)

        # 1) 主页面 open shadow
        print("\n1. 主页面 open shadow:")
        host_open = page.ele("#host-open-shadow")
        with host_open.with_shadow("open") as open_root:
            text = open_root.ele("#host-open-text").text
            print(f"   open文本: {text}")

        # 2) 主页面 closed shadow
        print("\n2. 主页面 closed shadow:")
        host_closed = page.ele("#host-closed-shadow")
        with host_closed.with_shadow("closed") as closed_root:
            text = closed_root.ele("#host-closed-text").text
            print(f"   closed文本: {text}")

        # 3) 进入 iframe，测试 open/closed shadow
        print("\n3. 进入iframe并测试 shadow:")
        with page.with_frame("#outer-iframe") as frame:
            inner_title = frame.ele("#inner-title").text
            print(f"   iframe标题: {inner_title}")

            inner_open = frame.ele("#inner-open-host")
            with inner_open.with_shadow("open") as inner_open_root:
                open_text = inner_open_root.ele("#inner-open-text").text
                print(f"   iframe open文本: {open_text}")

            inner_closed = frame.ele("#inner-closed-host")
            with inner_closed.with_shadow("closed") as inner_closed_root:
                closed_text = inner_closed_root.ele("#inner-closed-text").text
                print(f"   iframe closed文本: {closed_text}")

        # 4) 退出 with_frame 后仍可访问主页面
        print("\n4. 退出iframe后主页面可访问:")
        host_title = page.ele("#host-title").text
        print(f"   主页面标题: {host_title}")

        print("\n" + "=" * 60)
        print("✓ Shadow DOM + 嵌套iframe 测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(1)
        page.quit()


if __name__ == "__main__":
    test_shadow_dom()

```

```
# -*- coding: utf-8 -*-
"""示例14: Shadow DOM + 嵌套 iframe（open/closed 完整场景）

覆盖点：
1) 主页面 open shadow
2) 主页面 closed shadow（桥接函数）
3) 进入 iframe 后 open shadow
4) 进入 iframe 后 closed shadow（桥接函数）
5) with_frame / with_shadow 简洁 API
"""

import io
import os
import sys


if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")


sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))

from ruyipage import FirefoxOptions, FirefoxPage


def test_shadow_dom():
    print("=" * 60)
    print("测试14: Shadow DOM + 嵌套iframe")
    print("=" * 60)

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        test_page = os.path.join(
            os.path.dirname(__file__), "test_pages", "complex_shadow_iframe.html"
        )
        test_url = "file:///" + os.path.abspath(test_page).replace("\\", "/")
        page.get(test_url)
        page.wait(1)

        # 1) 主页面 open shadow
        print("\n1. 主页面 open shadow:")
        host_open = page.ele("#host-open-shadow")
        with host_open.with_shadow("open") as open_root:
            text = open_root.ele("#host-open-text").text
            print(f"   open文本: {text}")

        # 2) 主页面 closed shadow
        print("\n2. 主页面 closed shadow:")
        host_closed = page.ele("#host-closed-shadow")
        with host_closed.with_shadow("closed") as closed_root:
            text = closed_root.ele("#host-closed-text").text
            print(f"   closed文本: {text}")

        # 3) 进入 iframe，测试 open/closed shadow
        print("\n3. 进入iframe并测试 shadow:")
        with page.with_frame("#outer-iframe") as frame:
            inner_title = frame.ele("#inner-title").text
            print(f"   iframe标题: {inner_title}")

            inner_open = frame.ele("#inner-open-host")
            with inner_open.with_shadow("open") as inner_open_root:
                open_text = inner_open_root.ele("#inner-open-text").text
                print(f"   iframe open文本: {open_text}")

            inner_closed = frame.ele("#inner-closed-host")
            with inner_closed.with_shadow("closed") as inner_closed_root:
                closed_text = inner_closed_root.ele("#inner-closed-text").text
                print(f"   iframe closed文本: {closed_text}")

        # 4) 退出 with_frame 后仍可访问主页面
        print("\n4. 退出iframe后主页面可访问:")
        host_title = page.ele("#host-title").text
        print(f"   主页面标题: {host_title}")

        print("\n" + "=" * 60)
        print("✓ Shadow DOM + 嵌套iframe 测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(1)
        page.quit()


if __name__ == "__main__":
    test_shadow_dom()

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
