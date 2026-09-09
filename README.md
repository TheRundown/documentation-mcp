# TheRundown Documentation MCP

This is the official Cursor plugin wrapper for TheRundown's public
documentation MCP at `https://docs.therundown.io/mcp`.

The server searches published API documentation: endpoint contracts, V2 event
and market schemas, parameters, market IDs, authentication guidance, plan
limits, billing, and integration examples. It is documentation-only. It does
not return live odds or scores, access Product API data, or require a customer
API key.

## Cursor configuration

The plugin supplies this remote MCP configuration:

```json
{
  "mcpServers": {
    "therundown-documentation": {
      "type": "http",
      "url": "https://docs.therundown.io/mcp"
    }
  }
}
```

This repository supplies Cursor plugin metadata and a standalone `mcp.json`
configuration.

## Related official resources

- [Documentation MCP guide](https://docs.therundown.io/documentation-mcp)
- [Product API OpenAPI](https://docs.therundown.io/openapi.yaml)
- [Local Data MCP](https://github.com/TheRundown/data-mcp): a separate,
  local stdio server that uses a customer-managed API key. It is not a hosted
  data MCP endpoint.

## First conversation

Ask: “Search TheRundown’s documentation for the V2 event and market response
hierarchy, then explain which fields identify the event, market, participant,
line, price, and price update time. Link to the relevant public documentation.”
