# Cloudflare MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Cloudflare APIs.

This API translates into names space in TS/JS SDK: `cloudflare`.

## OpenAPI spec files

### Cloudflare API

File: `./openapi-spec/openapi.json`

Source: [https://github.com/cloudflare/api-schemas](https://github.com/cloudflare/api-schemas)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0002] ➔ JS/TS runtime namespace created             methods_num=3251 namespace=cloudflare
INFO[0002] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=3251 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-08T14:05:18-07:00] ➔ Loaded config                              
INFO[2026-08-08T14:05:18-07:00] ➔ Creating server                            
INFO[2026-08-08T14:05:18-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.20
INFO[2026-08-08T14:05:18-07:00] In memory sessions storage: creating storage 
INFO[2026-08-08T14:05:18-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-08T14:05:18-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
