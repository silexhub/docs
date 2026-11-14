# Designing an agent workflow

[Documentation home](../README.md)

The examples here explain how to shape a useful workflow. They are not claims of released SilexHub tools.

## Example: compare business information

- **Input:** a small set of synthetic records, the fields to compare, and comparison rules.
- **Task:** find differences within that defined scope.
- **Output:** a comparison with field-level differences that a person or the next step can inspect.
- **Failure case:** missing required fields should produce a clear validation error rather than a result that appears complete.

A useful integration must state the accepted input size and formats, output field meanings, and what happens when the task cannot be completed. Those limits should come from the actual capability.

## Example: connect a result to software

A person chooses the action and authorizes the required scope. The agent supplies the documented fields. The service checks access and returns an inspectable result.

For actions that change external state, define duplicate-request and retry behavior before automating them. A retry should follow the documented contract, not an assumption that repeating the action is harmless.

## Build around a complete contract

Choose the task → review input and output → authorize scope → execute through a supported interface → use the result.

The first real workflow should verify both success and a relevant failure. See the [MCP capability contract](https://github.com/silexhub/mcp-server/blob/main/docs/capability-contract.md) for the information an agent-facing integration needs.
