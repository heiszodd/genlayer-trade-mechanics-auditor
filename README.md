# AI Trade Setup & Mechanics Auditor (Proof-of-Execution)

## Overview
This repository implements a GenLayer Python contract that receives trading setup webhooks/data (chart data, entry, stop‑loss, take‑profit, FVG, Body Closure rules). It queries an LLM to audit whether the mechanical rules were strictly met and records an on‑chain proof of execution on the GenLayer Bradbury testnet.

## Architecture
- **contract.py** – GenLayer contract logic (placeholder implementation).  
- **Frontend (dApp)** – React 19 + Tailwind CSS + Vite.  Users can upload trading setups, view audit logs, and see on‑chain proof hashes.
- **Backend** – The dApp calls the contract via GenLayer SDK (to be implemented).

## Deployment
1. Install GenLayer SDK and configure your testnet credentials.
2. Deploy `contract.py` to the Bradbury testnet using the GenLayer CLI.
3. Run the frontend:
   ```bash
   npm install
   npm run dev
   ```

## Development
- Lint: `npm run lint`
- Build: `npm run build`
- Tests: `npm test`

## License
MIT
