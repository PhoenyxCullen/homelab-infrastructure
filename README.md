# Personal Infrastructure Lab

## Active Projects

### 1. Qubes OS Security Learning Platform (System76 Bonobo WS)

**Hardware:**
- Intel Core i9-14900HX (24 cores)
- 64GB DDR5 RAM
- Dual GPUs: Intel UHD (dom0) + NVIDIA RTX 4080 Mobile
- 3x 3.6TB NVMe SSDs (10.8TB total NVMe capacity)
- System76 Bonobo WS workstation

**Storage:**
- 3x 3.6TB NVMe SSDs (10.8TB total NVMe capacity)
- Enterprise-grade all-NVMe storage array
- High-performance storage for multiple VM templates and isolated workspaces
- Ultra-low latency for demanding virtualization workloads

**Current Configuration:**
- Qubes OS 4.3 RC3 (pre-release testing)
- Implementing compartmentalized security architecture
- Active VMs: vault (air-gapped), personal, work, untrusted
- Whonix integration for anonymized networking
- Default Qubes storage configuration with LUKS encryption

**Learning Focus:**
- Xen hypervisor fundamentals
- Security-by-isolation model
- VM-based compartmentalization
- Hardware compatibility with pre-release software
- Whonix/Tor integration for anonymity

**Skills Demonstrated:**
- Running cutting-edge security software (RC3 pre-release)
- Understanding security domains and isolation
- Multi-VM workflow management
- System76 open-hardware platform
- Comfort with complex virtualization environments

**Status:** Active learning environment, default configuration being evaluated before customization

---

### 2. Advanced Storage Architecture Project (Desktop - Planned)

**Objective:** Design and implement production-grade storage solution

**Hardware (Desktop):**
- AMD Ryzen 9 7950X3D (16 cores)
- AMD Radeon RX 7800 XT
- 64GB RAM
- 5 drives (15TB+ total):
  - nvme1n1: 1.9TB (system)
  - sda: 10.9TB (home/Steam)
  - sdb: 2.7TB (data)
  - sdc: 931.5GB (data)
  - nvme0n1: 465.8GB (data)

**Planned Architecture:**
- Btrfs on LVM on LUKS across all drives
- Three volume groups:
  - vg-system (nvme1n1): root, var/log, var/cache, swap, docker
  - vg-data (sdb+sdc+nvme0n1): VMs, aggregated storage
  - vg-home-allen (sda): home directory + separate Steam games subvolume
- Automated snapshot management (Timeshift)
- Subvolume isolation with independent compression policies
- LUKS encryption across all volume groups

**Skills to Demonstrate:**
- Complex LVM topology design
- Btrfs advanced features (subvolumes, snapshots, compression)
- Multi-drive encryption strategy
- Storage architecture for different workload types
- Backup and disaster recovery planning

**Status:** Design phase complete, awaiting implementation

**Documentation:** Full migration plan exists, ready for execution when time permits

---

### 3. Current Daily Infrastructure

**Desktop System:**
- Primary workstation for development, gaming, productivity
- Arch Linux-based
- Managing 3-5 systems total (desktop + laptop + friend's migration project)
- Active Git workflows for projects (GitLab: MegaMek/MekHQ contributions)

**Skills in Practice:**
- Multi-system Linux administration
- Windows to Linux migration assistance
- Daily use of advanced Linux features
- Git collaboration workflows
```

---

## Updated Resume Section (Honest Version):
```
### Qubes OS Security Platform (System76 Bonobo WS) - 2024-Present
*Hands-on learning with security-focused virtualization*

- Running Qubes OS 4.3 RC3 (pre-release) on Intel i9-14900HX System76 workstation
- Dual-GPU architecture: Intel UHD (dom0) + RTX 4080 Mobile (available for passthrough)
- Implementing security-by-isolation model with separate VMs for vault, personal, work, and untrusted activities
- Integrated Whonix for anonymized networking research
- System76 platform chosen for Linux-first design and open-source firmware support

**Learning:** Xen hypervisor, VM security isolation, compartmentalized computing, pre-release software evaluation

### Advanced Storage Architecture Design (Desktop - In Planning)
*Enterprise-grade storage solution design for production deployment*

- Designed Btrfs-on-LVM-on-LUKS architecture across 5-drive, 15TB array
- Three-tier volume group strategy: vg-system (performance), vg-data (capacity), vg-home (user data)
- Subvolume isolation with independent compression and snapshot policies
- Full-disk LUKS encryption across all volume groups
- Automated snapshot management with Timeshift integration

**Skills:** LVM topology, Btrfs advanced features, encryption strategy, storage architecture design
