<p align="center">
  <a href="https://probecli.com"><img src="assets/banner.svg" alt="PROBE: test hooks, get paid for verified work" width="100%"></a>
</p>

<p align="center">
  <a href="https://probecli.com"><img src="https://img.shields.io/badge/probecli.com-141413?style=flat-square&logo=data:image/svg%2bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAzMiAzMiI+PHBhdGggZD0iTTQuNSA1LjUgTDE2IDEzLjQgTTQuNSAyNi41IEwxNiAxOC42IiBzdHJva2U9IiNGN0Y2RjIiIHN0cm9rZS13aWR0aD0iNSIgZmlsbD0ibm9uZSIvPjxjaXJjbGUgY3g9IjI0LjUiIGN5PSIxNiIgcj0iNC4yNSIgZmlsbD0iI0U4M0YyOCIvPjwvc3ZnPg==" alt="Website"></a>
  <a href="https://verifier.probecli.com"><img src="https://img.shields.io/website?url=https%3A%2F%2Fverifier.probecli.com%2Fhealth&style=flat-square&label=verifier&up_message=live&up_color=e83f28&down_message=down&labelColor=141413" alt="Verifier status"></a>
  <a href="https://robinhoodchain.blockscout.com/address/0x75a7af44fe0117b1f5ff11eddad11fe1e0d34189"><img src="https://img.shields.io/badge/ProbeJobs-0x75a7…4189-e83f28?style=flat-square&labelColor=141413" alt="ProbeJobs contract"></a>
  <a href="https://github.com/probecli/probe"><img src="https://img.shields.io/badge/source-verified-e83f28?style=flat-square&labelColor=141413&logo=github" alt="Source verified"></a>
  <a href="https://x.com/probecli"><img src="https://img.shields.io/badge/@probecli-141413?style=flat-square&logo=x" alt="@probecli on X"></a>
</p>

<br>

**PROBE runs reproducible tests for Uniswap v4 hooks.** Hook teams fund a job on-chain. Operators run the `probe` CLI, where an AI agent proposes test cases against a pinned chain snapshot. A deterministic verifier replays every case, and the contract pays once for each new execution path it reproduces. Passing locally earns nothing; reproducing does.

<br>

<img src="assets/flow.svg" alt="How a job flows: the sponsor funds it, the operator runs the CLI, the verifier reproduces each case, the contract pays once per new path" width="100%">

<br>

### `probe work`, start to finish

<img src="assets/terminal.svg" alt="A probe work session: three cases pass locally; the verifier accepts one, marks one a duplicate and fails one for reading wall-clock time" width="100%">

<sub>Output from a real CLI run on a local test chain with a test token. Mainnet jobs pay in the token the sponsor funds.</sub>

<br>

### Run it

```shell
git clone https://github.com/probecli/probe && cd probe/protocol
npm install && npm link        # Node 22.18+ and Foundry
probe init                     # your operator key; rewards go to its address
probe jobs                     # what's funded on the live verifier
probe work <job>
```

### Live

| | |
|---|---|
| Network | Robinhood Chain mainnet · chain `4663` |
| Contract | [`0x75a7af44fe0117b1f5ff11eddad11fe1e0d34189`](https://robinhoodchain.blockscout.com/address/0x75a7af44fe0117b1f5ff11eddad11fe1e0d34189) · source verified, exact match |
| Verifier | [`verifier.probecli.com`](https://verifier.probecli.com) · `0xd3c3…d746`, approved on-chain |
| Code | [`probecli/probe`](https://github.com/probecli/probe): contract, verifier, CLI, job specs |

<br>

<p align="center">
  <sub><a href="https://probecli.com">probecli.com</a> · <a href="https://probecli.com/operators">Earn as an operator</a> · <a href="https://probecli.com/teams">Fund a job</a> · <a href="https://x.com/probecli">@probecli</a></sub>
</p>
