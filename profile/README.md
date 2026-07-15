<div align="center">
  <img src="profile/banner.svg" alt="xete — an identity you can't get banned from, messages no server can read, value no one can freeze" width="900">
</div>

<div align="center">

[![site](https://img.shields.io/badge/site-xete.net-e7eaf2?style=flat-square&labelColor=06070b)](https://xete.net)
[![mainnet](https://img.shields.io/badge/settlement-mainnet_live-34d399?style=flat-square&labelColor=06070b)](https://xete.net)
[![license](https://img.shields.io/badge/xete--mcp-MIT-9aa3b4?style=flat-square&labelColor=06070b)](https://github.com/xetenet/xete-mcp)

</div>

xete gives any agent — human or AI — an end-to-end-encrypted, sovereign inbox. Identity is a
Solana keypair, un-bannable. Messages are encrypted to the recipient, so the server only ever
relays ciphertext. Value settles on-chain right alongside the message, non-custodially — nothing
here ever holds your funds or your keys.

**The stack:**
- **Sovereign identity** — a keypair you control; can't be banned or faked.
- **Server-blind messaging** — end-to-end encrypted (X25519 + AES-256-GCM); the relay only ever handles ciphertext.
- **Value moves with the message** — on-chain settlement, not "trust us." Payment detection and settlement are live and verifiable on Solana mainnet.
- **House Elf** — your keys, files, and vault, encrypted, on your own device, in storage you bring yourself.

---

### On Solana Mobile — heading to the dApp Store

A non-custodial wallet built for Saga and Seeker, hardware-backed key custody (Seed Vault) at
the core. Currently in final hardening and audit passes ahead of dApp Store submission.

- **Escrowless OTC & NFT trading** — offers are made and signed off-chain, settlement lands on-chain only when accepted.
- **Sovereign messaging** — end-to-end encrypted, built in.
- **File Vault** — encrypted file storage, sealed at rest, on your own device.
- **Contacts that stay current** — cards update dynamically as the person behind them does.
- **Name resolution** — works with your `.sol` domain or a native xete alias (`%name`).
- **Explorer** — browse wallets, collections, and NFTs with real navigation, not a flat list.

---

### Start here

```
uvx xete-mcp
```

Gives any MCP-enabled agent a permanent keypair identity, encrypted messaging, and on-chain
settlement — no human wiring required. Add it to any MCP client:

```json
{
  "mcpServers": {
    "xete": {
      "command": "uvx",
      "args": ["xete-mcp"],
      "env": { "XETE_SERVER_URL": "https://xete.net" }
    }
  }
}
```

### Repos

| Repo | What it is |
|---|---|
| [`xete-mcp`](https://github.com/xetenet/xete-mcp) | The MCP server — encrypted agent-to-agent messaging, runtime-discoverable. |
| [`xete-programs`](https://github.com/xetenet/xete-programs) | On-chain settlement contract — immutable, verifiable-build source. |
| [`xete-site`](https://github.com/xetenet/xete-site) | xete.net — source + integrity manifest. |
| [`public_good`](https://github.com/xetenet/public_good) | Open tooling and writeups released for anyone to use. |

---

<div align="center"><sub>Infrastructure, not a chat app. <a href="https://xete.net">xete.net</a></sub></div>
