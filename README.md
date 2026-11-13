# AY Inbox Homebrew tap and Scoop bucket

Package manager manifests for `ayinbox`, the command line tool for [AY Inbox](https://ayinbox.com), a hosted cold email platform.

AY Inbox is a hosted service. This repository holds the Homebrew formula and Scoop manifest for the CLI's release binaries, which are published on [ayinbox/ayinbox-cli](https://github.com/ayinbox/ayinbox-cli/releases). The service itself is not open source.

## Homebrew (macOS and Linux)

```bash
brew install ayinbox/tap/ayinbox
```

Upgrade with `brew upgrade ayinbox`.

## Scoop (Windows)

```powershell
scoop bucket add ayinbox https://github.com/ayinbox/homebrew-tap
scoop install ayinbox
```

Upgrade with `scoop update ayinbox`.

## Then

```bash
ayinbox auth login
ayinbox campaign list
```

Documentation: https://docs.ayinbox.com/api/cli/

## How this repository is updated

`Formula/ayinbox.rb` and `bucket/ayinbox.json` are generated together with the release archives, so their checksums always match what they describe. A maintainer commits them here for every release. Do not edit them by hand. Until the first release exists, both files are placeholders and the install commands above will fail.

## Licence

The files in this repository are MIT licensed (see [LICENSE](LICENSE)). The `ayinbox` binaries they install are proprietary and free to use with an AY Inbox account; their licence is in [ayinbox/ayinbox-cli](https://github.com/ayinbox/ayinbox-cli/blob/main/LICENSE).
