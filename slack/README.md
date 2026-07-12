# Slack MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Slack Web API.

This API translates into names space in TS/JS SDK: `slack`.

## OpenAPI spec files

### Slack API

File: `./openapi-spec/slack-web-openapi-v2.json`

Source: [https://raw.githubusercontent.com/slackapi/slack-api-specs/refs/heads/master/web-api/slack_web_openapi_v2.json](https://raw.githubusercontent.com/slackapi/slack-api-specs/refs/heads/master/web-api/slack_web_openapi_v2.json)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=174 namespace=slack
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=174 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-11T22:06:27-07:00] ➔ Loaded config                              
INFO[2026-07-11T22:06:27-07:00] ➔ Creating server                            
INFO[2026-07-11T22:06:27-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.13
INFO[2026-07-11T22:06:27-07:00] In memory sessions storage: creating storage 
INFO[2026-07-11T22:06:27-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-11T22:06:27-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
