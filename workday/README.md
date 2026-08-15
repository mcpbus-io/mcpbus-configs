# Workday MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that combines Workday APIs:

- HR
  - Staffing v6
  - Recruiting v3
  - Talent Management v2
  - Performance Management v2
  - Performance Enablement v4.1

These APIs translate into namespaces in generated TS/JS SDK:

- `workdayHrStaffing`
  - file: `./openapi-spec/staffing_oas3.json`
  - source: [https://developer.workday.com/rest-api-explorer/docs#staffing/v6/](https://developer.workday.com/rest-api-explorer/docs#staffing/v6/)
- `workdayHrRecruiting`
  - file: `./openapi-spec/recruiting_oas3.json`
  - source: [https://developer.workday.com/rest-api-explorer/docs/recruiting/v3](https://developer.workday.com/rest-api-explorer/docs/recruiting/v3)
- `workdayHrTalentManagement`
  - file: `./openapi-spec/talentManagement_oas3.json`
  - source: [https://developer.workday.com/rest-api-explorer/docs/talentManagement/v2](https://developer.workday.com/rest-api-explorer/docs/talentManagement/v2)
- `workdayHrPerformanceManagement`
  - file: `./openapi-spec/performanceManagement_oas3.json`
  - source: [https://developer.workday.com/rest-api-explorer/docs/performanceManagement/v2](https://developer.workday.com/rest-api-explorer/docs/performanceManagement/v2)
- `workdayHrPerformanceEnablement`
  - file: `./openapi-spec/performanceEnablement_oas3.json`
  - source: [https://developer.workday.com/rest-api-explorer/docs/performanceEnablement/v4.1](https://developer.workday.com/rest-api-explorer/docs/performanceEnablement/v4.1)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=144 namespace=workdayHrStaffing
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=31 namespace=workdayHrRecruiting
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=21 namespace=workdayHrTalentManagement
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=7 namespace=workdayHrPerformanceManagement
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=23 namespace=workdayHrPerformanceEnablement
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=226 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-11T23:09:54-07:00] ➔ Loaded config                              
INFO[2026-08-11T23:09:54-07:00] ➔ Creating server                            
INFO[2026-08-11T23:09:54-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.22
INFO[2026-08-11T23:09:54-07:00] In memory sessions storage: creating storage 
INFO[2026-08-11T23:09:54-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-11T23:09:54-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```

### NOTE

The auth token can be obtained through Workforce API Explorer.