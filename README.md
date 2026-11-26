# tangem-mcp-demo

A demo of using the Tangem MCP server with Claude Code.

## What it shows

- **List wallet assets**: read the coins and tokens in a Tangem wallet, with their networks and addresses.
- **Read balances**: check the balance of each address on supported networks.
- **Prepare transactions**: create a send request that you review and sign in the Tangem app. The MCP server never signs or sends funds itself.

## Getting started

1. Add the Tangem MCP server to Claude Code and approve a wallet for the session in the Tangem app.
2. Ask Claude to list your wallet's tokens and balances.
3. To send, ask Claude to prepare a transaction, then open the Tangem app (or the deeplink) to review and sign it.

## Security

Private keys stay on your Tangem card. Every transaction must be confirmed in the Tangem app.
