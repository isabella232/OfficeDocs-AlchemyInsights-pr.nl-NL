---
title: Foutcode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388240"
---
Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken.
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Zie voor meer informatie, [Moderne-verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL is standaard ingeschakeld in Office 365 ProPlus en Office 2016. > extern bureaublad-Services (RDS) is eerder met de naam Terminal Services.
  