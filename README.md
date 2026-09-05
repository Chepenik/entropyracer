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
open the file directly in a modern desktop browser. Use Up Arrow to accelerate,
Down Arrow to brake or reverse at low speed, Left/Right Arrow to steer and
drift, and Space to fire. The game pauses when focus leaves it; return and press
an Arrow key or Space to continue.

During each endless run, rotating micro-objectives point toward entropy gates,
hash-chain checkpoints, moving target formations, drift zones, and near-miss
opportunities. Temporary rapid-laser, wide-shot, and thrust boosts build a
score-only “chaos flow” combo. Score, combos, objectives, event counts, and the
collection percentage are gameplay/collection metrics—not claimed entropy bits.

Optional physical input accepts Heads = 0 and Tails = 1. For a fair die, 1 =
00, 2 = 01, 3 = 10, and 4 = 11; 5 and 6 are deliberately rejected and require
another roll. This rejection sampling avoids bias. Record every outcome honestly
and in order; the software cannot verify the physical process.

No server, installation, build tool, package manager, or network connection is
required. The source, styles, official BIP39 English word list, and game are all
contained in that one file.

The repository's [SHA256SUMS](SHA256SUMS) file can detect accidental changes to
the HTML. A checksum only establishes provenance when you obtain it through a
channel you already trust.

Seeing `file://` in the address bar does not prove that networking is
disconnected. The application makes no automatic network requests, but the
browser, extensions, operating system, and other software remain outside its
security boundary. Established hardware-wallet workflows remain preferable for
meaningful funds.

## Security

Please report suspected vulnerabilities privately. Do not include mnemonic
phrases, private keys, or other real secrets in any report. See
[SECURITY.md](SECURITY.md) for the reporting process and threat-model scope.

## Contributing

Contributions are welcome. Security-sensitive changes require tests and a clear
explanation of their assumptions. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Licensed under the [MIT License](LICENSE).
