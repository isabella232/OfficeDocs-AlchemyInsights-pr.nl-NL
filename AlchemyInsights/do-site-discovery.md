---
title: Sitedetectie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692936"
---
# <a name="do-site-discovery"></a><span data-ttu-id="ae65c-102">Sitedetectie</span><span class="sxs-lookup"><span data-stu-id="ae65c-102">Do site discovery</span></span>

<span data-ttu-id="ae65c-103">Als uw organisatie nog steeds gebruikmaakt van oudere webtoepassingen en abonnementen voor het gebruik van de Internet Explorer-modus (wat de meeste klanten doen), moet u aanvullende sitedetectie uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="ae65c-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="ae65c-104">**U hebt al een oudere versie van Microsoft Edge geïmplementeerd**</span><span class="sxs-lookup"><span data-stu-id="ae65c-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="ae65c-105">Als u de lijst met ondernemingssite's al hebt geconfigureerd voor de oudere versie van Microsoft Edge, is uw sitedetectie bijna klaar.</span><span class="sxs-lookup"><span data-stu-id="ae65c-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="ae65c-106">Het enige wat u mogelijk moet doen, is het toevoegen van neutrale sites.</span><span class="sxs-lookup"><span data-stu-id="ae65c-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="ae65c-107">Neutrale sites zijn meestal sites die eenmalige aanmelding bieden.</span><span class="sxs-lookup"><span data-stu-id="ae65c-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="ae65c-108">Als u vanuit Microsoft Edge naar een neutrale site gaat, wilt u in Microsoft Edge blijven voor verificatie.</span><span class="sxs-lookup"><span data-stu-id="ae65c-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="ae65c-109">Als u naar een neutrale site gaat in de Internet Explorer-modus, wilt u in de Internet Explorer-modus blijven voor verificatie.</span><span class="sxs-lookup"><span data-stu-id="ae65c-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="ae65c-110">Identificeer eenmalige aanmelding of andere neutrale sites die u gebruikt en voeg deze toe aan uw lijst met ondernemingssites.</span><span class="sxs-lookup"><span data-stu-id="ae65c-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="ae65c-111">**Internet Explorer is uw standaardbrowser**</span><span class="sxs-lookup"><span data-stu-id="ae65c-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="ae65c-112">Als u nu alleen Internet Explorer gebruikt, weet u mogelijk niet welke sites zijn bijgewerkt naar moderne webstandaards en voor welke sites Internet Explorer nog steeds is vereist.</span><span class="sxs-lookup"><span data-stu-id="ae65c-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="ae65c-113">U zult deze sites willen zoeken en toevoegen aan de lijst met ondernemingssites, zodat u de Internet Explorer-modus alleen voor deze sites kunt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="ae65c-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="ae65c-114">[Met Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) worden sites gevonden die mogelijk de Internet Explorer-modus nodig hebben.</span><span class="sxs-lookup"><span data-stu-id="ae65c-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="ae65c-115">Het kan gegevens verzamelen op computers met Windows Internet Explorer 8 tot en met Internet Explorer 11 op Windows 10, Windows 8.1 of Windows 7.</span><span class="sxs-lookup"><span data-stu-id="ae65c-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="ae65c-116">**De gegevens analyseren**</span><span class="sxs-lookup"><span data-stu-id="ae65c-116">**Analyze the data**</span></span>

<span data-ttu-id="ae65c-117">Nadat u sitegegevens hebt verzameld, wordt u aangeraden de volgende vier stappen uit te zetten om de gegevens te analyseren:</span><span class="sxs-lookup"><span data-stu-id="ae65c-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="ae65c-118">Sorteer de gegevens op domein en vervolgens op URL.</span><span class="sxs-lookup"><span data-stu-id="ae65c-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="ae65c-119">Definieer de grenzen van een app die u wilt configureren voor de Internet Explorer-modus.</span><span class="sxs-lookup"><span data-stu-id="ae65c-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="ae65c-120">U wilt alle sites en webbesturingselementen opnemen die de app definiëren, maar u wilt geen extra sites en besturingselementen opnemen.</span><span class="sxs-lookup"><span data-stu-id="ae65c-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="ae65c-121">Sommige sites zijn zo eenvoudig als terwijl u voor andere sites meerdere sites en *https://contoso.com/app1* pagina's moet definiëren.</span><span class="sxs-lookup"><span data-stu-id="ae65c-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="ae65c-122">Test de app om te controleren of deze niet in het eigen land werkt.</span><span class="sxs-lookup"><span data-stu-id="ae65c-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="ae65c-123">Veel sites bieden moderne inhoud wanneer ze een moderne browser detecteren en bieden alleen verouderde inhoud wanneer Internet Explorer wordt gedetecteerd.</span><span class="sxs-lookup"><span data-stu-id="ae65c-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="ae65c-124">Voeg de app toe aan de lijst met ondernemingssite's als het testen mislukt.</span><span class="sxs-lookup"><span data-stu-id="ae65c-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="ae65c-125">U wordt daarom het beste alle sites in een app gegroepeerd.</span><span class="sxs-lookup"><span data-stu-id="ae65c-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="ae65c-126">Wanneer u een app upgradet, is het dan eenvoudiger om de hele site uit de Internet Explorer-modus te verwijderen en een moderne browser voor die app te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="ae65c-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="ae65c-127">Wanneer u klaar bent met sitedetectie en de gegevens hebt geanalyseerd, kunt u uw kanaalstrategie bekijken.</span><span class="sxs-lookup"><span data-stu-id="ae65c-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

