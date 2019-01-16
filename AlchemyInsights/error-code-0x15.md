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
<span data-ttu-id="467c6-103">Als u een foutbericht ontvangt bij het activeren van Office 2013 op implementaties van extern bureaublad-Services (RDS), kunt u het ADAL inschakelen door het register te bewerken.</span><span class="sxs-lookup"><span data-stu-id="467c6-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="467c6-104">**Registersleutel**</span><span class="sxs-lookup"><span data-stu-id="467c6-104">**Registry key**</span></span>|<span data-ttu-id="467c6-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="467c6-105">**Type**</span></span>|<span data-ttu-id="467c6-106">**Value**</span><span class="sxs-lookup"><span data-stu-id="467c6-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="467c6-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="467c6-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="467c6-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="467c6-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="467c6-109">1</span><span class="sxs-lookup"><span data-stu-id="467c6-109">1</span></span>  <br/> |
   
<span data-ttu-id="467c6-110">Zie voor meer informatie, [Moderne-verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="467c6-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="467c6-p101">ADAL is standaard ingeschakeld in Office 365 ProPlus en Office 2016. > De extern bureaublad-Services (RDS) is eerder met de naam Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="467c6-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

