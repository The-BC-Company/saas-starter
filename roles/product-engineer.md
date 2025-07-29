# Frontend Engineer aka Product Engineer

## Role

At our company, frontend engineers architect, implement, and deploy user interfaces end-to-end to make blockchain data universally accessible.

Depending on your interests, this might mean building real-time data visualization systems, crafting intuitive search interfaces for complex blockchain queries, or obsessively optimizing performance for millions of concurrent users. Perhaps it involves solving interface problems not yet conceived of in the blockchain space.

## What You'll Build

You'll craft interfaces that handle real-time blockchain data streams, build sophisticated search and filtering systems, and create visualizations that make sense of complex on-chain activity. You'll work directly with Next.js, React, and TypeScript to build experiences that serve both crypto natives and mainstream users.

Core technologies: Next.js, React, tRPC, TypeScript, Tailwind CSS, D3.js, WebGL for high-performance graphics.

## Requirements

- 3+ years building production React applications
- Deep Next.js expertise (SSR, SSG, performance optimization)
- Strong TypeScript and modern JavaScript skills
- Experience with real-time data visualization and/or streaming data
- Experience with keyboard heavy user interaction
- Understanding of web performance and scalability

Bonus: blockchain/crypto experience, WebGL/Canvas, data visualization libraries.

## Task

### Pick one

1. build a result table with virtualization & infinite scrolling  
   - TanStack Table + TanStack Virtual (MIT)  
   - react-window / react-virtualized  
   - SWR or React Query for paged fetching  
   - MirageJS for quick mock API

2. build a Cmd+K dialog with 2 pages that allows shortcut search  
   - kbar or cmdk (MIT) for command palette  
   - Radix UI primitives for accessibility & focus management  
   - Fuse.js for local fuzzy search or Algolia DocSearch (free tier)

3. create a live-updating blockchain throughput chart with D3.js and Tailwind controls  
   - D3.js or Recharts / Nivo for charting  
   - use-websocket or socket.io-client (MIT) for live data  
   - ethers.js or viem + free RPC (Alchemy/Ankr)  
   - Tailwind CSS for styling

4. implement a drag-and-drop wallet list with validation and balance fetch via tRPC  
   - dnd-kit or react-beautiful-dnd for drag-and-drop  
   - tRPC + zod for type-safe API & validation  
   - wagmi or viem to read wallet balances  
   - Generate mock addresses with `ethers.Wallet.createRandom()` (loop for N)  
   - Hardhat/Foundry local node comes with 20 prefunded test wallets  
   - Ganache CLI `ganache -d` seeds deterministic wallets you can drag-drop  
   - Pull real testnet wallets via Etherscan/Covalent free API if you want non-random data

5. add a keyboard friendly dark / light theme toggle that persists across sessions  
   - Tailwind CSS dark-mode classes + `next-themes` (MIT)  
   - localStorage or cookies for persistence  
   - Headless UI or Radix Toggle for accessible switch

### Evaluation
- Quantitative (50%)
  - Correctness & functionality: 25 pts
  - Performance metrics (FPS, load time, Lighthouse): 10 pts
  - Automated tests & type-safety coverage: 15 pts
- Qualitative (35%)
  - Code readability & architectural choices: 15 pts
  - UX polish & visual design alignment: 10 pts
  - Communication of trade-offs during interview: 10 pts
- AI Tool Use (15%)
  - Effective, transparent use of AI/code-gen tools: 5 pts
  - Quality of prompts & commit messages referencing AI: 5 pts
  - Critical thinking overriding incorrect AI suggestions: 5 pts