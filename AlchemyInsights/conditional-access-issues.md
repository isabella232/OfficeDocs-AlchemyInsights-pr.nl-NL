---
title: Problemen met voorwaardelijke toegang
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014786"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="8cad4-102">Problemen met voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="8cad4-102">Conditional access issues</span></span>

<span data-ttu-id="8cad4-103">**Problemen oplossen met de diagnostische gegevens**</span><span class="sxs-lookup"><span data-stu-id="8cad4-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="8cad4-104">U kunt snel nagaan wat er is gebeurd of problemen met de aanmelding van gebruikers oplossen met behulp van de [Diagnostische gegevens](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="8cad4-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="8cad4-105">Start de diagnostische aanmelding.</span><span class="sxs-lookup"><span data-stu-id="8cad4-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="8cad4-106">Zoek de gebeurtenis die u wilt analyseren door gegevens in te voeren die u hebt ingevoerd voor de gebruiker, toepassing, tijdstip van aanmelding, aanvraag-id of correlatie-id.</span><span class="sxs-lookup"><span data-stu-id="8cad4-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="8cad4-107">Bekijk de diagnostische resultaten met de details van wat er is gebeurd en welke acties u moet uitvoeren om wijzigingen aan te brengen (als u wijzigingen nodig hebt).</span><span class="sxs-lookup"><span data-stu-id="8cad4-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="8cad4-108">**Stappen voor het oplossen van problemen met een aanmelding**</span><span class="sxs-lookup"><span data-stu-id="8cad4-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="8cad4-109">Ga naar de aanmeldingspagina van Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8cad4-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="8cad4-110">Meld u aan op een gebruiker, tijdsbereik, toepassing, status, client-app, enzovoort.</span><span class="sxs-lookup"><span data-stu-id="8cad4-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="8cad4-111">Selecteer een aanmeld gebeurtenis en Bekijk het tabblad voorwaardelijke toegang om te zien welke beleidsregels zijn geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="8cad4-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="8cad4-112">Klik op de rij van een beleid om de beleidsdetails te bekijken en te begrijpen waarom de beleidsdetails zijn toegepast.</span><span class="sxs-lookup"><span data-stu-id="8cad4-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="8cad4-113">**Hulpmiddelen voor het oplossen van problemen met een voorwaardelijk toegangsbeleid**</span><span class="sxs-lookup"><span data-stu-id="8cad4-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="8cad4-114">Met de modus voor alleen rapporten kunt u een beleid evalueren zonder dat dit invloed heeft op de gebruikers.</span><span class="sxs-lookup"><span data-stu-id="8cad4-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="8cad4-115">Met What-als-functie kunt u aanmeld gebeurtenissen simuleren en bekijken welke beleidsregels van toepassing zijn.</span><span class="sxs-lookup"><span data-stu-id="8cad4-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="8cad4-116">De werkmap inzichten en rapporten laat de realtime impact van elk beleid weergeven.</span><span class="sxs-lookup"><span data-stu-id="8cad4-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="8cad4-117">**Beleidsregels voor basisbescherming**</span><span class="sxs-lookup"><span data-stu-id="8cad4-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="8cad4-118">Beleidsregels voor basisbescherming van basislijn zijn verouderd.</span><span class="sxs-lookup"><span data-stu-id="8cad4-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="8cad4-119">De persoon wordt niet meer afgedwongen en wordt binnenkort verwijderd van Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="8cad4-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="8cad4-120">U wordt aangeraden [beveiligingsstandaarden](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="8cad4-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="8cad4-121">Zie voor meer informatie over voorwaardelijke toegang:</span><span class="sxs-lookup"><span data-stu-id="8cad4-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="8cad4-122">[Aanbevolen procedures voor voorwaardelijke toegang in azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Voorwaarden in voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Besturingselementen in voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locaties in voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="8cad4-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
