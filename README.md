BlockDocsChat System

BlockDocsChat System is an integrated blockchain-based application that combines a secure chat system and a decentralized document sharing system using IPFS. A central homepage is used only for navigation, while all modules run independently without modifying their original frontend or logic.

PROJECT MODULES

1. BlockHomepage
Central homepage for navigation and redirection.

2. BlockChatGem
Blockchain-based secure chat application using Ethereum smart contracts.

3. BlockDocsGem
IPFS-based decentralized document sharing system built using Python and Flask.

FOLDER STRUCTURE

BlockDocsChat-System
- BlockHomepage
- BlockChatGem
- BlockDocsGem
- README.md

TECHNOLOGIES USED

Frontend:
React.js, Vite, TypeScript, Tailwind CSS

Blockchain:
Solidity, Hardhat, Ethereum (Localhost), MetaMask

Backend:
Python 3.10.11, Flask, Flask-CORS

Decentralized Storage:
IPFS (Local daemon)

Tools:
VS Code, Git, GitHub, NVM, Python Virtual Environment

PREREQUISITES

Node.js (18.x and 22.x)
NVM
Python 3.10.11
IPFS
Git
VS Code

HOW TO RUN THE PROJECT

STEP 1: Start IPFS
Command:
ipfs daemon

STEP 2: Run Document Sharing Backend
cd BlockDocsGem/main_server
py -3.10 -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python server.py

Runs on: http://127.0.0.1:5111

STEP 3: Run Document Sharing UI
cd BlockDocsGem/client_server_1
py -3.10 -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python server.py

Runs on: http://127.0.0.1:5113

STEP 4: Run Blockchain Chat Backend
cd BlockChatGem/web3
nvm use 18.17.1
npm install
npm run compile
npm run node

STEP 5: Deploy Smart Contracts
npm run deploy-local

STEP 6: Run Chat Frontend
cd BlockChatGem
nvm use 22.14.0
npm install
npm run dev

Runs on: http://localhost:3001

STEP 7: Run Homepage
cd BlockHomepage
nvm use 22.14.0
npm install
npm run dev

Runs on: http://localhost:5173

APPLICATION URLs

Homepage: http://localhost:5173
Document Sharing UI: http://127.0.0.1:5113
Document Backend API: http://127.0.0.1:5111
Chat Application: http://localhost:3001

SYSTEM FLOW

User opens the homepage.
User selects Chat or Document Sharing.
Homepage redirects to the selected module.
Each module runs independently.

KEY FEATURES

Modular architecture
Blockchain-secured chat
IPFS-based decentralized storage
Python virtual environment usage
Beginner-friendly setup

VIVA EXPLANATION

BlockDocsChat System integrates a blockchain-based chat application and an IPFS-based document sharing system using a centralized homepage while preserving modular and independent deployments.

AUTHOR

Developed by Gemini G
