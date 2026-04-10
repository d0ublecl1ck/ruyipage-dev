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
[Automation](https://0xshoulderlab.site/automation) / PDF
RuyiPage Docs
#  RuyiPage PDF
这里集中讲 PDF 打印、纸张参数、页范围和导出形式。
## API 与参数说明
### page.save_pdf
`page.save_pdf(path, **kwargs)`
将页面保存为 PDF 文件
参数说明
参数 | 说明  
---|---  
path | 本地文件路径或目录路径。  
**kwargs | 参数含义与默认值请结合当前 API 场景使用。  
### page.pdf
`page.pdf(as_bytes=True)`
获取 PDF bytes 数据
参数说明
参数 | 说明  
---|---  
as_bytes=True | 参数含义与默认值请结合当前 API 场景使用。  
### page.pdf
`page.pdf(as_base64=True)`
获取 PDF base64 数据
参数说明
参数 | 说明  
---|---  
as_base64=True | 参数含义与默认值请结合当前 API 场景使用。  
### page.save_pdf
`page.save_pdf(path, paper_format='A4')`
指定纸张尺寸
参数说明
参数 | 说明  
---|---  
path | 本地文件路径或目录路径。  
paper_format='A4' | PDF 纸张尺寸，如 A4。  
### page.save_pdf
`page.save_pdf(path, landscape=True)`
横向打印
参数说明
参数 | 说明  
---|---  
path | 本地文件路径或目录路径。  
landscape=True | 参数含义与默认值请结合当前 API 场景使用。  
### page.save_pdf
`page.save_pdf(path, margin=...)`
自定义页边距
参数说明
参数 | 说明  
---|---  
path | 本地文件路径或目录路径。  
margin=... | 参数含义与默认值请结合当前 API 场景使用。  
### page.save_pdf
`page.save_pdf(path, page_ranges='1-3')`
指定打印页范围
参数说明
参数 | 说明  
---|---  
path | 本地文件路径或目录路径。  
page_ranges='1-3' | PDF 打印页码范围，如 1-3。  
## 相关示例
  * 参见示例中心：/automation/examples


## 相关示例源码
### PDF 打印：纸张尺寸、方向、边距、页范围与导出数据
examples/19_pdf_printing.py
集中说明 save_pdf 的参数覆盖能力。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/19_pdf_printing.py) page.save_pdfpage.pdf
  * 基础 PDF 导出
  * A4 纸张和背景打印
  * 横向打印与缩放
  * 自定义页边距和页范围
  * 获取 PDF bytes 与 base64


源码文件：`app/content/ruyipage_examples/19_pdf_printing.py` · 仓库：[19_pdf_printing.py](https://github.com/LoseNine/ruyipage/blob/main/examples/19_pdf_printing.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
# =============================
# RuyiPage 示例注释版
# 标题: PDF 打印：纸张尺寸、方向、边距、页范围与导出数据
# 说明: 集中说明 save_pdf 的参数覆盖能力。
# 你会学到:
#   1. 基础 PDF 导出
#   2. A4 纸张和背景打印
#   3. 横向打印与缩放
#   4. 自定义页边距和页范围
#   5. 获取 PDF bytes 与 base64
# 相关 API: page.save_pdf, page.pdf
# =============================

# -*- coding: utf-8 -*-
"""示例19: PDF 打印（完整参数覆盖）"""

import io
import os
import sys


if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")


sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))

from ruyipage import FirefoxOptions, FirefoxPage


def _size_of(path):
    return os.path.getsize(path) if os.path.exists(path) else 0


