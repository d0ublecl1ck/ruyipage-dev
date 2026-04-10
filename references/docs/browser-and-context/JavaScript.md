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
[Automation](https://0xshoulderlab.site/automation) / JavaScript
RuyiPage Docs
#  RuyiPage JavaScript
run_js、参数传递、DOM 修改和脚本注入是调试和增强页面控制的重要补充。
## API 与参数说明
### page.run_js
`page.run_js(script, *args)`
在页面执行 JavaScript，支持传参
参数说明
参数 | 说明  
---|---  
script | 参数含义与默认值请结合当前 API 场景使用。  
*args | 参数含义与默认值请结合当前 API 场景使用。  
### ele.run_js
`ele.run_js(script, *args)`
在元素上下文执行 JavaScript
参数说明
参数 | 说明  
---|---  
script | 参数含义与默认值请结合当前 API 场景使用。  
*args | 参数含义与默认值请结合当前 API 场景使用。  
### page.get_realms
`page.get_realms()`
获取所有 JavaScript realm
### page.eval_handle
`page.eval_handle(script)`
执行脚本并返回远程对象句柄
参数说明
参数 | 说明  
---|---  
script | 参数含义与默认值请结合当前 API 场景使用。  
### page.add_preload_script
`page.add_preload_script(script)`
注入 preload script（页面加载前执行）
参数说明
参数 | 说明  
---|---  
script | 参数含义与默认值请结合当前 API 场景使用。  
### page.remove_preload_script
`page.remove_preload_script(script_id)`
移除已注入的 preload script
参数说明
参数 | 说明  
---|---  
script_id | 参数含义与默认值请结合当前 API 场景使用。  
## 相关示例
  * 参见示例中心：/automation/examples


## 相关示例源码
### JavaScript 执行与脚本能力
examples/07_javascript.py
展示 run_js、参数传递、DOM 修改和 preload script 的调试价值。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/07_javascript.py) page.run_jsele.run_jspage.get_realmspage.eval_handlepage.add_preload_scriptpage.remove_preload_script
  * 执行表达式并获取返回值
  * 向脚本传参
  * 直接修改 DOM 内容
  * 在元素上下文执行 JS
  * 读取 realms 并注入 preload script


源码文件：`app/content/ruyipage_examples/07_javascript.py` · 仓库：[07_javascript.py](https://github.com/LoseNine/ruyipage/blob/main/examples/07_javascript.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
# =============================
# RuyiPage 示例注释版
# 标题: JavaScript 执行与脚本能力
# 说明: 展示 run_js、参数传递、DOM 修改和 preload script 的调试价值。
# 你会学到:
#   1. 执行表达式并获取返回值
#   2. 向脚本传参
#   3. 直接修改 DOM 内容
#   4. 在元素上下文执行 JS
#   5. 读取 realms 并注入 preload script
# 相关 API: page.run_js, ele.run_js, page.get_realms, page.eval_handle, page.add_preload_script, page.remove_preload_script
# =============================

# -*- coding: utf-8 -*-
"""
示例7: JavaScript执行
测试功能：
- 执行JavaScript代码
- 获取返回值
- 传递参数
- 在元素上执行JS
- 修改页面内容
"""

import os
import sys
import io

# 设置控制台输出编码为UTF-8（Windows兼容）
if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))

from ruyipage import FirefoxPage, FirefoxOptions


