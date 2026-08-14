# Calendly MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Calendly API:

- Scheduled Events
- Activity Log
- Availability
- Data Compliance
- Event Types
- Groups
- Invitees
- Organizations
- Routing Forms
- Shares
- Users
- Webhook Subscriptions

These APIs translate into namespace `calendly` in generated TS/JS SDK:

- file: `./openapi-spec/calendly-scheduled-events-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-scheduled-events-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-scheduled-events-api-openapi.yml)
- file: `./openapi-spec/calendly-activity-log-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-activity-log-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-activity-log-api-openapi.yml)
- file: `./openapi-spec/calendly-availability-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-availability-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-availability-api-openapi.yml)
- file: `./openapi-spec/calendly-data-compliance-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-data-compliance-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-data-compliance-api-openapi.yml)
- file: `./openapi-spec/calendly-event-types-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-event-types-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-event-types-api-openapi.yml)
- file: `./openapi-spec/calendly-groups-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-groups-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-groups-api-openapi.yml)
- file: `./openapi-spec/calendly-invitees-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-invitees-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-invitees-api-openapi.yml)
- file: `./openapi-spec/calendly-organizations-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-organizations-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-organizations-api-openapi.yml)
- file: `./openapi-spec/calendly-routing-forms-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-routing-forms-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-routing-forms-api-openapi.yml)
- file: `./openapi-spec/calendly-shares-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-shares-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-shares-api-openapi.yml)
- file: `./openapi-spec/calendly-users-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-users-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-users-api-openapi.yml)
- file: `./openapi-spec/calendly-webhook-subscriptions-api-openapi.yml`
  - source: [https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-webhook-subscriptions-api-openapi.yml](https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-webhook-subscriptions-api-openapi.yml)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=35 namespace=calendly
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=35 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-13T22:37:12-07:00] ➔ Loaded config                              
INFO[2026-08-13T22:37:12-07:00] ➔ Creating server                            
INFO[2026-08-13T22:37:12-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.23
INFO[2026-08-13T22:37:12-07:00] In memory sessions storage: creating storage 
INFO[2026-08-13T22:37:12-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-13T22:37:12-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
