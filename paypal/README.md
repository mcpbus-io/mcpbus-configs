# PayPal MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to PayPal APIs.

This API translates into names space in TS/JS SDK: `paypalPayments`.

## OpenAPI spec files

### PayPal API

File: `./openapi-spec/payments_payment_v2.json`

Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payments_payment_v2.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payments_payment_v2.json)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] JS/TS SDK summary                            
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.authorizations_get method_title="Show details for authorized payment"
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.authorizations_capture method_title="Capture authorized payment"
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.authorizations_reauthorize method_title="Reauthorize authorized payment"
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.authorizations_void method_title="Void authorized payment"
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.captures_get method_title="Show captured payment details"
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.captures_refund method_title="Refund captured payment"
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.find_eligible_methods method_title="Find a list of eligible payment methods."
INFO[0000] ➔ JS/TS SDK method available                  method_name=paypalPayments.refunds_get method_title="Show refund details"
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=8 namespace=paypalPayments
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=8 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-04T23:55:34-07:00] ➔ Loaded config                              
INFO[2026-08-04T23:55:34-07:00] ➔ Creating server                            
INFO[2026-08-04T23:55:34-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.20
INFO[2026-08-04T23:55:34-07:00] In memory sessions storage: creating storage 
INFO[2026-08-04T23:55:34-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-04T23:55:34-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```
