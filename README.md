# WARNING: THIS REPOSITORY IS MALWARE

**Do not download, install, or run anything from this repository or its GitHub Releases.**

This is **not** MetaMask. It is **not** Consensys. Official MetaMask is a **browser extension** from [metamask.io](https://metamask.io/download) and [github.com/MetaMask/metamask-extension](https://github.com/MetaMask/metamask-extension). Consensys does **not** ship a Windows installer named `Metamask.Setup.1.6.0.exe`.

## What this repo does

The `v1.6.0` release (`Metamask.Setup.1.6.0.exe`, plus a macOS `.dmg` and Linux `.AppImage`) is a fake desktop wallet.

If you install it:

1. The UI clones MetaMask onboarding.
2. It asks you to **create or import a wallet**.
3. Your **Secret Recovery Phrase (seed phrase)** and wallet password are written to local storage.
4. A hidden native module (`wallet.node`) downloads a second-stage infostealer from GitHub and injects it into memory.
5. Stolen seeds, browser cookies/passwords, and wallet files are sent off your machine.

**Anyone who entered a seed phrase here should treat that wallet as compromised.** Move funds to a **new** wallet created in official MetaMask (or another wallet you trust), on a clean device. Never reuse that seed.

## Installer (Windows)

| | |
|---|---|
| File | `Metamask.Setup.1.6.0.exe` |
| SHA256 | `520483c5b0dfe213b871ae0b47b4c441388dc62b8b29015e734d47f97878d7fc` |
| Size | 101.83 MB |
| Type | Unsigned NSIS 3.04 Electron installer |
| VirusTotal | 0/67 when last checked (undetected, still malware) |

Related hashes:

- `wallet.node` SHA256 `11e61ae5e63ac08f44fefcd912443fd37615fbe58ecd05ccd0b24ac74584b6e1`
- Stage-2 DLL SHA256 `6b944e8436b715d2b76e0a39b1372b78cc020b62ea2c59778f0f5180fb372abb`

## Related infrastructure

- This GitHub user (`MetaMask-AI`) impersonates MetaMask (logo, `metamask.io`, `@metamask`).
- Predecessor lure account `metamask-eth` (now deleted) shipped the same `v1.6.0` binaries in June 2026.
- Stage-1 payload host: `github.com/ejunmao/settings` file `base`.

This pull request replaces the lure files with this warning. **Delete the Releases** (`Metamask.Setup.1.6.0.exe` / `.dmg` / `.AppImage`) as well; a README change does not unpublish those assets.

Analysis was static only. The sample was not executed.

If you already ran the installer, also rotate browser passwords and assume Chromium cookies may have been stolen.