def test_pdf_printing():
    print("=" * 60)
    print("测试19: PDF打印功能")
    print("=" * 60)

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        test_page = os.path.join(
            os.path.dirname(__file__), "test_pages", "test_page.html"
        )
        test_url = "file:///" + os.path.abspath(test_page).replace("\\", "/")
        page.get(test_url)
        page.wait(1)

        output_dir = os.path.join(os.path.dirname(__file__), "output", "pdf")
        os.makedirs(output_dir, exist_ok=True)

        # 1) 基本打印
        print("\n1. 基本PDF打印:")
        p1 = os.path.join(output_dir, "basic.pdf")
        page.save_pdf(p1)
        print(f"   ✓ 已保存: {p1} ({_size_of(p1)} bytes)")

        # 2) A4 + 背景
        print("\n2. A4 + 背景:")
        p2 = os.path.join(output_dir, "a4_bg.pdf")
        page.save_pdf(
            p2,
            page={"width": 21.0, "height": 29.7},
            background=True,
        )
        print(f"   ✓ 已保存: {p2} ({_size_of(p2)} bytes)")

        # 3) 横向 + 缩放 + 页边距
        print("\n3. 横向 + 缩放 + 页边距:")
        p3 = os.path.join(output_dir, "landscape_scaled.pdf")
        page.save_pdf(
            p3,
            orientation="landscape",
            scale=0.9,
            margin={
                "top": 1.2,
                "bottom": 1.2,
                "left": 1.0,
                "right": 1.0,
            },
        )
        print(f"   ✓ 已保存: {p3} ({_size_of(p3)} bytes)")

        # 4) 指定页范围 + shrinkToFit
        print("\n4. 指定页范围 + shrinkToFit:")
        p4 = os.path.join(output_dir, "page_ranges_shrink.pdf")
        page.save_pdf(
            p4,
            page_ranges=["1-2"],
            shrink_to_fit=True,
        )
        print(f"   ✓ 已保存: {p4} ({_size_of(p4)} bytes)")

        # 5) 获取 bytes/base64
        print("\n5. 获取 bytes / base64:")
        pdf_bytes = page.pdf(page_ranges=["1"])
        pdf_b64 = (
            __import__("base64")
            .b64encode(page.pdf(shrink_to_fit=False))
            .decode("ascii")
        )
        print(f"   bytes长度: {len(pdf_bytes)}")
        print(f"   base64长度: {len(pdf_b64)}")

        if not (len(pdf_bytes) > 100 and len(pdf_b64) > 100):
            raise RuntimeError("PDF 输出长度异常")

        print("\n" + "=" * 60)
        print("✓ 所有PDF打印测试通过！")
        print(f"PDF保存在: {output_dir}")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(1)
        page.quit()


if __name__ == "__main__":
    test_pdf_printing()

```

```
# -*- coding: utf-8 -*-
"""示例19: PDF 打印（完整参数覆盖）"""

import io
import os
import sys


if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")


sys.path.insert(0, os.path.join(os.path.dirname(__file__), ".."))

from ruyipage import FirefoxOptions, FirefoxPage


def _size_of(path):
    return os.path.getsize(path) if os.path.exists(path) else 0


def test_pdf_printing():
    print("=" * 60)
    print("测试19: PDF打印功能")
    print("=" * 60)

    opts = FirefoxOptions()
    opts.headless(False)
    page = FirefoxPage(opts)

    try:
        test_page = os.path.join(
            os.path.dirname(__file__), "test_pages", "test_page.html"
        )
        test_url = "file:///" + os.path.abspath(test_page).replace("\\", "/")
        page.get(test_url)
        page.wait(1)

        output_dir = os.path.join(os.path.dirname(__file__), "output", "pdf")
        os.makedirs(output_dir, exist_ok=True)

        # 1) 基本打印
        print("\n1. 基本PDF打印:")
        p1 = os.path.join(output_dir, "basic.pdf")
        page.save_pdf(p1)
        print(f"   ✓ 已保存: {p1} ({_size_of(p1)} bytes)")

        # 2) A4 + 背景
        print("\n2. A4 + 背景:")
        p2 = os.path.join(output_dir, "a4_bg.pdf")
        page.save_pdf(
            p2,
            page={"width": 21.0, "height": 29.7},
            background=True,
        )
        print(f"   ✓ 已保存: {p2} ({_size_of(p2)} bytes)")

        # 3) 横向 + 缩放 + 页边距
        print("\n3. 横向 + 缩放 + 页边距:")
        p3 = os.path.join(output_dir, "landscape_scaled.pdf")
        page.save_pdf(
            p3,
            orientation="landscape",
            scale=0.9,
            margin={
                "top": 1.2,
                "bottom": 1.2,
                "left": 1.0,
                "right": 1.0,
            },
        )
        print(f"   ✓ 已保存: {p3} ({_size_of(p3)} bytes)")

        # 4) 指定页范围 + shrinkToFit
        print("\n4. 指定页范围 + shrinkToFit:")
        p4 = os.path.join(output_dir, "page_ranges_shrink.pdf")
        page.save_pdf(
            p4,
            page_ranges=["1-2"],
            shrink_to_fit=True,
        )
        print(f"   ✓ 已保存: {p4} ({_size_of(p4)} bytes)")

        # 5) 获取 bytes/base64
        print("\n5. 获取 bytes / base64:")
        pdf_bytes = page.pdf(page_ranges=["1"])
        pdf_b64 = (
            __import__("base64")
            .b64encode(page.pdf(shrink_to_fit=False))
            .decode("ascii")
        )
        print(f"   bytes长度: {len(pdf_bytes)}")
        print(f"   base64长度: {len(pdf_b64)}")

        if not (len(pdf_bytes) > 100 and len(pdf_b64) > 100):
            raise RuntimeError("PDF 输出长度异常")

        print("\n" + "=" * 60)
        print("✓ 所有PDF打印测试通过！")
        print(f"PDF保存在: {output_dir}")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback

        traceback.print_exc()
    finally:
        page.wait(1)
        page.quit()


