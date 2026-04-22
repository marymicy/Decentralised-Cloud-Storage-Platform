#  Decentralized Cloud Storage Platform

A robust, blockchain-based file storage ecosystem designed to eliminate centralized points of failure. By utilizing a **Proof-of-Work (PoW)** consensus mechanism and a peer-to-peer architecture, this platform ensures that file metadata is immutable, transparent, and securely managed across a distributed network.

##  Key Features
* **Blockchain Metadata Management**: Every file upload is recorded as a transaction in a block, secured by SHA-256 hashing.
* **Proof-of-Work (PoW)**: Implements a mining consensus to validate blocks, ensuring the integrity of the storage ledger.
* **Peer-to-Peer (P2P) Synchronization**: Nodes communicate to share and validate the longest chain, preventing unauthorized data tampering.
* **Flask-Based Dashboard**: A user-friendly web interface for seamless file uploads and blockchain visualization.
* **Performance Comparison**: Includes scripts to analyze the efficiency of different PoW difficulty levels.

##  The Science: Proof-of-Work (PoW)
To ensure the integrity of the storage ledger, each block must satisfy a difficulty target. The mining process involves finding a **nonce** such that:

$$Hash(Block + Nonce) < Target$$

This prevents attackers from easily modifying historical file records, as they would need to redo the work for all subsequent blocks.

##  Tech Stack
* **Backend**: Python 3.x
* **Web Framework**: Flask
* **Consensus Logic**: Custom Proof-of-Work (PoW)
* **Frontend**: HTML5, CSS3 (Bootstrap), JavaScript
* **Network**: Distributed Peer-to-Peer Ledger

##  Project Structure
* `Blockchain.py`: The core logic for chain management and consensus.
* `Block.py`: Defines the structure and hashing of individual blocks.
* `peer.py`: Handles network communication between different nodes.
* `run_app.py`: Entry point for the Flask web application.
* `/app`: Contains UI templates and static assets (CSS/JS).
* `POW_Comparison.py`: Analysis tool for consensus benchmarking.

##  Getting Started
1. **Clone the repository**:
   ```bash
   git clone [https://github.com/marymicy/Decentralised-Cloud-Storage-Platform.git](https://github.com/marymicy/Decentralised-Cloud-Storage-Platform.git)
