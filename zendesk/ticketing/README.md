# Zendesk Support Ticketing API MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Zendesk Support Ticketing API.

This API translates into names space in TS/JS SDK: `zendeskTicketing`.

## OpenAPI spec files

### Zendesk Support Ticketing API

File: `./openapi-spec/oas.yaml`

Source: [https://developer.zendesk.com/api-reference/ticketing/introduction/#download-openapi-file](https://developer.zendesk.com/api-reference/ticketing/introduction/#download-openapi-file)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=625 namespace=zendeskTicketing
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=625 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-25T20:53:41-07:00] ➔ Loaded config                              
INFO[2026-07-25T20:53:41-07:00] ➔ Creating server                            
INFO[2026-07-25T20:53:41-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.18
INFO[2026-07-25T20:53:41-07:00] In memory sessions storage: creating storage 
INFO[2026-07-25T20:53:41-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-25T20:53:41-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```

### NOTE

Don't forget, Zendesk's auth requires you to add `/token` suffix to your email specified in config field `apiAuthUser`.