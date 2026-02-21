🎓 Blockchain-Based Academic Certificate Verification System
📌 Overview
This project is a blockchain-powered academic certificate verification platform designed to combat certificate forgery, document tampering, and inefficient manual verification processes.
The system leverages Ethereum smart contracts to create tamper-proof certificate records while storing certificate data off-chain for efficiency and scalability. Each issued certificate is cryptographically secured and verifiable through hash integrity checks.
The platform enables institutions to issue certificates securely and allows employers to independently verify authenticity without relying on manual confirmation.

🎯 Objectives
This project was developed to:
1.	Design a secure platform for issuing and verifying academic certificates using blockchain technology.
2.	Prevent certificate forgery and document tampering.
3.	Eliminate long and inefficient manual verification processes.
4.	Store certificate records securely using blockchain-backed integrity mechanisms.

🏗 System Architecture
🔹 On-Chain Components
•	Ethereum smart contracts written in Solidity
•	Stores certificate hash references and wallet address associations
•	Provides immutable verification records
🔹 Off-Chain Components
•	Certificate data stored off-chain
•	Hash of certificate generated (SHA-based integrity check)
•	Hash stored on blockchain to ensure tamper-proof validation
🔹 Roles in the System
•	Admin – Manages system configuration and institutional access
•	Institution Registrar – Issues certificates to students
•	Employer – Verifies certificate authenticity by checking hash integrity
•	Student – Receives certificate associated with a wallet address
Each certificate is linked to a unique wallet address, enabling secure identity association.

🔐 Verification Mechanism
1.	Certificate is issued by the registrar.
2.	A cryptographic hash of the certificate is generated.
3.	The hash is recorded on the Ethereum blockchain.
4.	Employers verify certificate authenticity by:
o	Recomputing the certificate hash
o	Comparing it against the on-chain stored hash
5.	If hashes match → certificate integrity is confirmed.
This ensures:
•	Tamper detection
•	Transparency
•	Trustless verification

🛠 Technology Stack
Blockchain Layer
•	Ethereum
•	Solidity Smart Contracts
•	Hardhat (Development & Testing)
•	MetaMask (Wallet Integration)
•	Web3.js
Backend
•	Node.js
•	JavaScript
•	PostgreSQL (initially MongoDB, later migrated)
Frontend
•	React.js

🔒 Security Considerations
•	Certificates are not stored fully on-chain to reduce cost and improve scalability.
•	Only certificate hashes are stored on-chain to guarantee immutability.
•	Wallet-based association ensures identity linkage.
•	Hash comparison prevents document tampering.
•	Role separation (Admin / Registrar / Employer/Student) reduces misuse risk.

🚀 How It Works (High-Level Flow)
1.	Registrar logs into the system.
2.	Certificate details are submitted.
3.	System generates a cryptographic hash.
4.	Hash is recorded on Ethereum via smart contract.
5.	Student receives certificate linked to wallet address.
6.	Employer verifies by comparing hash with on-chain record.

📎 Repository
This repository is a fork of the original group project.
It is maintained here to highlight my contributions and backend leadership role.
