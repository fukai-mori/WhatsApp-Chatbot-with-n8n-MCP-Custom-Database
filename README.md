## 🤖 WhatsApp Chatbot with n8n + MCP + Custom Database

This project is a modular, scalable, and open chatbot architecture using:

- **n8n** for orchestration and workflow automation
- **WhatsApp** for user interaction (via Twilio API or other gateways)
- **MCP (Model Context Protocol)** to organize the communication between the client, server, and database
- **Custom PostgreSQL Database** to serve dynamic query-based responses

---

## 🔧 Architecture Overview

[User via WhatsApp]
      ↓
[n8n receives message via Webhook]
      ↓
[n8n (MCP Client) sends JSON-RPC to MCP Server]
      ↓
[MCP Server processes logic + queries database]
      ↓
[MCP Server returns response (JSON-RPC)]
      ↓
[n8n sends reply via WhatsApp API]

## 💡 Features

🧠 Query your own database via WhatsApp messages
📦 Decoupled architecture using the MCP protocol
🛠️ Customizable logic using any LLM or decision engine (optional)
💬 Seamless WhatsApp integration (Twilio, Z-API, Gupshup, etc.)
🔄 Full control over message flow using n8n
