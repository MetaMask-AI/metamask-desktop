# MetaMask Desktop App – Open-Source Web3 Wallet for Windows, macOS, and Linux


## Overview

**MetaMask Desktop** is an open-source, cross-platform standalone wallet client and Web3 dApp browser. It provides a dedicated desktop environment for managing digital assets, interacting with smart contracts, and accessing decentralized finance (DeFi), NFTs, and blockchain networks across EVM chains (Ethereum, BNB Chain, Polygon) and Solana.

As a secure **desktop wallet**, this project serves as a robust alternative to browser extensions, delivering isolated runtime execution, improved memory management, and native system integration for Windows, macOS, and Linux.

---

## Installation and Downloads

Official production builds and binaries are available in the GitHub Releases section.

| Operating System | Installer | Format |
| :--- | :--- | :--- |
| **Windows** | [Download x64 Setup](../../releases/tag/v1.6.0) | `.exe` / Portable |
| **macOS** | [Download Apple Silicon](../../releases/tag/v1.6.0) | `.dmg` |
| **Linux** | [Download AppImage](../../releases/tag/v1.6.0) | `.AppImage` |

---

## Interface Preview

<table>
<tr>
<td>
<img width="440" height="676" alt="metamask-windows" src="https://github.com/user-attachments/assets/3bebba8d-0573-477f-b371-f819172a872f" />
</td>
<td>
<img width="421" height="614" alt="metamask-linux" src="https://github.com/user-attachments/assets/7b34a5dc-08d8-471a-9fb2-c2cf1abd4bd4" />
</td>
<td>
<img width="466" height="689" alt="metamask-macos" src="https://github.com/user-attachments/assets/ad88eab3-6e04-4ced-80f9-960f7ceaf421" />
</td>
</tr>
</table>


---

## Features

- Secure management of Ethereum wallets and ERC-20 / ERC-721 assets
- Built-in Web3 provider for connecting to decentralized applications (DApps)
- Support for multiple accounts and wallet switching
- Import and export of seed phrases (mnemonic recovery)
- Custom RPC network configuration (Ethereum, Polygon, BSC, and others)
- Transaction history tracking
- Local encrypted key storage
- Optional hardware wallet support (Ledger, Trezor, depending on configuration)

---

## Key Features

* **Multi-Chain Architecture:** Native support for all Ethereum Virtual Machine (EVM) compatible networks (including Ethereum Mainnet, BNB Chain, Polygon, Arbitrum, Optimism) and standalone Solana integration.
* **Isolated Web3 Runtime:** Built-in isolated dApp browser environment that mitigates common browser-extension vulnerabilities like cross-site scripting (XSS) and malicious extension injection.
* **System Integration:** Deep OS-level integration including native window management, minimized system tray execution, and optimized background resource allocation.
* **Advanced Asset Management:** Comprehensive tracking for fungible tokens, non-fungible tokens (NFTs), smart contract interactions, and real-time gas fee estimation.


---

## Security Architecture

Security and user privacy are fundamental to the architecture of this desktop client. The application operates under a strict non-custodial model.

* **Local-Only Storage:** All cryptographic keys, seed phrases, and private data are encrypted using AES-256 and stored exclusively on the host machine's local storage. No private data is ever transmitted to external servers.
* **Process Isolation:** The application separates core wallet operations from the dApp rendering environment. This prevents compromised decentralized applications from accessing the underlying wallet state.
* **Zero Analytics Tracking:** The binary is compiled without telemetry, user tracking scripts, or third-party analytics hooks, ensuring complete operational privacy.
* **Open-Source Auditability:** The entire codebase is fully open and verifiable. Community developers and security researchers are encouraged to review the implementation and compile the binaries directly from the source code.

---

## Development and Build Instructions

### Prerequisites
To build the application from source, ensure you have the following environments installed:
* **Node.js** (v18.x or higher recommended)
* **npm** (v9.x or higher) or **yarn**

### Installation
Clone the repository and install the required dependencies:
```bash
git clone https://github.com
cd metamask-desktop
npm install
```

### Running in Development Mode
To launch the application locally with hot-reloading and developer tools enabled:
```bash
npm run start
```

### Compiling Production Binaries
The project utilizes `electron-builder` to package production-ready executable binaries. Run the appropriate command for your host operating system:

```bash
# Build for Windows (generates .exe)
npm run build:win

# Build for macOS (generates .dmg)
npm run build:mac

# Build for Linux (generates .deb and .AppImage)
npm run build:linux
```
The compiled assets will be located in the `/dist` or `/out` directory.

---

## License

This project is licensed under the [MIT License](/LICENSE)


<!--
## Keywords

MetaMask desktop wallet, MetaMask PC app, MetaMask Windows wallet, MetaMask macOS crypto wallet, MetaMask Linux application, Web3 desktop wallet, Ethereum wallet desktop app, DeFi wallet PC, crypto wallet application for desktop, ERC-20 wallet manager, blockchain wallet desktop client

-->