if __name__ == "__main__":
    test_pdf_printing()

```

### 基础导航与页面保存
examples/01_basic_navigation.py
覆盖最基础的页面访问、前进后退和保存 HTML/PDF。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/01_basic_navigation.py) FirefoxPageFirefoxOptionspage.getpage.titlepage.urlpage.htmlpage.backpage.forward
  * 打开本地文件页面和外部页面
  * 读取标题、URL 和 HTML 源码
  * 执行前进、后退和刷新
  * 保存 HTML 与 PDF


源码文件：`app/content/ruyipage_examples/01_basic_navigation.py` · 仓库：[01_basic_navigation.py](https://github.com/LoseNine/ruyipage/blob/main/examples/01_basic_navigation.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
# =============================
# RuyiPage 示例注释版
# 标题: 基础导航与页面保存
# 说明: 覆盖最基础的页面访问、前进后退和保存 HTML/PDF。
# 你会学到:
#   1. 打开本地文件页面和外部页面
#   2. 读取标题、URL 和 HTML 源码
#   3. 执行前进、后退和刷新
#   4. 保存 HTML 与 PDF
# 相关 API: FirefoxPage, FirefoxOptions, page.get, page.title, page.url, page.html, page.back, page.forward
# =============================

# -*- coding: utf-8 -*-
"""
示例1: 基础导航和页面操作
测试功能：
- 创建浏览器实例
- 页面导航
- 获取标题、URL
- 前进、后退、刷新
- 页面保存
"""

import os
import sys
import io

# 设置控制台输出编码为UTF-8（Windows兼容）
if sys.platform == 'win32':
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8')
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding='utf-8')

sys.path.insert(0, os.path.join(os.path.dirname(__file__), '..'))

from ruyipage import FirefoxPage, FirefoxOptions

def test_basic_navigation():
    """测试基础导航功能"""
    print("=" * 60)
    print("测试1: 基础导航和页面操作")
    print("=" * 60)

    # 创建浏览器实例
    opts = FirefoxOptions()
    opts.headless(False)  # 显示浏览器窗口
    page = FirefoxPage(opts)

    try:
        # 1. 导航到测试页面
        test_page = os.path.join(os.path.dirname(__file__), 'test_pages', 'test_page.html')
        test_url = 'file:///' + os.path.abspath(test_page).replace('\\', '/')
        print(f"\n1. 导航到测试页面: {test_url}")
        page.get(test_url)
        print(f"   ✓ 页面加载成功")

        # 2. 获取页面信息
        print(f"\n2. 获取页面信息:")
        print(f"   标题: {page.title}")
        print(f"   URL: {page.url}")
        print(f"   HTML长度: {len(page.html)} 字符")

        # 3. 导航到其他页面
        print(f"\n3. 导航到其他页面:")
        page.get('https://www.example.com')
        print(f"   当前标题: {page.title}")
        print(f"   当前URL: {page.url}")

        # 4. 后退
        print(f"\n4. 后退到上一页:")
        page.back()
        page.wait(1)
        print(f"   当前标题: {page.title}")

        # 5. 前进
        print(f"\n5. 前进到下一页:")
        page.forward()
        page.wait(1)
        print(f"   当前标题: {page.title}")

        # 6. 刷新页面
        print(f"\n6. 刷新页面:")
        page.refresh()
        page.wait(1)
        print(f"   ✓ 页面已刷新")

        # 7. 保存页面
        print(f"\n7. 保存页面:")
        save_dir = os.path.join(os.path.dirname(__file__), 'output')
        os.makedirs(save_dir, exist_ok=True)

        # 保存为HTML
        html_path = page.save(path=save_dir, name='example_page', as_pdf=False)
        print(f"   HTML已保存: {html_path}")

        # 保存为PDF
        pdf_path = page.save(path=save_dir, name='example_page', as_pdf=True)
        print(f"   PDF已保存: {pdf_path}")

        print("\n" + "=" * 60)
        print("✓ 所有基础导航测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback
        traceback.print_exc()
    finally:
        # 关闭浏览器
        page.wait(2)
        page.quit()

if __name__ == '__main__':
    test_basic_navigation()

```

