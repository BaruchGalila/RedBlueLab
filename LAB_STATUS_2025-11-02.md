# Blue & Red Cyber Lab — Status Log

**Date:** 2025-11-02
**Snapshot state:** Stable baseline after network recovery
**Snapshots created:**
- Kali — pre-experiment-2025-11-02-Kali
- Windows 10 — pre-experiment-2025-11-02-Win10
- Windows Server (SRV1) — pre-experiment-2025-11-02-SRV1

**Network:**
- Kali connected to Internet (via NAT)
- Kali -> Win10: reachable (ping OK)
- Kali -> SRV1: check
- Note: Kali has Internet but is not fully connected to both other VMs for all services.

**Shared Folder:**
- /mnt/hgfs/VMShared mounted on Kali

**Git Sync:**
- Repo: https://github.com/BaruchGalila/RedBlueLab

**Next steps:**
1. Reconnect VMs internally.
2. Start tcpdump / capture tests.