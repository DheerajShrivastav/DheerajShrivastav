# Dheeraj Shrivastav

**Software engineer building AI agents and backend services in production.** Maharashtra, India.

At work I build a [real-time voice AI agent](https://dheerajshrivastav.me/projects/voice-agent) on Gemini Live that patients and doctors talk to in any language, with strict guardrails and doctors reviewing reports before they reach patients. On my own I'm building [DappDrop](https://dapp-drop.dheerajshrivastav.me), an on-chain rewards protocol.

[Website](https://dheerajshrivastav.me) · [Resume](https://dheerajshrivastav.me/resume/Dheeraj-Shrivastav-Resume.pdf) · [LinkedIn](https://www.linkedin.com/in/dheerajshrivastav/) · [X](https://x.com/Dheeraj_08_) · [Email](mailto:dheerajshrivastav08@gmail.com)

---

## What I'm building

### [DappDrop](https://github.com/DheerajShrivastav/Dapp-Drop-Smart-Contract): Sybil-resistant on-chain rewards protocol (founder, pre-launch on Sepolia)
Projects run reward campaigns, participants complete verified tasks, and escrowed ERC-20/721/1155 rewards settle via Merkle proofs.
- Protocol and security model: escrow, Merkle settlement with a 24h dispute window, a fallback settler, and satellite modules to stay under the 24 KB EIP-170 limit.
- 240 unit + 26 invariant tests with Slither/Aderyn gates. An escrow-solvency invariant caught a high-severity cross-campaign fund drain on the dev branch, before launch. The full log is in [`docs/SECURITY_FINDINGS.md`](https://github.com/DheerajShrivastav/Dapp-Drop-Smart-Contract/blob/dev/docs/SECURITY_FINDINGS.md).
- Off-chain: EIP-712 attestation signer, SIWE auth, The Graph subgraph with RPC fallback, keeper worker. [App repo](https://github.com/DheerajShrivastav/DappDrop-FrontEnd).
- Built with AI coding agents behind a verification gate I set up; I own the architecture and security decisions.

### [AWS Deploy AI](https://github.com/DheerajShrivastav/aws-deploy-ai): natural-language AWS deployments
An MCP server + Next.js app that analyzes a GitHub repo with AWS Bedrock (Claude) and deploys it to S3 + CloudFront or Lambda. TypeScript.

### [Latch](https://latch.netlify.app/): real-time multiplayer browser game (hackathon, team of 4)
I built the Socket.io multiplayer layer: movement sync, server-side combat and health, and animation state.

### [Event Horizon](https://github.com/DheerajShrivastav/decentralized-grant-program-dapp): AI-assisted grants (Base hackathon, team of 3)
A Groq-hosted LLM scores grant proposals; a Foundry-tested contract pays the approved ones.

## Open source

**[jam-nodes](https://github.com/wespreadjam/jam-nodes)** (wespreadjam, workflow-automation framework): 5 contributions merged
- Dev.to integration with 27 tests ([d5137d8](https://github.com/wespreadjam/jam-nodes/commit/d5137d8))
- WordPress integration ([6269fc7](https://github.com/wespreadjam/jam-nodes/commit/6269fc7))
- Webhook trigger node ([#48](https://github.com/wespreadjam/jam-nodes/pull/48))
- Rate limiter with fixed and sliding-window strategies ([#49](https://github.com/wespreadjam/jam-nodes/pull/49))
- DataForSEO extended operations ([#51](https://github.com/wespreadjam/jam-nodes/pull/51))

## Stack

**AI:** Gemini Live, Claude, AWS Bedrock, Groq, voice agents, AI agents, guardrails, MCP
**Backend:** TypeScript, Node.js, NestJS, Express, Bun, Socket.io, Prisma, PostgreSQL, Redis
**Web3:** Solidity, Foundry, EIP-712, Merkle proofs, The Graph, ethers.js, viem
**Infra:** Docker, GitHub Actions, AWS, Vercel, Azure
