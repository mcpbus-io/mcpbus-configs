# Confluence MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Confluence API.

These APIs translate into name space in TS/JS SDK: `confluence`.

## OpenAPI spec files

### Confluence API

File: `./openapi-spec/openapi-v2.v3.json`

Source: [https://dac-static.atlassian.com/cloud/confluence/openapi-v2.v3.json](https://dac-static.atlassian.com/cloud/confluence/openapi-v2.v3.json)


### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=217 namespace=confluence
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=217 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-24T23:43:01-07:00] ➔ Loaded config                              
INFO[2026-07-24T23:43:01-07:00] ➔ Creating server                            
INFO[2026-07-24T23:43:01-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.18
INFO[2026-07-24T23:43:01-07:00] In memory sessions storage: creating storage 
INFO[2026-07-24T23:43:01-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-24T23:43:01-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```