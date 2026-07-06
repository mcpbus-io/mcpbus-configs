# JIRA MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that combines two JIRA APIs - Platform API and Agile API.

These APIs translate into two names spaces in TS/JS SDK: `jira` and `jiraAgile`.

## OpenAPI spec files

### JIRA Platform API

File: `./openapi-spec/jira-swagger.v3.json`

Source: [https://dac-static.atlassian.com/cloud/jira/platform/swagger-v3.v3.json](https://dac-static.atlassian.com/cloud/jira/platform/swagger-v3.v3.json)

### JIRA Agile API

File: `./openapi-spec/jira-swagger-agile.v3.json`

Source: [https://dac-static.atlassian.com/cloud/jira/software/swagger.v3.json](https://dac-static.atlassian.com/cloud/jira/software/swagger.v3.json)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num=710 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-07-06T16:37:30-07:00] ➔ Loaded config                              
INFO[2026-07-06T16:37:30-07:00] ➔ Creating server                            
INFO[2026-07-06T16:37:30-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.12
INFO[2026-07-06T16:37:30-07:00] In memory sessions storage: creating storage 
INFO[2026-07-06T16:37:30-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-07-06T16:37:30-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```

### NOTE

Most of JIRA Platform API endpoints have in payload schemas field `"token"` specified as `required`. This field can be omitted in case of HTTP basic auth and most LLMs will know it right out of the box. 

However, some JIRA API write-operation like `jira.assignIssue` or `jira.editIssue` will require `"token"` field to be present in payload, in this case passing empty string will be enough. Please make sure your agen adds this instruction into context or updates memory related to this specific workaround.