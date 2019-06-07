---
title: DKIM-installatieproblemen oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764977"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="52289-102">DKIM-installatieproblemen oplossen</span><span class="sxs-lookup"><span data-stu-id="52289-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="52289-103">Als u problemen hebt met het DKIM inschakelen voor uw aangepaste domein, gebruikt u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="52289-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="52289-104">De meeste problemen bij de installatie DKIM zijn gerelateerd aan een onjuiste DNS-records.</span><span class="sxs-lookup"><span data-stu-id="52289-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="52289-105">Controleer of dat de DKIM CNAME-record (**niet** een TXT-record) juist is opgemaakt.</span><span class="sxs-lookup"><span data-stu-id="52289-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="52289-106">Raadpleeg dit [onderwerp](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="52289-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="52289-107">Na het maken of bijwerken uw DKIM DNS-records op de DNS-hostingservice voor uw domein (meestal uw domeinregistratieservice), wachten op de DNS-records doorgeven.</span><span class="sxs-lookup"><span data-stu-id="52289-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="52289-108">Als u geen DKIM DNS records in het beheercentrum maken, vervangt u \<CustomDomain\> met uw aangepaste domein (bijvoorbeeld contoso.com) en voer deze opdracht uit in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="52289-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
