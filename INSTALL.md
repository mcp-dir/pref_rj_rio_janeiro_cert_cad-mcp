# Instalação rápida

Prefeitura RJ Rio de Janeiro: Certidão de Elementos Cadastrais - IPTU é um servidor MCP remoto hospedado em `https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad`. Você não baixa nem roda nada localmente — só aponta seu cliente pra essa URL.

A auth acontece em runtime: clientes com **OAuth 2.1** (Claude Desktop, Cursor, VS Code recentes) abrem o browser na 1ª chamada (magic-link). Clientes sem OAuth recebem a tool `authenticate` — abra `https://app.mcp.ai/agent-auth`, faça login, copie o JWT e cole no chat.

---

## Claude (Web e Desktop)

[➕ Abrir no Claude e conectar](https://claude.ai/new?modal=add-custom-connector#settings/customize-connectors)

Manual: [claude.ai/customize/connectors](https://claude.ai/customize/connectors?surface=cowork) → **+** → **Adicionar conector personalizado** → `Prefeitura RJ Rio de Janeiro: Certidão de Elementos Cadastrais - IPTU` / `https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad`.

Config file (legado): `~/Library/Application Support/Claude/claude_desktop_config.json` (macOS) ou `%APPDATA%\Claude\claude_desktop_config.json` (Windows):

```json
{ "mcpServers": { "pref_rj_rio_janeiro_cert_cad": { "type": "http", "url": "https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad" } } }
```

## Cursor

[➕ Instalar no Cursor](cursor://anysphere.cursor-deeplink/mcp/install?name=pref_rj_rio_janeiro_cert_cad&config=eyJ1cmwiOiJodHRwczovL2FwaS5tY3AuYWkvcF9wcmVmX3JqX3Jpb19qYW5laXJvX2NlcnRfY2FkIn0=)

`.cursor/mcp.json`:
```json
{ "mcpServers": { "pref_rj_rio_janeiro_cert_cad": { "url": "https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad" } } }
```

## VS Code (Copilot Chat)

[➕ Instalar no VS Code](vscode:mcp/install?name=pref_rj_rio_janeiro_cert_cad&config=%7B%22type%22%3A%22http%22%2C%22url%22%3A%22https%3A%2F%2Fapi.mcp.ai%2Fp_pref_rj_rio_janeiro_cert_cad%22%7D)

`.vscode/mcp.json`:
```json
{ "servers": { "pref_rj_rio_janeiro_cert_cad": { "type": "http", "url": "https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad" } } }
```

## Outros clientes MCP

Qualquer cliente com **MCP over HTTP**. URL fixa:

```
https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad
```

Dúvidas? [pref_rj_rio_janeiro_cert_cad@mcp.ai](mailto:pref_rj_rio_janeiro_cert_cad@mcp.ai)
