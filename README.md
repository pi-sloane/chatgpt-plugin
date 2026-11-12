# Pi Security for ChatGPT and Codex

Bring security context from Pi into the way you already work. Pi Security helps you investigate findings, understand your security posture, get remediation guidance, review designs, import Markdown reports, and follow secure-development guidance without leaving your conversation.

![Pi Security logo](assets/pi-favicon-light.svg)

## What you can do

| Workflow | Use it to |
| --- | --- |
| **Investigate a finding** | Understand the evidence behind a Pi finding and what it may mean |
| **Review security posture** | Bring together threat-model context and Code Gatekeeper results |
| **Get remediation guidance** | Retrieve Pi's recommended next steps for findings and vulnerable packages |
| **Start a design review** | Send a supported design document to Pi for security review |
| **Decide design-review gaps** | Accept the fix, accept the risk, mark false positive, or reopen each gap of a completed review |
| **Import a Markdown report** | Start processing a security report you paste into the conversation |
| **Use the secure-development playbook** | Apply relevant security guidance while planning or building software |

The plugin clearly separates information returned by Pi from its own interpretation, so you can see what is evidence and what is analysis.

## Get started

1. Open **Plugins** in ChatGPT Work or the ChatGPT desktop app.
2. Find **Pi Security** and select **Install**.
3. Connect your Pi Security account when prompted.
4. Start a new conversation and ask for the outcome you want, or choose Pi Security with `@`.

Pi respects the access available to your signed-in Pi account. If you belong to more than one Pi workspace, the plugin will identify the active workspace before taking an action.

### Try these prompts

- “Investigate Pi finding FND-123 and explain the supporting evidence.”
- “Review my current threat-model and Code Gatekeeper posture.”
- “Get the remediation guidance for this finding without changing code.”
- “Accept the fix on the first gap of my latest design review and accept the risk on the second.”
- “Use Pi's secure-development playbook for this implementation.”

Examples use synthetic identifiers. Replace them with your own Pi finding or project details.

## You're always in control

Finding investigations and posture reviews are read-only. Before Pi Security starts an action—such as queuing a design review, recording a design-review verdict, importing a report, preparing a package remediation plan, or sending playbook feedback—it will:

1. show the destination and relevant details;
2. ask you to confirm; and
3. make one request only after you confirm.

Starting a review or import means Pi has queued the work. It does not mean processing is already complete.

## Supported content

For this release, Pi Security supports:

- Pi finding IDs and supported Pi finding links;
- supported Confluence and Notion links for design reviews; and
- Markdown pasted directly into the conversation.

Markdown security reports need a filename ending in `.md` or `.markdown`. This plugin does not directly upload attachments, PDFs, Word documents, screenshots, or files from your computer. For those formats, use the [Pi Security website](https://www.pi.security/) or the Sloane CLI when appropriate.

## Where it works

Pi Security is designed for:

- ChatGPT Work on the web;
- Work and Codex in the ChatGPT desktop app; and
- Codex CLI and the Codex IDE extension when installed through a plugin marketplace.

This release is available in English and is not intended for mobile use.

## Updates and removal

To update Pi Security, open its page in the plugin directory and install an available update, then begin a new conversation.

To remove it, open **Pi Security** in the plugin directory and select **Uninstall**. Your Pi account connection may remain available to other integrations until you disconnect it separately in your ChatGPT or Pi settings.

## Privacy and security

Only share content you are authorized to send to Pi. Avoid including credentials, secrets, or unrelated customer data in prompts and reports.

- [Privacy Policy](https://www.pi.security/privacy-policy)
- [Terms and Conditions](https://www.pi.security/terms-and-conditions)
- [Data Processing Agreement](https://www.pi.security/data-processing-agreement)
- [Security reporting](SECURITY.md)

## Help

Visit [pi.security](https://www.pi.security/) or email [contact@pi.security](mailto:contact@pi.security).

Developers who want to improve this plugin can read [CONTRIBUTING.md](CONTRIBUTING.md).
