# vote-app

A voting dApp frontend built with Next.js, TypeScript, Tailwind CSS, Firebase and Web3 integrations.

This repository contains the frontend for a voting application (UI + authentication + blockchain/web3 hooks). It uses the Next.js App Router and follows modern React + TypeScript patterns.

## Key features

- Next.js (App Router) + TypeScript
- Tailwind CSS for styling
- Firebase for authentication and backend integration
- Ethers/Web3 for blockchain interactions
- Minimal, well-structured routes under `src/app`

## Tech stack

- Next.js 15+ (App Router)
- React 19+
- TypeScript
- Tailwind CSS
- Firebase
- ethers / web3

## Quick start

Prerequisites:
- Node.js 18+ (recommended)
- npm, pnpm or yarn

1. Install dependencies

```powershell
npm install
```

2. Create an `.env.local` file at the project root and add the required environment variables (examples below).

3. Run the dev server

```powershell
npm run dev
```

Open http://localhost:3000 in your browser.

## Important environment variables (examples)

Create `.env.local` and populate values used by `src/lib/firebase.js` and `src/lib/web3*`:

- NEXT_PUBLIC_FIREBASE_API_KEY=
- NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=
- NEXT_PUBLIC_FIREBASE_PROJECT_ID=
- NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=
- NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=
- NEXT_PUBLIC_FIREBASE_APP_ID=
- NEXT_PUBLIC_RPC_URL=    # RPC endpoint for web3 (e.g. Infura/Alchemy)
- NEXT_PUBLIC_CONTRACT_ADDRESS=

Note: The repo uses `NEXT_PUBLIC_` prefix for variables needed in the browser.

## Available scripts

- `npm run dev` — run development server (Next.js)
- `npm run build` — build for production
- `npm run start` — start production server
- `npm run lint` — run ESLint

## Firebase & Web3 notes

- Firebase configuration and initialization live in `src/lib/firebase.js`.
- Blockchain interactions are handled in `src/lib/web3-integration.ts` and `src/lib/web3.ts`. Review and configure RPC/contract addresses in environment variables before using.

## Contributing

If you'd like to contribute, please:

1. Fork the repo
2. Create a feature branch
3. Open a pull request with a clear description

Keep changes small and focused. Add tests where appropriate.

## License

This project does not include a license file. Add one if you intend to publish under an open-source license.

---

If you'd like any specific content added to this README (screenshots, architecture diagram, deployment steps, CI, or contributor rules), tell me what to include and I can update it.