def test_javascript():
    """测试JavaScript执行功能"""
    print("=" * 60)
    print("测试7: JavaScript执行")
    print("=" * 60)

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        # 加载测试页面
        test_page = os.path.join(
            os.path.dirname(__file__), "test_pages", "test_page.html"
        )
        test_url = "file:///" + os.path.abspath(test_page).replace("\\", "/")
        page.get(test_url)
        page.wait(1)

        # 1. 执行简单的JavaScript
        print("\n1. 执行简单的JavaScript:")
        result = page.run_js("return 1 + 2")
        print(f"   1 + 2 = {result}")

        # 2. 获取页面信息
        print("\n2. 获取页面信息:")
        title = page.run_js("return document.title")
        print(f"   页面标题: {title}")

        url = page.run_js("return window.location.href")
        print(f"   页面URL: {url}")

        # 3. 修改页面内容
        print("\n3. 修改页面内容:")
        page.run_js(
            'document.getElementById("main-title").textContent = "标题已被JS修改"'
        )
        new_title = page.ele("#main-title").text
        print(f"   修改后的标题: {new_title}")

        # 4. 传递参数
        print("\n4. 传递参数到JavaScript:")
        result = page.run_js("return arguments[0] + arguments[1]", 10, 20)
        print(f"   10 + 20 = {result}")

        # 5. 在元素上执行JavaScript
        print("\n5. 在元素上执行JavaScript:")
        btn = page.ele("#click-btn")
        btn_text = btn.run_js("function() { return this.textContent; }")
        print(f"   按钮文本: {btn_text}")

        # 修改元素样式
        btn.run_js(
            'function() { this.style.background = "red"; this.style.color = "white"; }'
        )
        page.wait(0.5)
        print(f"   ✓ 按钮样式已修改")

        # 6. 获取元素属性
        print("\n6. 通过JS获取元素属性:")
        input_elem = page.ele("#text-input")
        placeholder = input_elem.run_js("function() { return this.placeholder; }")
        print(f"   输入框placeholder: {placeholder}")

        # 7. 执行复杂的JavaScript
        print("\n7. 执行复杂的JavaScript:")
        result = page.run_js("""
            (() => {
                const elements = document.querySelectorAll('.test-class');
                return Array.from(elements).map(el => el.textContent);
            })()
        """)
        print(f"   所有.test-class元素的文本: {result}")

        # 8. 修改输入框的值
        print("\n8. 通过JS修改输入框:")
        page.run_js("document.getElementById('text-input').value = 'JS设置的值'")
        value = page.ele("#text-input").value
        print(f"   输入框的值: {value}")

        # 9. 通过JS触发事件
        print("\n9. 通过JS触发事件:")
        page.run_js('document.getElementById("click-btn").click()')
        page.wait(0.5)
        result = page.ele("#click-result").text
        print(f"   点击结果: {result}")

        # 10. 获取计算样式
        print("\n10. 获取元素的计算样式:")
        color = page.run_js("""
            (() => {
                const elem = document.getElementById('click-btn');
                return window.getComputedStyle(elem).backgroundColor;
            })()
        """)
        print(f"   按钮背景色: {color}")

        # 11. 滚动到元素
        print("\n11. 通过JS滚动到元素:")
        page.run_js('document.getElementById("scroll-section").scrollIntoView()')
        page.wait(0.5)
        print(f"   ✓ 已滚动到滚动测试区域")

        # 12. 创建新元素
        print("\n12. 通过JS创建新元素:")
        page.run_js("""
            const div = document.createElement('div');
            div.id = 'js-created';
            div.textContent = 'JavaScript创建的元素';
            div.style.padding = '10px';
            div.style.background = '#ffeb3b';
            document.body.appendChild(div);
        """)
        page.wait(0.5)
        new_elem = page.ele("#js-created")
        print(f"   新元素文本: {new_elem.text}")

        # 13. 在 sandbox 中执行脚本
        print("\n13. 在sandbox中执行JavaScript:")
        sandbox_value = page.run_js(
            """
            globalThis.__ruyiSandboxCount = (globalThis.__ruyiSandboxCount || 0) + 1;
            return globalThis.__ruyiSandboxCount;
            """,
            as_expr=False,
            sandbox="example07",
        )
        normal_value = page.run_js("return globalThis.__ruyiSandboxCount || 0")
        print(f"   sandbox 计数: {sandbox_value}")
        print(f"   页面主世界计数: {normal_value}")

        # 14. 获取当前 context 的 realms
        print("\n14. 获取脚本Realms:")
        realms = page.get_realms()
        realm_types = sorted({realm.type or "unknown" for realm in realms})
        print(f"   Realm数量: {len(realms)}")
        print(f"   Realm类型: {realm_types}")

        # 15. 通过高层 script 结果对象执行并读取 handle/value
        print("\n15. 通过高层脚本接口执行:")
        eval_result = page.eval_handle(
            "JSON.stringify({title: document.title, ready: document.readyState})"
        )
        print(f"   evaluate 返回类型: {eval_result.type}")
        print(f"   evaluate 结果: {eval_result.result.value}")

        # 16. 预加载脚本
        print("\n16. 预加载脚本 add/removePreloadScript:")
        preload_id = page.add_preload_script("""() => {
            window.__example07Preload = 'preload-ready';
        }""")
        page.get(test_url)
        page.wait(1)
        preload_value = page.run_js("return window.__example07Preload")
        print(f"   preload脚本ID: {preload_id.id}")
        print(f"   preload注入结果: {preload_value}")
        page.remove_preload_script(preload_id)

        # 17. 移除预加载脚本后再次导航
        print("\n17. 移除预加载脚本后验证:")
        page.get(test_url)
        page.wait(1)
        removed_value = page.run_js("return window.__example07Preload || null")
        print(f"   移除后注入结果: {removed_value}")

        print("\n" + "=" * 60)
        print("✓ 所有JavaScript执行测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(2)
        page.quit()


if __name__ == "__main__":
    test_javascript()

```

```
# -*- coding: utf-8 -*-
"""
示例7: JavaScript执行
测试功能：
- 执行JavaScript代码
- 获取返回值
- 传递参数
- 在元素上执行JS
- 修改页面内容
"""

import os
import sys
import io

# 设置控制台输出编码为UTF-8（Windows兼容）
if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))

