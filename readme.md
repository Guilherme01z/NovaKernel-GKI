<div align="center">

# NovaKernel-GKI
### Automated GKI Kernel Build with KernelSU + SUSFS

**Automated GKI Kernel Builds | KernelSU Official + SUSFS**

[![Release](https://img.shields.io/github/v/release/Guilherme01z/NovaKernel-GKI?label=Release&style=flat-square&logo=github&logoColor=white&color=2ea44f)](https://github.com/Guilherme01z/NovaKernel-GKI/releases)
[![KernelSU](https://img.shields.io/badge/KernelSU-Official-0088cc?style=flat-square)](https://github.com/tiann/KernelSU)
[![SUSFS](https://img.shields.io/badge/SUSFS-Integrated-E67E22?style=flat-square)](https://gitlab.com/simonpunk/susfs4ksu)

---

</div>

## About

This repository automates the build of Android GKI (Generic Kernel Image) kernels with **KernelSU (Official)** and **SUSFS** integrated.

Forked from [zzh20188/GKI_KernelSU_SUSFS](https://github.com/zzh20188/GKI_KernelSU_SUSFS/) and adapted for the **official KernelSU** variant by [tiann](https://github.com/tiann/KernelSU).

## Supported Versions

| Android | Kernel | Status |
|:---:|:---:|:---|
| Android 12 | 5.10 | Supported |
| Android 13 | 5.15 | Supported |
| Android 14 | 6.1 | Supported |
| Android 15 | 6.6 | Supported |
| Android 16 | 6.12 | Supported |

## Features

- **KernelSU Official** - Root solution by tiann
- **SUSFS** - Hide root traces from detection
- **ZRAM Enhancement** - LZ4 v1.10.0 + LZ4KD + ARM64 NEON acceleration
- **BBG (Baseband Guard)** - Protection against baseband exploits
- **Re-Kernel** - Kernel-level protection via GKI Vendor Hooks
- **Droidspaces** - Linux container support on Android (experimental)
- **NTSync** - NT synchronization for Wine/Proton (experimental)
- **Stock Config** - Spoof `/proc/config.gz` with official config

## Optional Features Impact

| Feature | Battery | Performance | When Active |
|:---|:---:|:---:|:---|
| ZRAM/LZ4KD | Improves | Improves | Always (swap) |
| BBG | Negligible | Negligible | Baseband operations |
| Re-Kernel | Minimal overhead | Minimal overhead | Always (hooks) |
| Droidspaces | Zero | Zero | Only with containers |
| NTSync | Zero | Zero | Only with Wine/Proton |

## How to Use

1. Go to **Actions** tab
2. Select **Build GKI Kernel** workflow
3. Click **Run workflow**
4. Select Android/Kernel versions and options
5. Wait for build to complete
6. Download the AnyKernel3 zip from Releases or Artifacts

## Credits

- [tiann](https://github.com/tiann) - KernelSU creator
- [simonpunk](https://gitlab.com/simonpunk) - SUSFS creator
- [zzh20188](https://github.com/zzh20188) - Original GKI_KernelSU_SUSFS repo

---

<div align="center">

⭐ If this project helps you, give it a Star!

</div>
