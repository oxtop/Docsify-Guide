# Cursor 中使用 MCP 案例

## 5.1 工具定位
- AI 编程 IDE，集成 MCP 后支持外部工具调用。
- 对话模式：Ask、Agent、Manual。

## 5.2 配置方式
- **全局设置**：Settings → MCP → Add Server。
- **项目级设置**：`.cursor/mcp.json` 文件。

## 5.3 案例
任务：**北京一日游攻略**
- 调用高德地图 API 获取地铁路线和美食。
- 写入 MySQL 数据库（subway_trips, location_foods）。
- 导出为 txt 文件。
- 生成 HTML 页面。
