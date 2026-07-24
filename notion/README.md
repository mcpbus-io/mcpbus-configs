# Notion MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Notion API.

This API translates into names space in TS/JS SDK: `notion`.

## OpenAPI spec files

### Notion API

File: `./openapi-spec/openapi.json`

Source: [https://developers.notion.com/openapi.json](https://developers.notion.com/openapi.json)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0001] ➔ JS/TS runtime namespace created             methods_num=48 namespace=notion
INFO[0001] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=48 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-24T00:07:11-07:00] ➔ Loaded config                              
INFO[2026-07-24T00:07:11-07:00] ➔ Creating server                            
INFO[2026-07-24T00:07:11-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.17
INFO[2026-07-24T00:07:11-07:00] In memory sessions storage: creating storage 
INFO[2026-07-24T00:07:11-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-24T00:07:11-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
