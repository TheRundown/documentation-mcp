# TheRundown Documentation MCP

This repository configures only the public documentation MCP. It does not
provide Product API access, live odds, scores, customer keys, or a hosted data
MCP.

Use the same public API working rules described in the documentation:

1. Resolve the event before requesting its data.
2. Treat every price as evidence with its own context and update time.
3. Keep missing data missing; do not invent coverage, prices, or results.
4. Obtain IDs from current Product API responses; documentation can explain an
   ID but does not prove current availability.

The documentation MCP can explain these rules and public contracts. It cannot
return data prices. For scoped data access, see the separate local Data MCP
repository and its customer-managed configuration.

Keep retired affiliate 27 excluded. Do not put customer API keys in prompts,
URLs, or metadata. Do not add private fields or non-public implementation
details to this repository.
