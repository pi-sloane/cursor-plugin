# Pi Security for Cursor IDE

Pi Security brings security findings, remediation guidance, design reviews, and secure-development guidance into Cursor IDE. Use it to understand security context and take informed action without leaving your development workflow.

![Pi Security logo](assets/pi-security.png)

This release supports Cursor IDE.

## Install

When the Pi Security listing is available in Cursor Marketplace:

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
| `security-design-review` | Start a design review from a supported document URL or pasted Markdown |
| `ingest-markdown-report` | Submit a Markdown security report to Pi |
| `secure-development-playbook` | Get secure-development guidance for an engineering task |

Cursor can select a relevant skill automatically. To choose one yourself, enter its name in Agent chat, such as `/investigate-finding`.

Example prompts:

- "Explain Pi finding FND-123."
- "Review the security posture for the payments service."
- "Get the remediation plan for lodash in the storefront codebase."
- "Start a Pi design review for this Confluence document."
- "Submit this pasted report as `pentest-summary.md`."
- "Use Pi's secure-development playbook for this webhook endpoint."

## Confirm actions in Pi

Some skills submit content or start hosted work. Before taking one of these actions, the skill summarizes what it will do and asks you to confirm. A queued or started response means Pi is processing the request; it does not mean the work is complete.

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
