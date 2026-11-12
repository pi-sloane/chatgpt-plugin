# Changelog

## [0.1.5] - 2026-11-12

- Added `decide-pi-design-review-gaps`: read a design review's gaps and record a verdict on each (accept fix, accepted risk, false positive, or reopen) with `pi_design_review_gap_update_status`, after a workspace check and explicit confirmation.

## [0.1.4] - 2026-08-25

- Bound development guidance to one playbook lookup for a stable task, with repository-evidence fallback for adjacent or missing coverage and one short generic lookup only for genuinely necessary threat-model context.

## [0.1.3] - 2026-07-17

- Restored ChatGPT GitHub import by relying on the MCP server's OAuth discovery metadata instead of unsupported MCP-only app fields.

## [0.1.2] - 2026-07-17

- Configured Codex MCP installations to request the `mcp:access` scope explicitly.

## [0.1.1] - 2026-07-17

- Added the Pi Security icon to the plugin directory and composer.

## [0.1.0] - 2026-07-16

Initial release of Pi Security for ChatGPT and Codex.

### Included

- Investigate Pi findings while keeping evidence separate from interpretation.
- Review threat-model and Code Gatekeeper security posture.
- Retrieve finding and package remediation guidance.
- Start security design reviews from supported links or pasted Markdown.
- Import pasted Markdown security reports.
- Apply Pi secure-development playbooks and share confirmed feedback.
