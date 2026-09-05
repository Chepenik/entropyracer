# Entropy Racer

Entropy Racer is an open-source educational Bitcoin hobby project that explores
how independent randomness sources can be combined for BIP39 mnemonic
generation through interactive gameplay.

> [!WARNING]
> Entropy Racer is experimental, has not been independently audited, and is not
> a substitute for an established hardware-wallet workflow. Do not use it to
> secure meaningful funds without reviewing and validating the implementation.

The application is a single, self-contained HTML file that can be inspected,
saved locally, disconnected from the internet, and opened in a modern desktop
browser without network dependencies.

## Project status

The first playable version is available for review. It includes internal
cryptographic self-tests, but it has not received an independent security audit.

## Run locally

Download [entropy-racer.html](entropy-racer.html), disconnect networking, and
open the file directly in a modern desktop browser. Use the arrow keys to drive
and Space to fire.

No server, installation, build tool, package manager, or network connection is
required. The source, styles, official BIP39 English word list, and game are all
contained in that one file.

The repository's [SHA256SUMS](SHA256SUMS) file can detect accidental changes to
the HTML. A checksum only establishes provenance when you obtain it through a
channel you already trust.

## Security

Please report suspected vulnerabilities privately. Do not include mnemonic
phrases, private keys, or other real secrets in any report. See
[SECURITY.md](SECURITY.md) for the reporting process and threat-model scope.

## Contributing

Contributions are welcome. Security-sensitive changes require tests and a clear
explanation of their assumptions. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Licensed under the [MIT License](LICENSE).
