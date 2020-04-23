---
title: Problemen met de installatie van DKIM oplossen
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717557"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="4a736-102">Problemen met de installatie van DKIM oplossen</span><span class="sxs-lookup"><span data-stu-id="4a736-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="4a736-103">Als u problemen ondervindt bij het inschakelen van DKIM voor uw aangepaste domein, gebruikt u de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="4a736-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="4a736-104">De meeste problemen met de installatie van DKIM zijn gerelateerd aan onjuiste DNS-records.</span><span class="sxs-lookup"><span data-stu-id="4a736-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="4a736-105">Controleer of de DKIM CNAME-record **(geen** TXT-record) correct is opgemaakt.</span><span class="sxs-lookup"><span data-stu-id="4a736-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="4a736-106">Zie dit [onderwerp](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4a736-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="4a736-107">Nadat u uw DKIM DNS-records hebt gemaakt of bijgewerkt bij de DNS-hostingservice voor uw domein (meestal uw domeinregistrar), wacht u tot de DNS-records worden gepropageerd.</span><span class="sxs-lookup"><span data-stu-id="4a736-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="4a736-108">Als u de DKIM DNS-records niet maken \<in\> het beheercentrum, u CustomDomain vervangen door uw aangepaste `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`domein (bijvoorbeeld contoso.com) en deze opdracht uitvoeren in Exchange Online [PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="4a736-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
