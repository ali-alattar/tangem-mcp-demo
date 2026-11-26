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

## Troubleshooting

- **No wallet approved for the session**: open the Tangem app and approve a wallet for the connected agent, then try again.
- **`get_tokens` returns an empty addresses list**: the Tangem app has not shared the addresses yet. Open the app, select the wallet and refresh.
- **A send request stays `CREATED`**: nobody has signed it yet. Open the request in the Tangem app (or the deeplink), review it and sign it, then check the status again.
