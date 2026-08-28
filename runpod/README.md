# Runpod v2 MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Runpod API v2.

This API translates into namespace in TS/JS SDK: `runpod`.

## OpenAPI spec files

### Runpod API v2

File: `./openapi-spec/openapi.json`

Source: [https://docs.runpod.io/api-reference-v2/overview#openapi-schema](https://docs.runpod.io/api-reference-v2/overview#openapi-schema)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=53 namespace=runpod
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=53 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-27T19:09:39-07:00] ➔ Loaded config                              
INFO[2026-08-27T19:09:39-07:00] ➔ Creating server                            
INFO[2026-08-27T19:09:39-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.24
INFO[2026-08-27T19:09:39-07:00] In memory sessions storage: creating storage 
INFO[2026-08-27T19:09:39-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-27T19:09:39-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
