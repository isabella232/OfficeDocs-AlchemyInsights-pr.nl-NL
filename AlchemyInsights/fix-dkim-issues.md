---
title: Problemen met DKIM-instellingen oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506769"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="506f6-102">Problemen met DKIM-instellingen oplossen</span><span class="sxs-lookup"><span data-stu-id="506f6-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="506f6-103">Als u problemen ondervindt bij het inschakelen van DKIM voor uw aangepaste domein, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="506f6-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="506f6-104">De meeste DKIM-installatieproblemen zijn gerelateerd aan onjuiste DNS-records.</span><span class="sxs-lookup"><span data-stu-id="506f6-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="506f6-105">Controleer of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt.</span><span class="sxs-lookup"><span data-stu-id="506f6-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="506f6-106">Zie dit onderwerp [voor](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="506f6-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="506f6-107">Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistrar), wacht u tot de DNS-records zijn doorgegeven.</span><span class="sxs-lookup"><span data-stu-id="506f6-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="506f6-108">Als u de DNS-records van DKIM niet maken in het beheercentrum, u \<CustomDomain\> uw aangepaste domein (bijvoorbeeld contoso.com) vervangen en deze opdracht uitvoeren in Exchange Online [PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="506f6-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
