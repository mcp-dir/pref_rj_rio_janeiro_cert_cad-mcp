# Instalação detalhada

Prefeitura RJ Rio de Janeiro: Certidão de Elementos Cadastrais - IPTU é um servidor MCP remoto. Aponte seu cliente pra `https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad`. Snippets rápidos: [INSTALL.md](../INSTALL.md).

| Cliente | URL | Auth |
|---|---|---|
| Claude Desktop | `https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad` | OAuth 2.1 ou agent-auth |
| Cursor | `https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad` | OAuth 2.1 ou agent-auth |
| VS Code (Copilot) | `https://api.mcp.ai/p_pref_rj_rio_janeiro_cert_cad` | OAuth 2.1 ou agent-auth |

A config JSON é a mesma em todos: só a URL, sem headers.

## Desinstalar

Remova o bloco `mcpServers.pref_rj_rio_janeiro_cert_cad` (ou `servers.pref_rj_rio_janeiro_cert_cad` no VS Code) do config do cliente e reinicie.
