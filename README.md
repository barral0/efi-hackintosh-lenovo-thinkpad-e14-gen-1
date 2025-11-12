## 💻 EFI OpenCore para Lenovo ThinkPad E14 Gen 1 (Intel)

Arquivos EFI para instalar o macOS Sonoma no Lenovo ThinkPad E14.

### ⚠️ AVISO LEGAL E SEGURANÇA

> Este repositório é fornecido **AS IS** (como está). Eu não sou responsável por qualquer dano, perda de dados ou problemas que possam ocorrer no seu hardware. **Faça um backup** de todos os seus dados importantes antes de prosseguir.
>
> É **fortemente recomendado** que você gere seus próprios números de série (`SMBIOS`) usando o [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) antes de usar esta EFI.

---

## 🛠️ Especificações do Hardware

| Componente | Detalhe da Peça | Status no macOS | Notas |
| :--- | :--- | :--- | :--- |
| **Modelo do Laptop** | Lenovo ThinkPad E14 Gen 1 | N/A | Video em breve |
| **CPU** | i5 10210U | ✅ Funcional | Performance nativa com Power Management. |
| **iGPU (Gráficos)** | UHD Graphics | ✅ Funcional | Aceleração gráfica (Metal) funcionando. |
| **Áudio** | ALC257 | ✅ Funcional | `layout-id`: 15 |
| **Wi-Fi / Bluetooth**| Intel AX201 | ✅ | AirportItlwm + OCLP (Necessário Wi-Fi Spoofing para o Patch). |
| **Ethernet** | Realtek RTL8111 | ✅ Funcional | |
| **Trackpad / Teclado** | Synaptics TrackPad | ✅ Funcional | Suporte a gestos (VoodooPS2Controller). |
| **Webcam** | Integrada | ✅ Funcional | |
| **SMBIOS Usado** | MacBookPro16,3 | N/A | |
| **Versão do OpenCore** | 1.0.5 | N/A | |

---

## ✅ O que Funciona

* ✅ Aceleração Gráfica Completa (Metal)
* ✅ Áudio (Alto-falantes e Fone de ouvido)
* ✅ TrackPad com Gestos e Teclado
* ✅ Portas USB 3.0 e Type-C
* ✅ Câmera e Microfone
* ✅ Wifi (via Sistema, com patch OCLP)
* ✅ Ethernet
* ✅ Monitor Externo (HDMI/USB-C)
* ✅ Gerenciamento de Energia e Bateria (Power Management)
* ✅ Sleep/Wake (Dormir/Acordar)

## ❌ O que Não Funciona

* ❌ **Bluetooth:** - Parcialmente
* ❌ **Leitor de Impressão Digital (Fingerprint):** Sem suporte.

---

## ⚙️ Configurações da BIOS

Acesse a BIOS aplique as seguintes configurações:

| Setting | Path (Caminho) | Valor |
| :--- | :--- | :--- |
| **Secure Boot** | Security > Secure Boot | `Disabled` |
| **Intel Platform Trust** | Security > Security Chip | `Disabled` (ou Desligado) |
| **Intel VT-d** | Security > Virtualization | `Disabled` |
| **SATA Mode** | Config > Serial ATA | `AHCI` |
| **Fast Boot** | Config > Power (ou Startup) | `Disabled` |

---

## 🔗 Recursos Úteis

* **Guia Dortania (OpenCore):** [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
* **Gerador de SMBIOS (GenSMBIOS):** [https://github.com/corpnewt/GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
* **Editor de Plist (ProperTree):** [https://github.com/corpnewt/ProperTree](https://github.com/corpnewt/ProperTree)

---
### 🎥 Meu Vídeo Sobre Este Hackintosh

Em breve

---


## 💻 OpenCore EFI for Lenovo ThinkPad E14 Gen 1 (Intel)

EFI files to install macOS Sonoma on the Lenovo ThinkPad E14.

### ⚠️ DISCLAIMER AND SAFETY

> This repository is provided **AS IS**. I am not responsible for any damage, data loss, or issues that may occur with your hardware. **Make a backup** of all your important data before proceeding.
>
> It is **strongly recommended** that you generate your own serial numbers (`SMBIOS`) using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) before using this EFI.

---

## 🛠️ Hardware Specifications

| Component | Part Detail | Status in macOS | Notes |
| :--- | :--- | :--- | :--- |
| **Laptop Model** | Lenovo ThinkPad E14 Gen 1 | N/A |  |
| **CPU** | i5 10210U | ✅ Working | Native performance with Power Management. |
| **iGPU (Graphics)** | UHD Graphics | ✅ Working | Graphics acceleration (Metal) working. |
| **Audio** | ALC257 | ✅ Working | `layout-id`: 15 |
| **Wi-Fi / Bluetooth**| Intel AX201 | ✅ | AirportItlwm + OCLP (Requires Wi-Fi Spoofing for the Patch). |
| **Ethernet** | Realtek RTL8111 | ✅ Working | |
| **Trackpad / Keyboard** | Synaptics TrackPad | ✅ Working | Gesture support (VoodooPS2Controller). |
| **Webcam** | Integrated | ✅ Working | |
| **SMBIOS Used** | MacBookPro16,3 | N/A | |
| **OpenCore Version** | 1.0.5 | N/A | |

---

## ✅ What Works

* ✅ Full Graphics Acceleration (Metal)
* ✅ Audio (Speakers and Headphone jack)
* ✅ TrackPad with Gestures and Keyboard
* ✅ USB 3.0 and Type-C Ports
* ✅ Camera and Microphone
* ✅ Wifi (via System, with OCLP patch)
* ✅ Ethernet
* ✅ External Monitor (HDMI/USB-C)
* ✅ Power Management and Battery
* ✅ Sleep/Wake

## ❌ What Doesn't Work

* ❌ **Bluetooth:** - Partially
* ❌ **Fingerprint Reader:** No support.

---

## ⚙️ BIOS Settings

Access the BIOS and apply the following settings:

| Setting | Path | Value |
| :--- | :--- | :--- |
| **Secure Boot** | Security > Secure Boot | `Disabled` |
| **Intel Platform Trust** | Security > Security Chip | `Disabled` |
| **Intel VT-d** | Security > Virtualization | `Disabled` |
| **SATA Mode** | Config > Serial ATA | `AHCI` |
| **Fast Boot** | Config > Power (ou Startup) | `Disabled` |

---

## 🔗 Useful Resources

* **Dortania's Guide (OpenCore):** [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
* **SMBIOS Generator (GenSMBIOS):** [https://github.com/corpnewt/GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
* **Plist Editor (ProperTree):** [https://github.com/corpnewt/ProperTree](https://github.com/corpnewt/ProperTree)

---

