# Stripe MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Stripe API.

This API translates into names space in TS/JS SDK: `stripe`.

## OpenAPI spec files

### Stripe API

File: `./openapi-spec/stripe-openapi.spec3.yaml`

Source: [https://raw.githubusercontent.com/stripe/openapi/refs/heads/master/latest/openapi.spec3.yaml](https://raw.githubusercontent.com/stripe/openapi/refs/heads/master/latest/openapi.spec3.yaml)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0020] ➔ JS/TS runtime namespace created             methods_num=585 namespace=stripe
INFO[0020] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=583 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-11T21:51:37-07:00] ➔ Loaded config                              
INFO[2026-07-11T21:51:37-07:00] ➔ Creating server                            
INFO[2026-07-11T21:51:37-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.13
INFO[2026-07-11T21:51:37-07:00] In memory sessions storage: creating storage 
INFO[2026-07-11T21:51:37-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-11T21:51:37-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