from ruyipage import FirefoxPage, FirefoxOptions


def test_javascript():
    """测试JavaScript执行功能"""
    print("=" * 60)
    print("测试7: JavaScript执行")
    print("=" * 60)

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        # 加载测试页面
        test_page = os.path.join(
            os.path.dirname(__file__), "test_pages", "test_page.html"
        )
        test_url = "file:///" + os.path.abspath(test_page).replace("\\", "/")
        page.get(test_url)
        page.wait(1)

        # 1. 执行简单的JavaScript
        print("\n1. 执行简单的JavaScript:")
        result = page.run_js("return 1 + 2")
        print(f"   1 + 2 = {result}")

        # 2. 获取页面信息
        print("\n2. 获取页面信息:")
        title = page.run_js("return document.title")
        print(f"   页面标题: {title}")

        url = page.run_js("return window.location.href")
        print(f"   页面URL: {url}")

        # 3. 修改页面内容
        print("\n3. 修改页面内容:")
        page.run_js(
            'document.getElementById("main-title").textContent = "标题已被JS修改"'
        )
        new_title = page.ele("#main-title").text
        print(f"   修改后的标题: {new_title}")

        # 4. 传递参数
        print("\n4. 传递参数到JavaScript:")
        result = page.run_js("return arguments[0] + arguments[1]", 10, 20)
        print(f"   10 + 20 = {result}")

        # 5. 在元素上执行JavaScript
        print("\n5. 在元素上执行JavaScript:")
        btn = page.ele("#click-btn")
        btn_text = btn.run_js("function() { return this.textContent; }")
        print(f"   按钮文本: {btn_text}")

        # 修改元素样式
        btn.run_js(
            'function() { this.style.background = "red"; this.style.color = "white"; }'
        )
        page.wait(0.5)
        print(f"   ✓ 按钮样式已修改")

        # 6. 获取元素属性
        print("\n6. 通过JS获取元素属性:")
        input_elem = page.ele("#text-input")
        placeholder = input_elem.run_js("function() { return this.placeholder; }")
        print(f"   输入框placeholder: {placeholder}")

        # 7. 执行复杂的JavaScript
        print("\n7. 执行复杂的JavaScript:")
        result = page.run_js("""
            (() => {
                const elements = document.querySelectorAll('.test-class');
                return Array.from(elements).map(el => el.textContent);
            })()
        """)
        print(f"   所有.test-class元素的文本: {result}")

        # 8. 修改输入框的值
        print("\n8. 通过JS修改输入框:")
        page.run_js("document.getElementById('text-input').value = 'JS设置的值'")
        value = page.ele("#text-input").value
        print(f"   输入框的值: {value}")

        # 9. 通过JS触发事件
        print("\n9. 通过JS触发事件:")
        page.run_js('document.getElementById("click-btn").click()')
        page.wait(0.5)
        result = page.ele("#click-result").text
        print(f"   点击结果: {result}")

        # 10. 获取计算样式
        print("\n10. 获取元素的计算样式:")
        color = page.run_js("""
            (() => {
                const elem = document.getElementById('click-btn');
                return window.getComputedStyle(elem).backgroundColor;
            })()
        """)
        print(f"   按钮背景色: {color}")

        # 11. 滚动到元素
        print("\n11. 通过JS滚动到元素:")
        page.run_js('document.getElementById("scroll-section").scrollIntoView()')
        page.wait(0.5)
        print(f"   ✓ 已滚动到滚动测试区域")

        # 12. 创建新元素
        print("\n12. 通过JS创建新元素:")
        page.run_js("""
            const div = document.createElement('div');
            div.id = 'js-created';
            div.textContent = 'JavaScript创建的元素';
            div.style.padding = '10px';
            div.style.background = '#ffeb3b';
            document.body.appendChild(div);
        """)
        page.wait(0.5)
        new_elem = page.ele("#js-created")
        print(f"   新元素文本: {new_elem.text}")

        # 13. 在 sandbox 中执行脚本
        print("\n13. 在sandbox中执行JavaScript:")
        sandbox_value = page.run_js(
            """
            globalThis.__ruyiSandboxCount = (globalThis.__ruyiSandboxCount || 0) + 1;
            return globalThis.__ruyiSandboxCount;
            """,
            as_expr=False,
            sandbox="example07",
        )
        normal_value = page.run_js("return globalThis.__ruyiSandboxCount || 0")
        print(f"   sandbox 计数: {sandbox_value}")
        print(f"   页面主世界计数: {normal_value}")

        # 14. 获取当前 context 的 realms
        print("\n14. 获取脚本Realms:")
        realms = page.get_realms()
        realm_types = sorted({realm.type or "unknown" for realm in realms})
        print(f"   Realm数量: {len(realms)}")
        print(f"   Realm类型: {realm_types}")

        # 15. 通过高层 script 结果对象执行并读取 handle/value
        print("\n15. 通过高层脚本接口执行:")
        eval_result = page.eval_handle(
            "JSON.stringify({title: document.title, ready: document.readyState})"
        )
        print(f"   evaluate 返回类型: {eval_result.type}")
        print(f"   evaluate 结果: {eval_result.result.value}")

        # 16. 预加载脚本
        print("\n16. 预加载脚本 add/removePreloadScript:")
        preload_id = page.add_preload_script("""() => {
            window.__example07Preload = 'preload-ready';
        }""")
        page.get(test_url)
        page.wait(1)
        preload_value = page.run_js("return window.__example07Preload")
        print(f"   preload脚本ID: {preload_id.id}")
        print(f"   preload注入结果: {preload_value}")
        page.remove_preload_script(preload_id)

        # 17. 移除预加载脚本后再次导航
        print("\n17. 移除预加载脚本后验证:")
        page.get(test_url)
        page.wait(1)
        removed_value = page.run_js("return window.__example07Preload || null")
        print(f"   移除后注入结果: {removed_value}")

        print("\n" + "=" * 60)
        print("✓ 所有JavaScript执行测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(2)
        page.quit()


if __name__ == "__main__":
    test_javascript()

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
