# Contributing to Entropy Racer

Thank you for helping improve Entropy Racer.

## Before contributing

- Use a public issue for ordinary bugs and feature proposals.
- Follow [SECURITY.md](SECURITY.md) for anything that may affect secrets,
  entropy, mnemonic correctness, or unintended data disclosure.
- Never place a real seed phrase, private key, or wallet secret in an issue,
  test, screenshot, commit, or pull request.

## Design constraints

The final application must remain a single self-contained HTML file. It must
work locally without a build step or network access and must not use remote
scripts, styles, fonts, images, APIs, analytics, or telemetry.

Cryptographic changes must use established browser primitives and BIP39 rules.
Do not introduce custom cryptography or use `Math.random()` for wallet entropy.
Security-critical behavior must fail closed.

## Pull requests

Keep changes focused and explain:

- What changed and why.
- How the change was tested in supported desktop browsers.
- Any security assumptions or threat-model impact.
- Whether the change affects entropy collection, BIP39 conversion, sensitive
  data lifetime, storage, clipboard access, or networking.

Cryptographic changes should include deterministic test vectors or self-tests.
Before submitting, verify that the application makes no network requests and
that no sensitive values are logged or persisted.

By contributing, you agree that your contributions are licensed under the
project's [MIT License](LICENSE).