```
# -*- coding: utf-8 -*-
"""
示例1: 基础导航和页面操作
测试功能：
- 创建浏览器实例
- 页面导航
- 获取标题、URL
- 前进、后退、刷新
- 页面保存
"""

import os
import sys
import io

# 设置控制台输出编码为UTF-8（Windows兼容）
if sys.platform == 'win32':
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding='utf-8')
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding='utf-8')

sys.path.insert(0, os.path.join(os.path.dirname(__file__), '..'))

from ruyipage import FirefoxPage, FirefoxOptions

def test_basic_navigation():
    """测试基础导航功能"""
    print("=" * 60)
    print("测试1: 基础导航和页面操作")
    print("=" * 60)

    # 创建浏览器实例
    opts = FirefoxOptions()
    opts.headless(False)  # 显示浏览器窗口
    page = FirefoxPage(opts)

    try:
        # 1. 导航到测试页面
        test_page = os.path.join(os.path.dirname(__file__), 'test_pages', 'test_page.html')
        test_url = 'file:///' + os.path.abspath(test_page).replace('\\', '/')
        print(f"\n1. 导航到测试页面: {test_url}")
        page.get(test_url)
        print(f"   ✓ 页面加载成功")

        # 2. 获取页面信息
        print(f"\n2. 获取页面信息:")
        print(f"   标题: {page.title}")
        print(f"   URL: {page.url}")
        print(f"   HTML长度: {len(page.html)} 字符")

        # 3. 导航到其他页面
        print(f"\n3. 导航到其他页面:")
        page.get('https://www.example.com')
        print(f"   当前标题: {page.title}")
        print(f"   当前URL: {page.url}")

        # 4. 后退
        print(f"\n4. 后退到上一页:")
        page.back()
        page.wait(1)
        print(f"   当前标题: {page.title}")

        # 5. 前进
        print(f"\n5. 前进到下一页:")
        page.forward()
        page.wait(1)
        print(f"   当前标题: {page.title}")

        # 6. 刷新页面
        print(f"\n6. 刷新页面:")
        page.refresh()
        page.wait(1)
        print(f"   ✓ 页面已刷新")

        # 7. 保存页面
        print(f"\n7. 保存页面:")
        save_dir = os.path.join(os.path.dirname(__file__), 'output')
        os.makedirs(save_dir, exist_ok=True)

        # 保存为HTML
        html_path = page.save(path=save_dir, name='example_page', as_pdf=False)
        print(f"   HTML已保存: {html_path}")

        # 保存为PDF
        pdf_path = page.save(path=save_dir, name='example_page', as_pdf=True)
        print(f"   PDF已保存: {pdf_path}")

        print("\n" + "=" * 60)
        print("✓ 所有基础导航测试通过！")
        print("=" * 60)

    except Exception as e:
        print(f"\n✗ 测试失败: {e}")
        import traceback
        traceback.print_exc()
    finally:
        # 关闭浏览器
        page.wait(2)
        page.quit()

if __name__ == '__main__':
    test_basic_navigation()

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
