# BambooHR API MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to BambooHR API.

This API translates into names space in TS/JS SDK: `bamboohr`.

## OpenAPI spec files

### BambooHR API

File: `./openapi-spec/public-openapi.yaml`

Source: [https://openapi.bamboohr.io/main/latest/docs/openapi/public-openapi.yaml](https://openapi.bamboohr.io/main/latest/docs/openapi/public-openapi.yaml)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=294 namespace=bamboohr
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=294 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-26T21:58:33-07:00] ➔ Loaded config                              
INFO[2026-07-26T21:58:33-07:00] ➔ Creating server                            
INFO[2026-07-26T21:58:33-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8085 server_name=MCPBus server_version=1.1.18
INFO[2026-07-26T21:58:33-07:00] In memory sessions storage: creating storage 
INFO[2026-07-26T21:58:33-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-26T21:58:33-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8085"
```

### NOTE

BambooHR API-key is passed over HTTP Basic Auth where your API-key is provided in username and password can be any string `"x"` in our example.