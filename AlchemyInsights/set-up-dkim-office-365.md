---
title: DKIM instellen in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666259"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="4e262-102">DKIM instellen in Office 365</span><span class="sxs-lookup"><span data-stu-id="4e262-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="4e262-103">De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Office 365 zijn [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4e262-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="4e262-104">Voor **elk** aangepast domein moet u **twee** dkim CNAME-records maken in de DNS-hosting service van uw domein (meestal de domeinregistrar).</span><span class="sxs-lookup"><span data-stu-id="4e262-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4e262-105">Contoso.com en fourthcoffee.com vereisen bijvoorbeeld vier DKIM CNAME-records: twee voor contoso.com en twee voor fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="4e262-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4e262-106">De DKIM CNAME-records voor **elk** aangepast domein gebruiken de volgende notaties:</span><span class="sxs-lookup"><span data-stu-id="4e262-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4e262-107">**Hostnaam**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4e262-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4e262-108">**Verwijst naar adres of waarde**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4e262-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4e262-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4e262-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4e262-110">**Hostnaam**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4e262-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4e262-111">**Verwijst naar adres of waarde**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4e262-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4e262-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4e262-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4e262-113">\<Domaingd\> is de tekst links van `.mail.protection.outlook.com` in de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor het domein contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4e262-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4e262-114">\<InitialDomain\> is het domein dat u hebt gebruikt toen u zich aanmeldde voor Office 365 (bijvoorbeeld contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="4e262-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4e262-115">Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies:</span><span class="sxs-lookup"><span data-stu-id="4e262-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4e262-116">A.</span><span class="sxs-lookup"><span data-stu-id="4e262-116">a.</span></span> <span data-ttu-id="4e262-117">[Meld u aan bij Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.</span><span class="sxs-lookup"><span data-stu-id="4e262-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4e262-118">B.</span><span class="sxs-lookup"><span data-stu-id="4e262-118">b.</span></span> <span data-ttu-id="4e262-119">Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheerder**.</span><span class="sxs-lookup"><span data-stu-id="4e262-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4e262-120">C.</span><span class="sxs-lookup"><span data-stu-id="4e262-120">c.</span></span> <span data-ttu-id="4e262-121">Vouw in de linkerbenedenhoek van de navigatie **admin** en kies **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4e262-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4e262-122">D.</span><span class="sxs-lookup"><span data-stu-id="4e262-122">d.</span></span> <span data-ttu-id="4e262-123">Ga naar **bescherming** > **dkim**.</span><span class="sxs-lookup"><span data-stu-id="4e262-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4e262-124">E.</span><span class="sxs-lookup"><span data-stu-id="4e262-124">e.</span></span> <span data-ttu-id="4e262-125">Selecteer het domein en kies vervolgens **inschakelen** voor **Aanmeldingsberichten voor dit domein met dkim-handtekeningen**.</span><span class="sxs-lookup"><span data-stu-id="4e262-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4e262-126">Herhaal deze stap voor elk aangepast domein.</span><span class="sxs-lookup"><span data-stu-id="4e262-126">Repeat this step for each custom domain.</span></span>
