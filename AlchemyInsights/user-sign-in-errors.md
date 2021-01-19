---
title: Aanmeldingsfouten van gebruikers
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900856"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="bc9db-102">Aanmeldingsfouten van gebruikers</span><span class="sxs-lookup"><span data-stu-id="bc9db-102">User sign-in errors</span></span>

<span data-ttu-id="bc9db-103">**Problemen oplossen met de diagnostische gegevens**</span><span class="sxs-lookup"><span data-stu-id="bc9db-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="bc9db-104">Voer de volgende stappen uit om de oorzaak te bepalen of problemen met de gebruikersaanmelding op te sporen.</span><span class="sxs-lookup"><span data-stu-id="bc9db-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="bc9db-105">Start de [Diagnostische aanmelding](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="bc9db-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="bc9db-106">Zoek de gebeurtenis die u wilt analyseren door de details in te voeren voor de gebruiker, toepassing, tijdstip van aanmelden, aanvraag-id of correlatie-id.</span><span class="sxs-lookup"><span data-stu-id="bc9db-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="bc9db-107">Bekijk de diagnostische resultaten met de details van wat er is gebeurd en welke acties u moet uitvoeren om wijzigingen aan te brengen, indien nodig wijzigingen.</span><span class="sxs-lookup"><span data-stu-id="bc9db-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="bc9db-108">**Zoeken naar informatie over de AADSTS-foutcodes die worden geretourneerd via de Azure Active Directory (Azure AD) beveiligingstokenservice (STS)?**</span><span class="sxs-lookup"><span data-stu-id="bc9db-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="bc9db-109">Lees [dit artikel](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) om AADSTS-fout beschrijvingen, fixes en enkele voorgestelde tijdelijke oplossingen te vinden</span><span class="sxs-lookup"><span data-stu-id="bc9db-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>