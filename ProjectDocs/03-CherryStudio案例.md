# Cherry Studio 中使用 MCP 案例

## 3.1 工具定位
- 面向大众用户，低代码可视化平台。
- 内置：对话、知识库、AI绘画、翻译等功能。
- 提供简洁配置界面，轻松接入 MCP 服务。

## 3.2 配置步骤
1. 安装 Cherry Studio，配置 API Key。
2. 安装 `uv` 和 `bun`（内置版本）。
3. 编辑 MCP Server JSON（如 fs、desktop-commander、amap-maps）。
4. 聊天界面选择 MCP Servers，输入需求。

## 3.3 案例
任务：**生成北京一日游攻略**
- 获取地铁路线 → 保存为 txt。
- 获取周边美食 → 保存为 txt。
- 最终合成 HTML 页面。
