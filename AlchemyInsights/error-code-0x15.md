---
title: Foutcode 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402734"
---
Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken. 
  
|**Registersleutel**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Zie voor meer informatie, [Moderne-verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL is standaard ingeschakeld in Office 365 ProPlus en Office 2016. > extern bureaublad-Services (RDS) is eerder met de naam Terminal Services. 
  

