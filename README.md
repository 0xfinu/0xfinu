# 0xfinu

![0xmuse logo](https://raw.githubusercontent.com/0xfinu/finu.muse/main/0xmuse-logo-160x160.jpg)

**finu.muse — 0xfinu + muse, building on testnets for zero real money: an ERC-20 token with real DEX pools, a spam sniper in training, and a multichain burner wallet set — every step verified onchain.**

🌐 [Live site — finu.muse](https://0xfinu.github.io/finu.muse/)

> DYOR, don't trust — verify, not your keys, not your coins.

---

Crypto enthusiast, developer, and creator — airdrops, testnets, bug fixes, bounty programs. The whole testnet programme is practice for a mainnet sniper launch; airdrops and rewards are a bonus, not the goal. Testnet first, free only, no KYC, no subscriptions.

## Tokens

All ERC-20, 1,000,000 supply, 18 decimals.

| Token | Chain | Contract |
| --- | --- | --- |
| STEST | Arc testnet | `0x2B1FB6394461bb9578cDd40fda5C07E774FB4804` |
| STEST | Robinhood Chain testnet | `0x2B1FB6394461bb9578cDd40fda5C07E774FB4804` |
| STEST | LiteForge testnet | `0x34fF4f6F184903d7b5d28de3bcF670FB3E71a073` |

Pools: STEST/USDC on Arc at `0x78dba0e6bf972f9d68732bbf20bd5e0d9888612b` (seeded 10,000 STEST + 10 test USDC); STEST/WETH on Robinhood at `0x0fF18427301c124115476975fF00a6C6B175Cd09` (seeded 10,000 STEST + 0.001 test WETH). LP tokens stay in the burner wallet — never locked, never burned. A 10% test-remove passed on both chains before the run.

## Sniper

Testnet-only buy/sell volume bot, trained on our own token's pools. The run: **1,000 transactions per chain — 2,000 total** — under hard gas quotas the runner cannot cross: 6.66666 test USDC on Arc, 0.00333 test ETH on Robinhood. Launched Nov 16, 2026. Liquidity removal is the final step of the run.

## Repos

| Repo | What it is |
| --- | --- |
| [finu.muse](https://github.com/0xfinu/finu.muse) | This website — the public record of the work |
| [finu-sniper](https://github.com/0xfinu/finu-sniper) | Spam sniper bot + pair watcher (testnet only) |
| [finu-tokens](https://github.com/0xfinu/finu-tokens) | STEST ERC-20 + pools + 0xmuse logo NFT |
| [finu-wallet](https://github.com/0xfinu/finu-wallet) | Multichain burner wallets — one mnemonic, all chains |
| [finu-circle-wallet](https://github.com/0xfinu/finu-circle-wallet) | Circle Arc testnet USDC claim script |

## Wallets (public addresses only — never seed phrases or private keys)

- **Burner wallet set** — one mnemonic derives all four chains: EVM `0xBb87bD789Ca67562F531685e10EB78eC03dE3dEB` · BTC SegWit `bc1qcvhkqg530t5qhjjgcvcvs2mgsqcsn6vexn4l9x` · BTC testnet `tb1qqc2egd574c5rvqpc8jfe805mvpwhtl70705vwx` · Solana `AYKM6NXM6ucPgCMnqWSdPgPe7WaCRtKJ31z7ePjjpbzt` · TRON `TP1TKuV4vj6WtDUkWpDVESvEyJHMbP6aaH`
- **Circle agent wallet** — Arc testnet only, `0xf1bfee7392a18cd9927b84e26560819c4676ae27`. Its only job: draw testnet USDC from the Circle faucet; funds move straight to the burner.

## Chains

| Chain | ID | Status |
| --- | --- | --- |
| Arc testnet | 5042002 | STEST + USDC pool live |
| Robinhood Chain testnet | 46630 | STEST + WETH pool live |
| LitVM LiteForge testnet | 4441 | STEST deployed via Token Factory |

## DYOR

Airdrop and reward hunting runs on one feed and three rules — rewards are a bonus, the reps are the point. Signal feed: Telegram [@airdropfind](https://t.me/s/airdropfind) (~513K subscribers). The feed is uncurated — every post gets verified before anything is touched. **Impersonator warning:** @AirdropFindTeam is a different channel.

- **Verify, don't trust.** Read the contract, source, creator and holders on the explorer before a single transaction.
- **Not your keys, not your coins.** Agent wallets are MPC with tiny caps; the burner holds testnet value only; a seed phrase is never typed anywhere a stranger suggests.
- **Free or nothing.** No subscriptions, no KYC, no paying to unlock an "airdrop."

## Side quest · the Bitcoin Puzzle

The famous 2015 puzzle is real and still open: **77 unsolved addresses holding ~903 BTC**, re-verified onchain Nov 15, 2026. Two engines hunt from the VM — a random key scanner weighted by expected value, and a Pollard's Kangaroo solver working inside puzzle #140's range. It's a lottery ticket, not a plan — and if a key ever lands, the claim goes through a private relay, never the public mempool.

---

*Built by 0xfinu + finu.muse. Testnet only — no real money, no mainnet funds.*
