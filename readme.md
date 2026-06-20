# NovaKernel-GKI

Build automatizado de kernel GKI com **KernelSU (Oficial)** + **SUSFS** integrados.

Forkado de [zzh20188/GKI_KernelSU_SUSFS](https://github.com/zzh20188/GKI_KernelSU_SUSFS) e adaptado para o KernelSU oficial de [tiann](https://github.com/tiann/KernelSU).

## Versão suportada

| Android | Kernel | Sublevel |
|:---:|:---:|:---:|
| Android 12 | 5.10 | 5.10.240 |

## Funcionalidades

| Feature | Status | Descrição |
|:---|:---:|:---|
| KernelSU Official | ✅ | Solução de root por tiann |
| SUSFS | ✅ | Esconde rastros de root |
| ZRAM LZ4KD | ✅ | LZ4 v1.10.0 + LZ4KD + aceleração ARM64 NEON |
| BBG (Baseband Guard) | ✅ | Proteção contra exploits de baseband |
| Re-Kernel | ✅ | Proteção via GKI Vendor Hooks |

## Como usar

1. Vá na aba **Actions**
2. Selecione o workflow **Compilar Kernel**
3. Clique em **Run workflow**
4. Aguarde o build finalizar
5. Baixe o zip AnyKernel3 em **Releases** ou **Artifacts**

## Créditos

- [tiann](https://github.com/tiann) - Criador do KernelSU
- [simonpunk](https://gitlab.com/simonpunk) - Criador do SUSFS
- [zzh20188](https://github.com/zzh20188) - Repo original GKI_KernelSU_SUSFS
