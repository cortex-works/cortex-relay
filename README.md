# CortexRelay

**The Sync & Backup Engine for the Cortex-Works Ecosystem**

> [!WARNING]
> **🚧 Alpha Version (Under Active Development)**
> This project is currently in early alpha stage and is undergoing heavy development. Features, APIs, and CLI commands are subject to breaking changes without notice. 
> 
> **Current Testing Environment (As of 25 Feb 2026):**
> Testing is exclusively performed on a developer machine running **macOS Sequoia 15.7.4** with the latest versions of compatible IDEs (Cursor/VS Code/Windsurf). 
> 
> *If you are cloning this repository to run on Windows, Linux, or older IDE versions, you may encounter instability or broken features. Cross-platform testing will be expanded in future releases.*

## 🌟 Overview
CortexRelay manages personal backup and team collaboration (multi-player) for CortexDB and CortexSync artifacts seamlessly without breaking local-first priorities.

### 🔌 Core Capabilities
* **Personal Mode (Backup):** Facilitates one-click backup of the local SQLite and LanceDB files (`~/.cortexast/data/`). Automates ZIP creation and cloud storage upload (Google Drive, S3) allowing for seamless workstation migration.
* **Team Mode (CRDT-based Sync):** Enables peer-to-peer data synchronization across different agent nodes (e.g. using Automerge or Loro) safely. Prevents database conflicts during synchronous multi-user editing or Scrum ticket execution, mimicking the smooth real-time sync of platforms like Figma or Linear.

## 🏛️ Concept
Part of the "Data Triad" Architecture within Cortex-Works:
1. `CortexSync` - Network events, IDE watchers and Agent interactions.
2. `CortexDB` - Local-first database storage (SQLite + LanceDB).
3. **`CortexRelay` (This Repo)** - Seamless synchronization and data persistence routing.

## 🚀 Phase 3 & 4 Roadmap
This module corresponds to the **Phase 4** and CRDT sync objectives:
* **One-Click Local Backup:** Local database compression system for seamless zero-friction backups and machine migrations.
* **CRDT-based Team Collaboration:** Leverage CRDTs (Conflict-free Replicated Data Type) like Automerge/Loro to sync databases (Tickets/Status) peer-to-peer between team machines without corrupting data.
