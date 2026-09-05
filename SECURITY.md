# Security Policy

Entropy Racer is an experimental educational project involving wallet seed
generation. Security reports are taken seriously, but the project has not been
independently audited and is not recommended for protecting meaningful funds.

## Reporting a vulnerability

Please report suspected vulnerabilities privately through the repository's
[GitHub security advisory form](https://github.com/Chepenik/entropyracer/security/advisories/new).

If private vulnerability reporting is unavailable, open a minimal public issue
asking the maintainer to establish a private contact channel. Do **not** include
exploit details in that issue.

Please include, when applicable:

- A concise description of the vulnerability and its likely impact.
- The affected commit, release, browser, and operating system.
- Reproduction steps or a minimal proof of concept using test data only.
- Whether the issue could expose, bias, reuse, persist, or predict secret data.
- Suggested mitigations, if known.

Never submit a real mnemonic, private key, passphrase, wallet file, address with
private context, or other secret. Maintainers will never ask for seed words.

Please allow a reasonable period for investigation and remediation before
public disclosure. Receipt will be acknowledged when possible, followed by
updates as the issue is assessed. No bounty or compensation program is offered.

## Especially important report areas

Reports are particularly valuable when they involve:

- Weak, biased, predictable, duplicated, or reused entropy.
- Incorrect BIP39 word selection, checksum handling, or validation.
- Secret material reaching storage, logs, URLs, the clipboard, or the network.
- State-reset or race-condition failures that permit duplicate generation.
- Bypasses of cryptographic self-tests or fail-closed behavior.
- Unexpected network requests or unsafe external dependencies.
- Injection vulnerabilities or malicious input reaching security-critical code.
- Incomplete destruction of visible mnemonic material.

## Scope and limitations

The project's security boundary is the published Entropy Racer source. It can
reduce reliance on remote services and a single entropy source, but it cannot
protect users from a compromised operating system, browser, extension,
hardware device, keylogger, screen recorder, modified application copy, poor
backup practice, coerced disclosure, or future cryptographic failures.

For meaningful Bitcoin holdings, use established, independently reviewed
hardware-wallet and backup workflows.

## Supported versions

Until stable releases are published, only the latest commit on `main` is
considered for security fixes. Older commits and modified copies are unsupported.
