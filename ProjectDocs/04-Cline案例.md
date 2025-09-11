# Cline 中使用 MCP 案例

## 4.1 工具定位
- VSCode 插件，被称为“程序员的副驾驶”。
- 核心：任务分解 + MCP 调用。

## 4.2 配置步骤
1. 安装 VSCode + Cline 插件。
2. 配置 API Key，选择模型。
3. 配置 MCP Server（如 mysqldb-mcp-server、desktop-commander）。

## 4.3 案例
任务：**北京一日游攻略**
- 从 `beijing_trip` 数据库中提取美食 & 地铁信息。
- 存入 txt 文件。
- 自动生成 HTML 展示页面。
