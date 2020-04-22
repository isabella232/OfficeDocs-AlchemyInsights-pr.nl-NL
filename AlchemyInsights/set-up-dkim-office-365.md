---
title: Installatie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645667"
---
# <a name="setup-dkim"></a><span data-ttu-id="ae8b9-102">Installatie DKIM</span><span class="sxs-lookup"><span data-stu-id="ae8b9-102">Setup DKIM</span></span>

<span data-ttu-id="ae8b9-103">De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Microsoft 365 zijn [hier.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="ae8b9-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="ae8b9-104">Voor **elk** aangepast domein moet u **twee** DKIM CNAME-records maken op de DNS-hostingservice van uw domein (meestal de domeinregistrar).</span><span class="sxs-lookup"><span data-stu-id="ae8b9-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="ae8b9-105">Voor contoso.com en fourthcoffee.com bijvoorbeeld vier DKIM CNAME-records: twee voor contoso.com en twee voor fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="ae8b9-106">De DKIM CNAME-records voor **elk** aangepast domein gebruiken de volgende indelingen:</span><span class="sxs-lookup"><span data-stu-id="ae8b9-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="ae8b9-107">**Hostnaam**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ae8b9-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ae8b9-108">**Adres- of waardeaanspraken:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ae8b9-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ae8b9-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="ae8b9-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="ae8b9-110">**Hostnaam**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="ae8b9-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="ae8b9-111">**Adres- of waardeaanspraken:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="ae8b9-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="ae8b9-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="ae8b9-112">**TTL**: 3600</span></span>

   <span data-ttu-id="ae8b9-113">\<DomainGUID\> is de tekst `.mail.protection.outlook.com` links van in de aangepaste MX-record `contoso-com` voor het aangepaste domein (bijvoorbeeld voor het domein contoso.com).</span><span class="sxs-lookup"><span data-stu-id="ae8b9-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="ae8b9-114">\<InitialDomain\> is het domein dat u hebt gebruikt toen u zich aanmeldde voor Microsoft 365 (bijvoorbeeld contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="ae8b9-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="ae8b9-115">Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies uit:</span><span class="sxs-lookup"><span data-stu-id="ae8b9-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="ae8b9-116">a.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-116">a.</span></span> <span data-ttu-id="ae8b9-117">[meld u aan bij Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="ae8b9-118">b.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-118">b.</span></span> <span data-ttu-id="ae8b9-119">Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheer**.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="ae8b9-120">C.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-120">c.</span></span> <span data-ttu-id="ae8b9-121">Vouw in het navigatievenster aan de linkerkant **Beheerder** uit en kies **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="ae8b9-122">D.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-122">d.</span></span> <span data-ttu-id="ae8b9-123">Ga naar **Protection** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="ae8b9-124">E.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-124">e.</span></span> <span data-ttu-id="ae8b9-125">Selecteer het domein en kies **Inschakelen** voor Berichten ondertekenen **voor dit domein met DKIM-handtekeningen**.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="ae8b9-126">Herhaal deze stap voor elk aangepast domein.</span><span class="sxs-lookup"><span data-stu-id="ae8b9-126">Repeat this step for each custom domain.</span></span>
