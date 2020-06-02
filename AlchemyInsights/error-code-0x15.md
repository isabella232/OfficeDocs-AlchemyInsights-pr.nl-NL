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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="00073-103">Fout tijdens activering Office 2013 op Extern bureaublad-services</span><span class="sxs-lookup"><span data-stu-id="00073-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="00073-104">Als u een foutmelding ontvangt tijdens het activeren van Office 2013 op RDS-implementaties (Remote Desktop Services), u ADAL inschakelen door het register te bewerken.</span><span class="sxs-lookup"><span data-stu-id="00073-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="00073-105">**Registersleutel**</span><span class="sxs-lookup"><span data-stu-id="00073-105">**Registry key**</span></span>|<span data-ttu-id="00073-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="00073-106">**Type**</span></span>|<span data-ttu-id="00073-107">**Value**</span><span class="sxs-lookup"><span data-stu-id="00073-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="00073-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="00073-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="00073-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="00073-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="00073-110">1</span><span class="sxs-lookup"><span data-stu-id="00073-110">1</span></span>  <br/> |

<span data-ttu-id="00073-111">Zie [Moderne verificatie voor Office 2013 inschakelen op Windows-apparaten voor](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="00073-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="00073-112">ADAL is standaard ingeschakeld in Microsoft 365 Apps for enterprise en Office 2016.</span><span class="sxs-lookup"><span data-stu-id="00073-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="00073-113">Rds (Remote Desktop Services) kreeg eerder de naam Terminal Services.</span><span class="sxs-lookup"><span data-stu-id="00073-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  