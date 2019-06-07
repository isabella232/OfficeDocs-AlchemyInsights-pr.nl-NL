---
title: Setup DKIM in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764989"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="d0202-102">Setup DKIM in Office 365</span><span class="sxs-lookup"><span data-stu-id="d0202-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="d0202-103">De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Office 365 zijn [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="d0202-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="d0202-104">U moet voor **elke** aangepaste domein maken **twee** DKIM CNAME-records van uw domein DNS-hostingservice (meestal de domeinregistratieservice).</span><span class="sxs-lookup"><span data-stu-id="d0202-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="d0202-105">Bijvoorbeeld contoso.com en fourthcoffee.com vier DKIM CNAME-records vereist: twee voor contoso.com en twee voor fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="d0202-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="d0202-106">De DKIM CNAME-records voor **elke** aangepaste domein gebruikt de volgende indelingen:</span><span class="sxs-lookup"><span data-stu-id="d0202-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="d0202-107">**Hostnaam**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0202-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d0202-108">**Verwijst naar het adres of de waarde**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0202-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d0202-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d0202-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="d0202-110">**Hostnaam**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0202-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="d0202-111">**Verwijst naar het adres of de waarde**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="d0202-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="d0202-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="d0202-112">**TTL**: 3600</span></span>

   <span data-ttu-id="d0202-113">\<DomainGUID\> is de tekst links van `.mail.protection.outlook.com` in de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor het domein contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d0202-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="d0202-114">\<InitialDomain\> is het domein dat u hebt gebruikt toen u zich voor Office 365 (bijvoorbeeld contoso.onmicrosoft.com aanmeldde).</span><span class="sxs-lookup"><span data-stu-id="d0202-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="d0202-115">Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies:</span><span class="sxs-lookup"><span data-stu-id="d0202-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="d0202-116">een.</span><span class="sxs-lookup"><span data-stu-id="d0202-116">a.</span></span> <span data-ttu-id="d0202-117">[Meld u aan bij Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.</span><span class="sxs-lookup"><span data-stu-id="d0202-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="d0202-118">b.</span><span class="sxs-lookup"><span data-stu-id="d0202-118">b.</span></span> <span data-ttu-id="d0202-119">Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheerder**.</span><span class="sxs-lookup"><span data-stu-id="d0202-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="d0202-120">c.</span><span class="sxs-lookup"><span data-stu-id="d0202-120">c.</span></span> <span data-ttu-id="d0202-121">Vouw **Admin** en kiest u **Exchange**in de navigatie links.</span><span class="sxs-lookup"><span data-stu-id="d0202-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="d0202-122">d.</span><span class="sxs-lookup"><span data-stu-id="d0202-122">d.</span></span> <span data-ttu-id="d0202-123">Ga naar **beveiliging** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="d0202-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="d0202-124">e.</span><span class="sxs-lookup"><span data-stu-id="d0202-124">e.</span></span> <span data-ttu-id="d0202-125">Selecteer het domein en kies vervolgens **inschakelen** voor **berichten voor dit domein met DKIM handtekeningen ondertekenen**.</span><span class="sxs-lookup"><span data-stu-id="d0202-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="d0202-126">Herhaal deze stap voor elke aangepaste domein.</span><span class="sxs-lookup"><span data-stu-id="d0202-126">Repeat this step for each custom domain.</span></span>
