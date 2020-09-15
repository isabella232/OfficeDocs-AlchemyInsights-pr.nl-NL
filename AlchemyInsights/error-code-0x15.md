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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="e4c87-103">Fout bij het activeren van Office 2013 op extern bureaublad-services</span><span class="sxs-lookup"><span data-stu-id="e4c87-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="e4c87-104">Als u een foutbericht krijgt bij het activeren van Office 2013 op Remote Desktop Services (RDS)-implementaties, dient u ADAL in te schakelen door het register te bewerken.</span><span class="sxs-lookup"><span data-stu-id="e4c87-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="e4c87-105">**Registersleutel**</span><span class="sxs-lookup"><span data-stu-id="e4c87-105">**Registry key**</span></span>|<span data-ttu-id="e4c87-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="e4c87-106">**Type**</span></span>|<span data-ttu-id="e4c87-107">**Value**</span><span class="sxs-lookup"><span data-stu-id="e4c87-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e4c87-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="e4c87-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="e4c87-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="e4c87-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="e4c87-110">1</span><span class="sxs-lookup"><span data-stu-id="e4c87-110">1</span></span>  <br/> |

<span data-ttu-id="e4c87-111">Zie [moderne verificatie inschakelen voor Office 2013 op Windows-apparaten](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e4c87-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="e4c87-112">ADAL is standaard ingeschakeld in Microsoft 365-apps voor Enterprise en Office 2016.</span><span class="sxs-lookup"><span data-stu-id="e4c87-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="e4c87-113">Extern bureaublad-services (RDS) stond eerder met de naam Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="e4c87-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  