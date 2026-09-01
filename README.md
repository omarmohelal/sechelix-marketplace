# SecHelix marketplace

The Claude Code plugin marketplace for **[SecHelix](https://github.com/omarmohelal/SecHelix)** —
an evidence-first application-security Agent Skill for authorized repositories and environments.

This repository is intentionally tiny. It contains only the marketplace manifest; the plugin
itself lives in the SecHelix repository.

## Install

```
/plugin marketplace add omarmohelal/sechelix-marketplace
/plugin install sechelix@sechelix
```

## Why a separate repository

Placing `marketplace.json` beside `plugin.json` in the SecHelix repository makes
`claude plugin validate .` stop validating the plugin and check only the marketplace, which
removes the signal the plugin's own CI depends on. Keeping the marketplace here preserves both.

## What you get

SecHelix maps the attack surface, selects only applicable security hypotheses, hunts in parallel
specialist lanes, **independently verifies every material finding and refutes false positives**,
fixes root causes, requires regression proof, and produces an explicit release decision.

Its public benchmark status is `NOT_MEASURED` and the blocker is documented. It makes no accuracy
claim it cannot reproduce.

- Documentation: <https://sechelix.com/docs>
- Source: <https://github.com/omarmohelal/SecHelix>
- License: Apache-2.0
