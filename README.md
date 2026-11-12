# Pi Security for Cursor IDE

Pi Security brings security findings, remediation guidance, design reviews, and secure-development guidance into Cursor IDE. Use it to understand security context and take informed action without leaving your development workflow.

![Pi Security logo](assets/pi-favicon-light.svg)

This release supports Cursor IDE.

## Install

### From this repository as a local marketplace

1. In Cursor's local marketplace flow, select the root of this repository.
2. Confirm that Cursor imports the marketplace as `pi-security-cursor`.
3. Install **Pi Security** for your project or user account.

The `pi-security-cursor` marketplace entry resolves the Cursor plugin from the repository root. If you also imported Pi Security's Claude plugin, do not select its `pi-security` marketplace; that is a separate package for Claude Code and Cowork.

### Direct local development

Cursor can also load the repository directly from `~/.cursor/plugins/local/pi-security`. Copy the repository there, or create a symlink to it, then restart Cursor or run **Developer: Reload Window**. This path loads `.cursor-plugin/plugin.json` directly and does not use the marketplace manifest.

### From Cursor Marketplace

When the public Pi Security listing is available:

1. Open **Customize** in the Cursor sidebar.
2. Find **Pi Security** and select **Install**.
3. Choose whether to install it for your project or for your user account.

## Sign in to Pi

After installation, enable the `pi-security` MCP server in **Customize**. Cursor opens Pi's sign-in flow in your browser and connects to your Pi environment.

See [SETUP.md](SETUP.md) for detailed setup and troubleshooting.

## What you can do

The plugin includes six skills:

| Skill | Use it to |
| --- | --- |
| `investigate-finding` | Find, explain, summarize, or compare Pi findings |
| `review-security-posture` | Review threat-model context and PR security posture |
| `remediation-guidance` | Retrieve remediation guidance for findings and vulnerable packages |
| `security-design-review` | Start a design review from a supported document URL or pasted Markdown, and record a verdict on each of its gaps |
| `ingest-markdown-report` | Submit a Markdown security report to Pi |
| `secure-development-playbook` | Get secure-development guidance for an engineering task |

Cursor can select a relevant skill automatically. To choose one yourself, enter its name in Agent chat, such as `/investigate-finding`.

Example prompts:

- "Explain Pi finding FND-123."
- "Review the security posture for the payments service."
- "Get the remediation plan for lodash in the storefront codebase."
- "Start a Pi design review for this Confluence document."
- "Accept the fix on the first gap of that design review and accept the risk on the second."
- "Submit this pasted report as `pentest-summary.md`."
- "Use Pi's secure-development playbook for this webhook endpoint."

## Confirm actions in Pi

Some skills submit content, start hosted work, or record design-review verdicts. Before taking one of these actions, the skill summarizes what it will do and asks you to confirm. A queued or started response means Pi is processing the request; it does not mean the work is complete.

Report ingestion uses Markdown pasted into the conversation. Design reviews accept pasted Markdown or a supported Confluence or Notion document URL. For other formats, use the Pi web app.

## Manage or remove the plugin

Use **Customize** to enable or disable the plugin, its skills, or the `pi-security` MCP server. Uninstalling or disconnecting the plugin removes access from Cursor but does not delete data in Pi.

## Support and legal

- Support: [contact@pi.security](mailto:contact@pi.security)
- Security reports: [SECURITY.md](SECURITY.md)
- License: [MIT](LICENSE)
- [Privacy Policy](https://www.pi.security/privacy-policy)
- [Terms and Conditions](https://www.pi.security/terms-and-conditions)
- [Data Processing Agreement](https://www.pi.security/data-processing-agreement)
