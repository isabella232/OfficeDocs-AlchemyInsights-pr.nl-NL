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
description: Als u een foutmelding ontvangt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), u ADAL inschakelen door het register te bewerken.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506841"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Fout tijdens activering Office 2013 op Extern bureaublad-services

Als u een foutmelding ontvangt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), u ADAL inschakelen door het register te bewerken.
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Zie [Moderne verificatie voor Office 2013 inschakelen op Windows-apparaten voor](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)meer informatie.
  
> [!NOTE]
>  ADAL is standaard ingeschakeld in Microsoft 365 Apps for enterprise en Office 2016. Rds (Remote Desktop Services) kreeg eerder de naam Terminal Services.
  