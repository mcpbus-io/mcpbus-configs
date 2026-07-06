# MCPBus config examples

There are number of MCPBus config examples categorized in folders in this repo.

All the config examples are validated and confirmed to be loading in Code-mode no problem.

## How to run MCPBus

Command to load MCPBus with a specific config:

```shell
mcpbus --config=path/to/your/mcpbus.conf
```

## Sensitive information in configs

The important part of configs are your auth-credentials which MCPBus will use when accessing the APIs.

These config values are pre-populated by default with placeholders prefixed with `MCPBUS_`

To load actual auth-credentials via config - you have two options:

1. replace placeholders with your usernames, passwords, api-keys or bot-tokens

2. Or, set environment variable that matches placeholder names, MCPBus picks all values prefixed with `MCPBUS_` and resolves them into environment variables. For example, if you have in your config file value `MCPBUS_MY_AUTH_TOKEN` then this value will be read from environment variable with the same name `MCPBUS_MY_AUTH_TOKEN`

How to get MCPBus and for more information please refer to: [https://mcpbus.io](https://mcpbus.io)
