## 💻 EFI OpenCore para Lenovo ThinkPad E14 Gen [Geração] (Processador [Intel/AMD])

Um guia e arquivos EFI para instalar o macOS [Nome do macOS, ex: Ventura/Sonoma] no Lenovo ThinkPad E14.

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
| **Áudio** | [Modelo do Codec, ex: Realtek ALC257] | ✅ Funcional | `layout-id`: [Número do Layout-ID] |
| **Wi-Fi / Bluetooth**| [Modelo do Chip, ex: Intel AX201] | ✅ / ❌ | Airportitm. |
| **Ethernet** | [Modelo, ex: Realtek RTL8111] | ✅ Funcional | |
| **Trackpad / Teclado** | [Modelo, ex: Synaptics TrackPad] | ✅ Funcional | Suporte a gestos (VoodooPS2Controller). |
| **Webcam** | Integrada | ✅ Funcional | |
| **SMBIOS Usado** | MacBookPro16,3 | N/A | Recomendado para o seu chip. |
| **Versão do OpenCore** | 1.0.5 | N/A | |

---

## ✅ O que Funciona

* ✅ Aceleração Gráfica Completa (Metal)
* ✅ Áudio (Alto-falantes e Fone de ouvido)
* ✅ TrackPad com Gestos e Teclado
* ✅ Portas USB 3.0 e Type-C
* ✅ Câmera e Microfone
* ✅ Wifi
* ✅ Ethernet
* ✅ Monitor Externo (HDMI/USB-C)
* ✅ Gerenciamento de Energia e Bateria (Power Management)
* ✅ Sleep/Wake (Dormir/Acordar)

## ❌ O que Não Funciona (Problemas Conhecidos)

* ❌ **Bluetooth:** 
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
| **Display (VRAM)**| Config > Display | [Se for possível, altere para **256M** ou **512M**] |
| **Fast Boot** | Config > Power (ou Startup) | `Disabled` |

---

## 🧩 Kexts e Drivers Usados

| Tipo | Nome | Versão | Função |
| :--- | :--- | :--- | :--- |
| Bootloader | OpenCore | [Versão] | Gerenciador de inicialização. |
| Kext | Lilu | [Versão] | Core patcher para diversas kexts. |
| Kext | WhateverGreen | [Versão] | Gráficos e correções de display. |
| Kext | VirtualSMC | [Versão] | Emulação do System Management Controller (SMC). |
| Kext | VoodooPS2Controller | [Versão] | Teclado e Trackpad. |
| Kext | AppleALC | [Versão] | Áudio. |
| Kext | [Sua Kext de Rede] | [Versão] | [Ethernet/Wi-Fi]. |
| SSDT | SSDT-PLUG | | Power Management. |
| SSDT | [Outro SSDT] | | [Função]. |

---

## 🔗 Recursos Úteis

* **Guia Dortania (OpenCore):** [https://dortania.github.io/OpenCore-Install-Guide/](https://dortania.github.io/OpenCore-Install-Guide/)
* **Gerador de SMBIOS (GenSMBIOS):** [https://github.com/corpnewt/GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
* **Editor de Plist (ProperTree):** [https://github.com/corpnewt/ProperTree](https://github.com/corpnewt/ProperTree)

---
### 🎥 Meu Vídeo Sobre Este Hackintosh

[Adicione o link do seu vídeo do YouTube aqui!] - [Título do Vídeo]

---
