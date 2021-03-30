---
title: Verificatie-app
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404598"
---
# <a name="authentication-app"></a><span data-ttu-id="fa407-102">Verificatie-app</span><span class="sxs-lookup"><span data-stu-id="fa407-102">Authentication app</span></span>

<span data-ttu-id="fa407-103">Als u een globale beheerder bent, kunt u snel weten wat er is gebeurd of problemen met het aanmelden van gebruikers opsporen met behulp van de [aanmeldingsdiagnose.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="fa407-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="fa407-104">Start de diagnostische gegevens door op de knop[Diagnostische](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)gegevens starten te klikken.</span><span class="sxs-lookup"><span data-stu-id="fa407-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="fa407-105">Zoek de gebeurtenis die u wilt analyseren door de gegevens in te dienen die u hebt over de gebruiker, de toepassing, het tijdstip van aanmelding, het aanvragen van id of correlatie-id.</span><span class="sxs-lookup"><span data-stu-id="fa407-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="fa407-106">Bekijk de diagnostische resultaten met de details van wat er is gebeurd en welke acties u kunt uitvoeren om wijzigingen aan te brengen, als er wijzigingen nodig zijn.</span><span class="sxs-lookup"><span data-stu-id="fa407-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="fa407-107">**Controleer het scenario dat van toepassing is:**</span><span class="sxs-lookup"><span data-stu-id="fa407-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="fa407-108">Als een gebruiker geen pushmelding ontvangt in de Microsoft Authenticator-app, controleert u of deze niet wordt weergegeven onder de MFA-geblokkeerde gebruikers, zoals beschreven in Gebruikers blokkeren en [deblokkeren.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="fa407-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="fa407-109">Als de gebruiker niet is geblokkeerd voor MFA, maar geen pushmelding ontvangt, kan de gebruiker de Microsoft Authenticator-app openen, waarmee de goedkeuringsaanvragen in behandeling worden opvragen.</span><span class="sxs-lookup"><span data-stu-id="fa407-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="fa407-110">Als alternatieve aanmeldingsmethode kan de gebruiker ook op Op een andere manier op Aanmelden klikken en een verificatiecode kiezen uit mijn mobiele app.</span><span class="sxs-lookup"><span data-stu-id="fa407-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="fa407-111">De Microsoft Authenticator-app is de enige beschikbare methode voor veel gebruikers.</span><span class="sxs-lookup"><span data-stu-id="fa407-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="fa407-112">[Meer informatie over beveiligingsinstellingen,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)raadpleeg Veelgestelde vragen over [authenticator-apps](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) voor veelgestelde vragen en hoe u deze kunt oplossen.</span><span class="sxs-lookup"><span data-stu-id="fa407-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="fa407-113">**Aanbevolen video's**</span><span class="sxs-lookup"><span data-stu-id="fa407-113">**Recommended Videos**</span></span>

<span data-ttu-id="fa407-114">[Authenticator-app instellen op een nieuwe telefoon (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="fa407-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
