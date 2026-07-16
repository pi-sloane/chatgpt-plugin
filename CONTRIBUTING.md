# Contributing

Thanks for helping make Pi Security easier and safer to use in ChatGPT and Codex.

## What belongs here

This repository contains the public plugin description, connection configuration, documentation, and six focused skills. Contributions should improve those areas without adding a local server, custom interface, browser extension, background hook, or unrelated automation.

Never include credentials, customer data, private URLs, internal documentation, production logs, or proprietary source code. Use synthetic examples in documentation and tests.

## Writing skills

When changing a skill:

- keep it focused on one user goal;
- explain clearly when it should and should not be used;
- ask for missing identifiers instead of guessing;
- distinguish Pi evidence from model interpretation;
- keep read-only workflows read-only;
- require a fresh, explicit confirmation before any action that changes Pi state; and
- keep the user-visible name and starter prompt aligned with the skill.

Exact Pi tool names in the skill files are part of the public integration contract. Avoid adding implementation details that are not needed to use those tools safely.

## Validate your changes

Use the validators included with your current Codex installation. `uv` keeps the Python dependency isolated:

```bash
for skill in skills/*; do
  uv run --with pyyaml \
    python ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py "$skill"
done

uv run --with pyyaml \
  python ~/.codex/skills/.system/plugin-creator/scripts/validate_plugin.py .

python -m json.tool .codex-plugin/plugin.json >/dev/null
python -m json.tool .mcp.json >/dev/null
```

Test installation from a temporary local marketplace, use synthetic prompts, and do not trigger write actions against a real Pi workspace merely to test packaging.

Before opening a pull request, read every changed file and check for private information, placeholders, unsupported claims, and missing confirmation steps.
