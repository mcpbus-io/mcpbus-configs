# Sentry MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Sentry API.

This API translates into namespace in TS/JS SDK: `sentry`.

## How to run example

Sentry schema describes its paths component schemas in sub-folders so you will need to run `mcpbus` from folder where the main OpenAPI spec file is: 

```shell
cd openapi-spec
MCPBUS_SENTRY_AUTH_TOKEN=yourtokenhere mcpbus --config=../mcpbus.conf 
```

## OpenAPI spec files

### Sentry Management

File: `./openapi-spec/openapi.json`

Source: [https://github.com/getsentry/sentry/tree/master/api-docs](https://github.com/getsentry/sentry/tree/master/api-docs)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=18 namespace=sentry
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=18 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-27T19:17:50-07:00] ➔ Loaded config                              
INFO[2026-08-27T19:17:50-07:00] ➔ Creating server                            
INFO[2026-08-27T19:17:50-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.24
INFO[2026-08-27T19:17:50-07:00] In memory sessions storage: creating storage 
INFO[2026-08-27T19:17:50-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-27T19:17:50-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
