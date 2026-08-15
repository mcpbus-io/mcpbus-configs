# PayPal MCPBus config

MCPBus config example: `./mcpbus.conf`

This config creates MCP-connector that provides access to PayPal APIs:

- Billing Subscriptions
- Catalog Products
- Checkout Orders
- Customer Disputes
- Partner Referrals
- Invoicing
- Notifications Webhooks
- Web Experience Profiles
- Payments
- Payouts Batch
- Transaction Search
- Shipment Tracking
- Payment Method Tokens

These APIs translate into namespaces in generated TS/JS SDK:

- `paypalBillingSubscriptions`
    - File: `./openapi-spec/billing_subscriptions_v1.json`
    - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/billing_subscriptions_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/billing_subscriptions_v1.json)
- `paypalCatalogProducts`
  - File: `./openapi-spec/catalogs_products_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/catalogs_products_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/catalogs_products_v1.json)
- `paypalCheckoutOrders`
  - File: `./openapi-spec/checkout_orders_v2.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/checkout_orders_v2.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/checkout_orders_v2.json)
- `paypalCustomerDisputes`
  - File: `./openapi-spec/customer_disputes_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/customer_disputes_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/customer_disputes_v1.json)
- `paypalPartnerReferrals`
  - File: `./openapi-spec/customer_partner_referrals_v2.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/customer_partner_referrals_v2.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/customer_partner_referrals_v2.json)
- `paypalPartnerReferrals`
  - File: `./openapi-spec/customer_partner_referrals_v2.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/customer_partner_referrals_v2.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/customer_partner_referrals_v2.json)
- `paypalInvoicing`
  - File: `./openapi-spec/invoicing_v2.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/invoicing_v2.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/invoicing_v2.json)
- `paypalNotificationsWebhooks`
  - File: `./openapi-spec/notifications_webhooks_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/notifications_webhooks_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/notifications_webhooks_v1.json)
- `paypalWebExperienceProfiles`
  - File: `./openapi-spec/payment-experience_web_experience_profiles_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payment-experience_web_experience_profiles_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payment-experience_web_experience_profiles_v1.json)
- `paypalPayments`
  - File: `./openapi-spec/payments_payment_v2.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payments_payment_v2.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payments_payment_v2.json)
- `paypalPayoutsBatch`
  - File: `./openapi-spec/payments_payouts_batch_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payments_payouts_batch_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/payments_payouts_batch_v1.json)
- `paypalTransactionSearch`
  - File: `./openapi-spec/reporting_transactions_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/reporting_transactions_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/reporting_transactions_v1.json)
- `paypalShipmentTracking`
  - File: `./openapi-spec/shipping_shipment_tracking_v1.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/shipping_shipment_tracking_v1.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/shipping_shipment_tracking_v1.json)
- `paypalPaymentMethodTokens`
  - File: `./openapi-spec/vault_payment_tokens_v3.json`
  - Source: [https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/vault_payment_tokens_v3.json](https://raw.githubusercontent.com/paypal/paypal-rest-api-specifications/refs/heads/main/openapi/vault_payment_tokens_v3.json)

### MCPBus log output

When successful, you should see log output similar to:

```shell
...
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=16 namespace=paypalNotificationsWebhooks
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=2 namespace=paypalTransactionSearch
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=5 namespace=paypalShipmentTracking
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=6 namespace=paypalPaymentMethodTokens
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=16 namespace=paypalBillingSubscriptions
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=4 namespace=paypalCatalogProducts
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=9 namespace=paypalCheckoutOrders
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=2 namespace=paypalPartnerReferrals
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=22 namespace=paypalInvoicing
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=6 namespace=paypalWebExperienceProfiles
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=8 namespace=paypalPayments
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=4 namespace=paypalPayoutsBatch
INFO[0000] ➔ JS/TS runtime namespace created             methods_num=15 namespace=paypalCustomerDisputes
INFO[0000] ➔ JS/TS runtime SDK created                   jit_enabled=true methods_num_total=115 mode="MCPBUs Meta Tool Search (TS/JS SDK runtime)"
INFO[2026-08-14T21:22:52-07:00] ➔ Loaded config                              
INFO[2026-08-14T21:22:52-07:00] ➔ Creating server                            
INFO[2026-08-14T21:22:52-07:00] ➔ Starting MCPBus server                      addr=localhost mcp_version=2025-11-25 port=8080 server_name=MCPBus server_version=1.1.23
INFO[2026-08-14T21:22:52-07:00] In memory sessions storage: creating storage 
INFO[2026-08-14T21:22:52-07:00] ➔ MCP-endpoint                                url="http://localhost:8080/mcp"
INFO[2026-08-14T21:22:52-07:00] ➔ 🚀  MCPBus server is running and ready to accept connections!  addr="localhost:8080"
```

### NOTE

By default, the server index in use is `0` which is PayPal sandbox. To point MCPBus to live PayPal production server, you will need to changes server index to `1` with using `"serverIndex": 1`:

```json
{
    "nameSpace": "paypalBillingSubscriptions",
    "serverIndex": 1,
    "filePath": "./openapi-spec/billing_subscriptions_v1.json",
    "allowDestructive": true,
    "apiAuthToken": "MCPBUS_PAYPAL_TOKEN"
}
```