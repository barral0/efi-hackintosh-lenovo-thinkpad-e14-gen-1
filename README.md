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
| **Wi-Fi / Bluetooth**| Intel AX201 | ✅ | Airportitm. |
| **Ethernet** | Realtek RTL8111 | ✅ Funcional | |
| **Trackpad / Teclado** | Synaptics TrackPad | ✅ Funcional | Suporte a gestos (VoodooPS2Controller). |
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
