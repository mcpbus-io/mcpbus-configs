# Rippling Platform MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to Rippling Platform API.

This API translates into namespace in TS/JS SDK: `rippling`.

## OpenAPI spec files

### Rippling Platform

File: `./openapi-spec/api_spec_2024-08-01_API_Tier_1.yaml`

Source: [https://developer.rippling.com/documentation/rest-api](https://developer.rippling.com/documentation/rest-api)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.update_titles method_title="Update a title"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.delete_titles method_title="Delete a title"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.list_users method_title="List users"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.get_users method_title="Retrieve a specific user"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.list_work_locations method_title="List work locations"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.create_work_locations method_title="Create a new work location"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.delete_work_locations method_title="Delete a work location"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.get_work_locations method_title="Retrieve a specific work location"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.update_work_locations method_title="Update a work location"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.list_workers method_title="List workers"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.get_workers method_title="Retrieve a specific worker"
INFO[0000] ➔ JS/TS SDK method available                  method_name=rippling.workflow_action_executions method_title="Execute a workflow action"
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=102 namespace=rippling
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=102 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-15T23:13:00-07:00] ➔ Loaded config                              
INFO[2026-08-15T23:13:00-07:00] ➔ Creating server                            
INFO[2026-08-15T23:13:00-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.23
INFO[2026-08-15T23:13:00-07:00] In memory sessions storage: creating storage 
INFO[2026-08-15T23:13:00-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-15T23:13:00-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
