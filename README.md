# CortexRelay

**The Sync & Backup Engine for the Cortex-Works Ecosystem**

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
* **One-Click Local Backup:** ระบบบีบอัดฐานข้อมูล Local เพื่อ Backup หรือย้ายเครื่องได้ง่ายๆ ไร้รอยต่อ.
* **CRDT-based Team Collaboration:** ใช้เทคโนโลยี CRDTs (Conflict-free Replicated Data Type) อย่าง Automerge/Loro เพื่อซิงค์ฐานข้อมูล (Tickets/Status) ระหว่างเครื่องในทีมแบบ Peer-to-Peer โดยไม่ทำให้ Data พัง.
