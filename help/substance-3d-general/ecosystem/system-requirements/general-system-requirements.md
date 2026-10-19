---
helpx_url: 'https://helpx.adobe.com/br/substance-3d-general/ecosystem/general-system-requirements.html'
breadcrumb-title: ''
description: Verifique os requisitos de sistema dos aplicativos da Substance 3D para garantir que seu hardware atenda às especificações mínimas, recomendadas ou ótimas.
helpx_creative_field: ''
helpx_description: General Knowledge > Ecosystem > General system requirements
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: Requisitos gerais de sistema
user-guide-description: ''
user-guide-title: ''
source-git-commit: eef3d78f33034f2c24f4c4471d9ccac805184525
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 2%
---

# Requisitos gerais de sistema

## Requisitos de hardware

+++Windows

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| **SO** | Windows 11 64 bits versão 23H2 | Windows 11 64 bits versão 24H1 | Windows 11 64 bits versão 24H2 |
| **CPU** | Intel Core i5 AMD Ryzen 5 | Intel Core i7 AMD Ryzen 7 | Intel Core i9 AMD Ryzen 9 |
| **GPU** | NVIDIA GeForce RTX 2060 Super NVIDIA Quadro RTX 4000 AMD Radeon RX 5700 XT AMD Radeon Pro W5700 | NVIDIA GeForce RTX 3080 NVIDIA Quadro RTX A4000 AMD Radeon RX 6800 XT AMD Radeon Pro W7700 | NVIDIA GeForce RTX 4090 NVIDIA Quadro RTX 5000 Ada Generation AMD Radeon RX 7900 XTX AMD Radeon Pro W7800 |
| **VRAM** | 8 GB | 16 GB | 24 GB |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Armazenamento** | SSD com 30 GB de espaço disponível | SSD com 50 GB de espaço disponível | SSD com 70 GB de espaço disponível |

+++

+++macOS

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| **SO** | macOS 15 Sequoia | macOS 27 Golden Gate | macOS 27 Golden Gate |
| **CPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **GPU** | Apple M1 | Apple M2 Pro | Apple M4 Pro |
| **RAM** | 16 GB | 32 GB | 64 GB |
| **Armazenamento** | SSD com 30 GB de espaço disponível | SSD com 50 GB de espaço disponível | SSD com 70 GB de espaço disponível |

>[!WARNING]
>
> Para pipelines criados com a [Plataforma de Referência VFX](https://vfxplatform.com/) em mente, os aplicativos da Substance 3D ainda podem ser instalados no macOS 14 Sonoma. No entanto, os aplicativos Substance não são mais testados nas versões do sistema operacional abaixo dos requisitos mínimos de sistema, portanto, a estabilidade não é garantida. É recomendável atualizar para uma versão mais recente do sistema operacional.

+++

+++Linux

|  | Mínimo | Recomendado | Ideal |
| --- | --- | --- | --- |
| **SO** | **ETLA corporativo** RHEL 8.6 ou posterior ou RHEL 9.2 ou posterior **Vapor** Ubuntu 22.04.1 LTS | **Enterprise ETLA** RHEL 8.6 ou posterior ou RHEL 9.4 ou posterior **Steam** Ubuntu 22.04.1 LTS ou posterior | **Enterprise ETLA** RHEL 8.6 ou posterior ou RHEL 9.4 ou posterior **Steam** Ubuntu 22.04.1 LTS ou posterior |

**Red Hat Enterprise Linux (RHEL) 9.x**: o pacote xcb-util-cursor necessário para nossos aplicativos foi removido do repositório EPEL 9 em 10 de maio de 2024. A partir dessa data, o pacote é suportado pelo repositório padrão do RHEL 9, coincidindo com a versão do RHEL 9.4. Os clientes que usam versões do RHEL anteriores à 9.4 não poderão mais obter o pacote xcb-util-cursor do repositório do EPEL 9 após 10 de maio de 2024.

Para obter mais informações sobre a disponibilidade deste pacote no repositório RHEL 9 padrão, consulte: [Red Hat Enterprise Linux 9 - Manifesto do pacote - Repositório AppStream](https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/9/html-single/package_manifest/index#AppStream-repository)

Para obter mais informações sobre essa alteração, consulte: [Red Hat Bugzilla - Bug 2238273](https://bugzilla.redhat.com/show_bug.cgi?id=2238273) , [Red Hat Bugzilla - Bug 2212302](https://bugzilla.redhat.com/show_bug.cgi?id=2212302)

+++

+++RV

| Marca | Modelos |
| --- | --- |
| Meta | Rift, Rift S, Quest, Quest 2 (com link), Quest Pro |

+++

Para obter mais detalhes, observe os requisitos de cada aplicativo:

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/sa-appicon-noshadow-256.png" alt="Ícone do Substance 3D Sampler" width="64px"/><br><a href="https://experienceleague.adobe.com/pt-br/docs/substance-3d-sampler/using/getting-started/system-requirements">Substance 3D Sampler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/ds-appicon-noshadow-256.png" alt="Ícone do Substance 3D Designer" width="64px"/><br><a href="https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/getting-started/system-requirements">Substance 3D</a> <a href="https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/getting-started/system-requirements">Designer</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/pt-appicon-noshadow-256.png" alt="Ícone do Substance 3D Painter" width="64px"/><br><a href="https://experienceleague.adobe.com/pt-br/docs/substance-3d-painter/using/getting-started/system-requirements">Substance 3D Painter</a></td>
  </tr>
</table>

<table>
  <tr style="border: 0;">
    <td style="border: 0;" valign="top"><img src="../../assets/md-appicon-noshadow-256.png" alt="Ícone do Substance 3D Modeler" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-modeler/getting-started/system-requirements.html">Substance 3D Modeler</a></td>
    <td style="border: 0;" valign="top"><img src="../../assets/sg-appicon-noshadow-256.png" alt="Ícone do Substance 3D Stager" width="64px"/><br><a href="https://helpx.adobe.com/substance-3d-stager/getting-started/system-requirements.html">Substance 3D Stager</a></td>
    <td style="border: 0;" valign="top"></td>
  </tr>
</table>

## Notas adicionais

### Configuração sem suporte

* As configurações do computador Apple com eGPUs e GPUs instaladas pelo usuário não são compatíveis.
* Não há suporte para máquinas virtuais do Windows.
* Não há suporte para o sistema operacional Windows Server.
