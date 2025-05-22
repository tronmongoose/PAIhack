# PAIhack
MCP server vulnerability scan for 2025 hackathon

# 🛡️ Agentic Threat Radar

**Hackathon Project** | _Scanning and Securing MCP Servers with Agentic Radar_

---

## 📌 Overview

This project demonstrates how to scan and detect vulnerabilities in [MCP (Model Context Protocol)](https://github.com/golf-mcp/golf) servers using [Agentic Radar](https://github.com/splx-ai/agentic-radar), an open-source static and dynamic security analysis tool for LLM agent workflows.

We build a minimal MCP server using the Golf framework, intentionally inject a vulnerability for demo purposes, and scan it using Agentic Radar to generate a human-readable security report. The result shows how platform teams can gain visibility into tool usage, prompt flows, and potential attack surfaces in LLM pipelines.

---

## ⚙️ Tech Stack

- 🧱 **[Golf MCP](https://github.com/golf-mcp/golf)** – Framework for building MCP-compatible servers
- 🔍 **[Agentic Radar](https://github.com/splx-ai/agentic-radar)** – Static and dynamic scanner for agent workflows
- 🐍 Python (3.10+)
- 🐳 Optional Docker setup

---

## 🗂️ Project Structure

```bash
.
├── mcp-server/             # MCP server built with Golf
│   └── routes/             # MCP bundle definitions and tool declarations
│   └── run_server.py       # Entry point
├── scans/                  # Output scan reports (HTML/JSON)
├── test-bundles/           # Sample JSON bundles with vulnerabilities
├── radar-scan.sh           # CLI helper script to run Agentic Radar
└── README.md
