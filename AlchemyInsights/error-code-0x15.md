---
title: Foutcode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Als u een foutmelding krijgt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), kunt u ADAL inschakelen door het register te bewerken.
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316681"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fout tijdens activering Office 2013 op Extern bureaublad Services

Als u een foutmelding krijgt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), kunt u ADAL inschakelen door het register te bewerken.
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Zie Moderne verificatie inschakelen voor Office [2013](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)op Windows apparaten voor meer informatie.
  
**Opmerking:** ADAL is standaard ingeschakeld in Microsoft 365-apps voor ondernemingen en Office 2016. Extern bureaublad Services (RDS) kreeg eerder de naam Terminal Services.
  