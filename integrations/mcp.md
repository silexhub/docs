# MCP integration

[Documentation home](../README.md)

Model Context Protocol (MCP) gives compatible agent clients a standard way to discover and access capabilities. A GitHub repository hosts integration materials; an MCP service handles protocol requests. Creating a repository does not itself start a service.

## SilexHub status

The official public integration repository is [silexhub/mcp-server](https://github.com/silexhub/mcp-server). It currently contains connection guidance, the capability contract, and release requirements. A public server endpoint and installable package have not been released.

## Start with a hosted connection

The first planned route is a hosted MCP integration. The public guide will identify the actual server address, supported clients, authorization flow, and available capabilities after validation.

A local adapter may follow when installation or distribution needs justify it. Publishing an adapter does not include the hosted SilexHub application or a bundled database.

## Read next

- [Connection guide](https://github.com/silexhub/mcp-server/blob/main/docs/connection-guide.md)
- [Capability contract](https://github.com/silexhub/mcp-server/blob/main/docs/capability-contract.md)
- [Release requirements](https://github.com/silexhub/mcp-server/blob/main/docs/release-readiness.md)
- [Current availability](../reference/availability.md)

Client configuration will be published alongside a verified release. Do not infer an endpoint from the product domain or from a repository name.
