---
title: Fout code 0x15
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
description: Als u een foutbericht krijgt bij het activeren van Office 2013 op Remote Desktop Services (RDS)-implementaties, dient u ADAL in te schakelen door het register te bewerken.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709182"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fout bij het activeren van Office 2013 op extern bureaublad-services

Als u een foutbericht krijgt bij het activeren van Office 2013 op Remote Desktop Services (RDS)-implementaties, dient u ADAL in te schakelen door het register te bewerken.
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Zie [moderne verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)voor meer informatie.
  
> [!NOTE]
>  ADAL is standaard ingeschakeld in Microsoft 365-apps voor Enterprise en Office 2016. Extern bureaublad-services (RDS) stond eerder met de naam Terminal Services.
  