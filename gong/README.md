# Gong MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that combines Gong APIs:

- Auditing
- Calls
- CRM
- Data Privacy
- Engage
- Engagement
- Library
- Meetings
- Permissions
- Settings
- Stats
- Users

These APIs translate into namespace in generated TS/JS SDK with the name `gong`:

- file: `./openapi-spec/gong-auditing-openapi.yml`
    - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-auditing-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-auditing-openapi.yml)
- file: `./openapi-spec/gong-calls-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-calls-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-calls-openapi.yml)
- file: `./openapi-spec/gong-crm-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-crm-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-crm-openapi.yml)
- file: `./openapi-spec/gong-data-privacy-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-data-privacy-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-data-privacy-openapi.yml)
- file: `./openapi-spec/gong-engage-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-engage-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-engage-openapi.yml)
- file: `./openapi-spec/gong-engagement-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-engagement-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-engagement-openapi.yml)
- file: `./openapi-spec/gong-library-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-library-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-library-openapi.yml)
- file: `./openapi-spec/gong-meetings-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-meetings-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-meetings-openapi.yml)
- file: `./openapi-spec/gong-permissions-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-permissions-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-permissions-openapi.yml)
- file: `./openapi-spec/gong-settings-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-settings-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-settings-openapi.yml)
- file: `./openapi-spec/gong-stats-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-stats-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-stats-openapi.yml)
- file: `./openapi-spec/gong-users-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-users-openapi.yml](https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/_original/gong-users-openapi.yml)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=57 namespace=gong
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=57 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[0000] ➔ Loaded config                              
INFO[0000] ➔ Creating server                            
INFO[0000] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.2.0
INFO[2026-09-02T22:06:48-07:00] In memory sessions storage: creating storage 
INFO[2026-09-02T22:06:48-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-09-02T22:06:48-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
