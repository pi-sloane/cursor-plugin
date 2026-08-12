# Set up Pi Security in Cursor IDE

Pi Security connects to Cursor through a hosted MCP server and uses browser-based sign-in.

## Prerequisites

- A current Cursor IDE release with plugin support
- A Pi Security account for your organization's Pi environment

## Install

When the Pi Security listing is available, open **Customize** in the Cursor sidebar, find **Pi Security**, and select **Install**.

## Sign in to your environment

1. Open **Customize** in Cursor.
2. Find the `pi-security` MCP server and enable it.
3. Continue to Pi's sign-in page when Cursor opens it in your browser.
4. Sign in to your Pi environment, then return to Cursor.

Cursor and Pi handle authentication through this sign-in flow; no API key or manual MCP authentication setup is needed.

## Troubleshooting

- Confirm that both the plugin and the `pi-security` MCP server are enabled in **Customize**.
- For connection or sign-in errors, open Cursor's **Output** panel and select **MCP Logs**.
- If sign-in remains invalid, disconnect and reconnect the MCP server.

MCP logs may contain information from your Pi environment. Remove sensitive details before sharing logs in a public issue.

## Disable or uninstall

Use **Customize** to disable the MCP server temporarily or uninstall Pi Security. This removes access from Cursor IDE without deleting data in Pi.

For help, email [contact@pi.security](mailto:contact@pi.security). Please report security issues through [SECURITY.md](SECURITY.md).
