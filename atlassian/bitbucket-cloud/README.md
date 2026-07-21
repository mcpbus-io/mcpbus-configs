# Bitbucket Cloud MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Bitbucket Cloud API.

This API translates into names space in TS/JS SDK: `bitbucket`.

## OpenAPI spec files

### Bitbucket Cloud API

File: `./openapi-spec/swagger.v3.json`

Source: [https://dac-static.atlassian.com/cloud/bitbucket/swagger.v3.json](https://dac-static.atlassian.com/cloud/bitbucket/swagger.v3.json)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=321 namespace=bitbucket
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=295 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-20T23:24:42-07:00] ➔ Loaded config                              
INFO[2026-07-20T23:24:42-07:00] ➔ Creating server                            
INFO[2026-07-20T23:24:42-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.16
INFO[2026-07-20T23:24:42-07:00] In memory sessions storage: creating storage 
INFO[2026-07-20T23:24:42-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-20T23:24:42-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
