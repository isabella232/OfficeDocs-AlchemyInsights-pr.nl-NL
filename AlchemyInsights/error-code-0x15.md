---
title: Foutcode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284224"
---
Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken. 
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Zie voor meer informatie, [Moderne-verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL is standaard ingeschakeld in Office 365 ProPlus en Office 2016. > De extern bureaublad-Services (RDS) is eerder met de naam Terminal Services. 
  

