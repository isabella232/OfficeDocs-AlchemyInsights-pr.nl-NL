---
title: DKIM instellen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808702"
---
# <a name="setup-dkim"></a><span data-ttu-id="315b5-102">DKIM instellen</span><span class="sxs-lookup"><span data-stu-id="315b5-102">Setup DKIM</span></span>

<span data-ttu-id="315b5-103">De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Microsoft 365 vindt u [hier](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="315b5-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="315b5-104">Voor **elke** aangepaste domein moet u **twee** dkim CNAME-records maken bij de DNS-hostingservice van uw domein (meestal de domeinregistratie).</span><span class="sxs-lookup"><span data-stu-id="315b5-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="315b5-105">Voorbeeld van contoso.com en fourthcoffee.com zijn er vier DKIM CNAME-records nodig: twee voor contoso.com en twee voor fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="315b5-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="315b5-106">Voor de DKIM CNAME-records voor **elk** aangepast domein worden de volgende indelingen gebruikt:</span><span class="sxs-lookup"><span data-stu-id="315b5-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="315b5-107">**Naam host**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="315b5-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="315b5-108">**Verwijst naar adres of waarde**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="315b5-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="315b5-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="315b5-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="315b5-110">**Naam host**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="315b5-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="315b5-111">**Verwijst naar adres of waarde**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="315b5-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="315b5-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="315b5-112">**TTL**: 3600</span></span>

   <span data-ttu-id="315b5-113">\<DomainGUID\> de tekst links van `.mail.protection.outlook.com` de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor de domein contoso.com).</span><span class="sxs-lookup"><span data-stu-id="315b5-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="315b5-114">\<InitialDomain\> het domein is dat u hebt gebruikt toen u zich aanmeldde voor Microsoft 365 (bijvoorbeeld contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="315b5-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="315b5-115">Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies uit:</span><span class="sxs-lookup"><span data-stu-id="315b5-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="315b5-116">a.</span><span class="sxs-lookup"><span data-stu-id="315b5-116">a.</span></span> <span data-ttu-id="315b5-117">Meld u met uw werk-of schoolaccount [aan bij Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) .</span><span class="sxs-lookup"><span data-stu-id="315b5-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="315b5-118">b.</span><span class="sxs-lookup"><span data-stu-id="315b5-118">b.</span></span> <span data-ttu-id="315b5-119">Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheer**.</span><span class="sxs-lookup"><span data-stu-id="315b5-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="315b5-120">c.</span><span class="sxs-lookup"><span data-stu-id="315b5-120">c.</span></span> <span data-ttu-id="315b5-121">Vouw in het navigatievenster aan de linkerkant **Beheerder** uit en kies **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="315b5-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="315b5-122">d.</span><span class="sxs-lookup"><span data-stu-id="315b5-122">d.</span></span> <span data-ttu-id="315b5-123">Ga naar **Protection**  >  **dkim**.</span><span class="sxs-lookup"><span data-stu-id="315b5-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="315b5-124">e.</span><span class="sxs-lookup"><span data-stu-id="315b5-124">e.</span></span> <span data-ttu-id="315b5-125">Selecteer het domein en kies vervolgens **inschakelen** voor **Onderteken berichten voor dit domein met dkim handtekeningen**.</span><span class="sxs-lookup"><span data-stu-id="315b5-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="315b5-126">Herhaal deze stap voor elk aangepast domein.</span><span class="sxs-lookup"><span data-stu-id="315b5-126">Repeat this step for each custom domain.</span></span>
