# MCP 基础概念

## 1.1 什么是 MCP
- **MCP（Model Context Protocol，模型上下文协议）**
  由 **Anthropic** 在 2024 年底提出，是一种开放标准协议。
  目标：为 **大语言模型（LLM）** 提供统一、标准化的方式，与 **外部工具和数据源** 交互。

- 核心作用：
  - 解决传统 AI 集成的 **M×N 架构复杂度问题**。
  - 统一接口 → LLM 通过 MCP 与外部 API、数据库、本地工具交互。
  - 让 LLM 不止能“对话”，还能“做事”。

## 1.2 MCP 的 C/S 架构
MCP 遵循 **Client-Server 架构**，包含 5 个核心概念：

1. **MCP Host**：宿主应用（如 Claude Desktop、Cursor、Cline、Cherry Studio）。
2. **MCP Client**：桥梁，负责请求转发和结果返回。
3. **MCP Server**：提供工具，可为本地程序或远程 API。
4. **本地资源**：本机文件/数据。
5. **远程资源**：云端 API / Web 数据。

## 1.3 通信机制
1. **stdio（本地进程通信）**
   - 优点：速度快、无需网络、可靠。
   - 缺点：配置复杂，不适合分布式。
2. **SSE（Server-Sent Events）**
   - 优点：基于 HTTP，配置简单，适合远程服务。
   - 应用：实时日志、推送、分布式场景。
