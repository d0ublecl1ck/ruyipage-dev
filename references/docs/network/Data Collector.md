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
[Automation](https://0xshoulderlab.site/automation) / Data Collector
RuyiPage Docs
#  RuyiPage Data Collector
collector 是 RuyiPage 在网络场景中非常有价值的高层能力，适合单列说明。
## API 与参数说明
### page.network.add_data_collector
`page.network.add_data_collector(phases)`
添加数据采集器，phases 指定阶段
参数说明
参数 | 说明  
---|---  
phases | 采集阶段列表，如 responseStarted/responseCompleted。  
### collector.get
`collector.get(request_id)`
按 request_id 读取采集的响应数据
参数说明
参数 | 说明  
---|---  
request_id | 参数含义与默认值请结合当前 API 场景使用。  
### collector.disown
`collector.disown(request_id)`
释放指定采集句柄
参数说明
参数 | 说明  
---|---  
request_id | 参数含义与默认值请结合当前 API 场景使用。  
### collector.remove
`collector.remove()`
移除整个 collector
## 相关示例
  * 参见示例中心：/automation/examples


## 相关示例源码
### 网络数据采集器：响应体抓取、读取与释放
examples/28_network_data_collector.py
用于说明 add_data_collector 在数据抓取和协议观测中的价值。
GitHub 仓库 [查看仓库源码](https://github.com/LoseNine/ruyipage/blob/main/examples/28_network_data_collector.py) page.network.set_extra_headerspage.network.set_cache_behaviorpage.network.add_data_collectorcollector.getcollector.disowncollector.removepage.listen.start
  * 注入额外请求头
  * 设置缓存 bypass
  * 添加并使用 data collector 采集 response 数据
  * 按 request_id 读取采集结果
  * 释放采集句柄并移除 collector


源码文件：`app/content/ruyipage_examples/28_network_data_collector.py` · 仓库：[28_network_data_collector.py](https://github.com/LoseNine/ruyipage/blob/main/examples/28_network_data_collector.py)
python 注释版
注释版 原始版 自动换行 复制代码
```
#!/usr/bin/env python
# =============================
# RuyiPage 示例注释版
# 标题: 网络数据采集器：响应体抓取、读取与释放
# 说明: 用于说明 add_data_collector 在数据抓取和协议观测中的价值。
# 你会学到:
#   1. 注入额外请求头
#   2. 设置缓存 bypass
#   3. 添加并使用 data collector 采集 response 数据
#   4. 按 request_id 读取采集结果
#   5. 释放采集句柄并移除 collector
# 相关 API: page.network.set_extra_headers, page.network.set_cache_behavior, page.network.add_data_collector, collector.get, collector.disown, collector.remove, page.listen.start
# =============================

# -*- coding: utf-8 -*-
"""示例28: Network Data Collector（严格结果版）"""

import io
import sys
from typing import Dict, List

if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

from ruyipage import DataCollector, DataPacket, FirefoxPage, InterceptedRequest
from ruyipage._functions.tools import find_free_port

from test_server import TestServer


def add_result(
    results: List[Dict[str, str]], item: str, status: str, note: str
) -> None:
    results.append({"item": item, "status": status, "note": note})


def print_results(results: List[Dict[str, str]]) -> None:
    print("\n| 项目 | 状态 | 说明 |")
    print("| --- | --- | --- |")
    for row in results:
        print(f"| {row['item']} | {row['status']} | {row['note']} |")


def main() -> None:
    print("=" * 70)
    print("测试 28: Network Data Collector")
    print("=" * 70)

    page = FirefoxPage()
    results: List[Dict[str, str]] = []
    collector: DataCollector | None = None
    server = None

    try:
        server = TestServer(port=find_free_port(9230, 9330)).start()
        base_url = server.get_url("")[:-1]

        page.get("about:blank")
        add_result(
            results, "页面加载", "成功", f"about:blank 已加载，服务地址: {base_url}"
        )

        page.network.set_extra_headers({"X-Test-Collector": "yes"})
        add_result(
            results, "network.setExtraHeaders", "成功", "已设置 X-Test-Collector"
        )

        try:
            page.network.set_cache_behavior("bypass")
            add_result(
                results, "network.setCacheBehavior", "成功", "缓存行为已设为 bypass"
            )
        except Exception as e:
            add_result(results, "network.setCacheBehavior", "不支持", str(e)[:120])

        collector = page.network.add_data_collector(
            ["responseCompleted"],
            data_types=["response"],
        )
        if collector.id:
            add_result(
                results, "network.addDataCollector", "成功", f"collector={collector.id}"
            )
        else:
            add_result(
                results, "network.addDataCollector", "失败", "未返回 collector ID"
            )

        page.intercept.start_requests()
        page.listen.start("/api/collector")
        page.run_js(
            f"fetch('{base_url}/api/collector').catch(()=>null); return true;",
            as_expr=False,
        )

        req: InterceptedRequest | None = page.intercept.wait(timeout=8)

        if req:
            has_header = "X-Test-Collector" in req.headers
            add_result(
                results,
                "request header injected",
                "成功" if has_header else "失败",
                f"request_id={req.request_id}, X-Test-Collector={has_header}",
            )
            req.continue_request()
        else:
            add_result(
                results,
                "request header injected",
                "失败",
                "未捕获到 beforeRequestSent 请求",
            )

        packet: DataPacket | None = page.listen.wait(timeout=8)

        if packet:
            add_result(
                results,
                "network.responseCompleted observed",
                "成功",
                f"status={packet.status} url={packet.url}",
            )
        else:
            add_result(
                results,
                "network.responseCompleted observed",
                "失败",
                "未在超时内观察到 responseCompleted",
            )

        if collector and req:
            got_response_data = False
            try:
                data = collector.get(req.request_id, data_type="response")
                if data.has_data:
                    got_response_data = True
                    add_result(
                        results,
                        "network.getData response",
                        "成功",
                        f"bytes={data.bytes} base64={'yes' if data.base64 else 'no'}",
                    )
                else:
                    add_result(
                        results, "network.getData response", "失败", f"raw={data.raw}"
                    )
            except Exception as e:
                add_result(results, "network.getData response", "失败", str(e)[:120])

            if got_response_data:
                try:
                    collector.disown(req.request_id, data_type="response")
                    add_result(
                        results, "network.disownData", "成功", "已释放 response 数据"
                    )
                except Exception as e:
                    add_result(results, "network.disownData", "失败", str(e)[:120])

                try:
                    data_after = collector.get(req.request_id, data_type="response")
                    if not data_after.has_data:
                        add_result(
                            results,
                            "network.getData after disown",
                            "成功",
                            "释放后已无可用数据",
                        )
                    else:
                        add_result(
                            results,
                            "network.getData after disown",
                            "跳过",
                            f"释放后仍可读取: {data_after.raw}",
                        )
                except Exception as e:
                    add_result(
                        results,
                        "network.getData after disown",
                        "成功",
                        f"释放后读取报错: {str(e)[:100]}",
                    )
            else:
                add_result(
                    results,
                    "network.disownData",
                    "跳过",
                    "未成功拿到 response 数据，跳过释放验证",
                )
                add_result(
                    results,
                    "network.getData after disown",
                    "跳过",
                    "未成功拿到 response 数据，跳过释放后验证",
                )

        if collector:
            try:
                collector.remove()
                add_result(
                    results,
                    "network.removeDataCollector",
                    "成功",
                    f"已移除 {collector.id}",
                )
                collector = None
            except Exception as e:
                add_result(results, "network.removeDataCollector", "失败", str(e)[:120])

        page.network.clear_extra_headers()
        add_result(results, "clear extra headers", "成功", "额外请求头已清理")

        print_results(results)

    except Exception as e:
        add_result(results, "示例执行", "失败", str(e)[:120])
        print_results(results)
        raise
    finally:
        try:
            page.listen.stop()
        except Exception:
            pass
        try:
            page.intercept.stop()
        except Exception:
            pass
        try:
            if server is not None:
                server.stop()
        except Exception:
            pass
        if collector:
            try:
                collector.remove()
            except Exception:
                pass
        try:
            page.network.clear_extra_headers()
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
"""示例28: Network Data Collector（严格结果版）"""

import io
import sys
from typing import Dict, List

if sys.platform == "win32":
    sys.stdout = io.TextIOWrapper(sys.stdout.buffer, encoding="utf-8")
    sys.stderr = io.TextIOWrapper(sys.stderr.buffer, encoding="utf-8")

from ruyipage import DataCollector, DataPacket, FirefoxPage, InterceptedRequest
from ruyipage._functions.tools import find_free_port

from test_server import TestServer


def add_result(
    results: List[Dict[str, str]], item: str, status: str, note: str
) -> None:
    results.append({"item": item, "status": status, "note": note})


def print_results(results: List[Dict[str, str]]) -> None:
    print("\n| 项目 | 状态 | 说明 |")
    print("| --- | --- | --- |")
    for row in results:
        print(f"| {row['item']} | {row['status']} | {row['note']} |")


def main() -> None:
    print("=" * 70)
    print("测试 28: Network Data Collector")
    print("=" * 70)

    page = FirefoxPage()
    results: List[Dict[str, str]] = []
    collector: DataCollector | None = None
    server = None

    try:
        server = TestServer(port=find_free_port(9230, 9330)).start()
        base_url = server.get_url("")[:-1]

        page.get("about:blank")
        add_result(
            results, "页面加载", "成功", f"about:blank 已加载，服务地址: {base_url}"
        )

        page.network.set_extra_headers({"X-Test-Collector": "yes"})
        add_result(
            results, "network.setExtraHeaders", "成功", "已设置 X-Test-Collector"
        )

        try:
            page.network.set_cache_behavior("bypass")
            add_result(
                results, "network.setCacheBehavior", "成功", "缓存行为已设为 bypass"
            )
        except Exception as e:
            add_result(results, "network.setCacheBehavior", "不支持", str(e)[:120])

        collector = page.network.add_data_collector(
            ["responseCompleted"],
            data_types=["response"],
        )
        if collector.id:
            add_result(
                results, "network.addDataCollector", "成功", f"collector={collector.id}"
            )
        else:
            add_result(
                results, "network.addDataCollector", "失败", "未返回 collector ID"
            )

        page.intercept.start_requests()
        page.listen.start("/api/collector")
        page.run_js(
            f"fetch('{base_url}/api/collector').catch(()=>null); return true;",
            as_expr=False,
        )

        req: InterceptedRequest | None = page.intercept.wait(timeout=8)

        if req:
            has_header = "X-Test-Collector" in req.headers
            add_result(
                results,
                "request header injected",
                "成功" if has_header else "失败",
                f"request_id={req.request_id}, X-Test-Collector={has_header}",
            )
            req.continue_request()
        else:
            add_result(
                results,
                "request header injected",
                "失败",
                "未捕获到 beforeRequestSent 请求",
            )

        packet: DataPacket | None = page.listen.wait(timeout=8)

        if packet:
            add_result(
                results,
                "network.responseCompleted observed",
                "成功",
                f"status={packet.status} url={packet.url}",
            )
        else:
            add_result(
                results,
                "network.responseCompleted observed",
                "失败",
                "未在超时内观察到 responseCompleted",
            )

        if collector and req:
            got_response_data = False
            try:
                data = collector.get(req.request_id, data_type="response")
                if data.has_data:
                    got_response_data = True
                    add_result(
                        results,
                        "network.getData response",
                        "成功",
                        f"bytes={data.bytes} base64={'yes' if data.base64 else 'no'}",
                    )
                else:
                    add_result(
                        results, "network.getData response", "失败", f"raw={data.raw}"
                    )
            except Exception as e:
                add_result(results, "network.getData response", "失败", str(e)[:120])

            if got_response_data:
                try:
                    collector.disown(req.request_id, data_type="response")
                    add_result(
                        results, "network.disownData", "成功", "已释放 response 数据"
                    )
                except Exception as e:
                    add_result(results, "network.disownData", "失败", str(e)[:120])

                try:
                    data_after = collector.get(req.request_id, data_type="response")
                    if not data_after.has_data:
                        add_result(
                            results,
                            "network.getData after disown",
                            "成功",
                            "释放后已无可用数据",
                        )
                    else:
                        add_result(
                            results,
                            "network.getData after disown",
                            "跳过",
                            f"释放后仍可读取: {data_after.raw}",
                        )
                except Exception as e:
                    add_result(
                        results,
                        "network.getData after disown",
                        "成功",
                        f"释放后读取报错: {str(e)[:100]}",
                    )
            else:
                add_result(
                    results,
                    "network.disownData",
                    "跳过",
                    "未成功拿到 response 数据，跳过释放验证",
                )
                add_result(
                    results,
                    "network.getData after disown",
                    "跳过",
                    "未成功拿到 response 数据，跳过释放后验证",
                )

        if collector:
            try:
                collector.remove()
                add_result(
                    results,
                    "network.removeDataCollector",
                    "成功",
                    f"已移除 {collector.id}",
                )
                collector = None
            except Exception as e:
                add_result(results, "network.removeDataCollector", "失败", str(e)[:120])

        page.network.clear_extra_headers()
        add_result(results, "clear extra headers", "成功", "额外请求头已清理")

        print_results(results)

    except Exception as e:
        add_result(results, "示例执行", "失败", str(e)[:120])
        print_results(results)
        raise
    finally:
        try:
            page.listen.stop()
        except Exception:
            pass
        try:
            page.intercept.stop()
        except Exception:
            pass
        try:
            if server is not None:
                server.stop()
        except Exception:
            pass
        if collector:
            try:
                collector.remove()
            except Exception:
                pass
        try:
            page.network.clear_extra_headers()
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
