---
title: Problemen met de installatie van DKIM oplossen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744945"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="d67e8-102">Problemen met de installatie van DKIM oplossen</span><span class="sxs-lookup"><span data-stu-id="d67e8-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="d67e8-103">Als u problemen ondervindt bij het inschakelen van DKIM voor uw aangepaste domein, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="d67e8-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="d67e8-104">De meeste problemen met de installatie van DKIM hebben betrekking op onjuiste DNS-records.</span><span class="sxs-lookup"><span data-stu-id="d67e8-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="d67e8-105">Controleer of de DKIM CNAME-record (**geen** TXT-record) correct is opgemaakt.</span><span class="sxs-lookup"><span data-stu-id="d67e8-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="d67e8-106">Zie het volgende [onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d67e8-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="d67e8-107">Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistratie), wacht dan totdat de DNS-records zijn doorgegeven.</span><span class="sxs-lookup"><span data-stu-id="d67e8-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="d67e8-108">Als u de DNS-records van DKIM niet kunt maken in het Beheercentrum, kunt u \<CustomDomain\> deze vervangen door uw aangepaste domein (bijvoorbeeld contoso.com) en deze opdracht uit te voeren in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="d67e8-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
