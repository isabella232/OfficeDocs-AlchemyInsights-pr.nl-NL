---
title: Foutcode 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Als u een fout ontvangt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), u overwegen ADAL in te schakelen door het register te bewerken.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703133"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fout bij activering office 2013 op Extern bureaublad-services

Als u een fout ontvangt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), u overwegen ADAL in te schakelen door het register te bewerken.
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |Reg_dword  <br/> |1  <br/> |

Zie [Moderne verificatie inschakelen voor Office 2013 op Windows-apparaten voor](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)meer informatie.
  
> [!NOTE]
>  ADAL is standaard ingeschakeld in Microsoft 365 Apps voor bedrijven en Office 2016. Extern bureaublad-services (RDS) kreeg eerder de naam Terminal Services.
  