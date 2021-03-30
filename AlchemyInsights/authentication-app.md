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
# <a name="authentication-app"></a>Verificatie-app

Als u een globale beheerder bent, kunt u snel weten wat er is gebeurd of problemen met het aanmelden van gebruikers opsporen met behulp van de [aanmeldingsdiagnose.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Start de diagnostische gegevens door op de knop[Diagnostische](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)gegevens starten te klikken. 
1. Zoek de gebeurtenis die u wilt analyseren door de gegevens in te dienen die u hebt over de gebruiker, de toepassing, het tijdstip van aanmelding, het aanvragen van id of correlatie-id.
1. Bekijk de diagnostische resultaten met de details van wat er is gebeurd en welke acties u kunt uitvoeren om wijzigingen aan te brengen, als er wijzigingen nodig zijn.

**Controleer het scenario dat van toepassing is:**

1. Als een gebruiker geen pushmelding ontvangt in de Microsoft Authenticator-app, controleert u of deze niet wordt weergegeven onder de MFA-geblokkeerde gebruikers, zoals beschreven in Gebruikers blokkeren en [deblokkeren.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Als de gebruiker niet is geblokkeerd voor MFA, maar geen pushmelding ontvangt, kan de gebruiker de Microsoft Authenticator-app openen, waarmee de goedkeuringsaanvragen in behandeling worden opvragen.
1. Als alternatieve aanmeldingsmethode kan de gebruiker ook op Op een andere manier op Aanmelden klikken en een verificatiecode kiezen uit mijn mobiele app.
1. De Microsoft Authenticator-app is de enige beschikbare methode voor veel gebruikers. [Meer informatie over beveiligingsinstellingen,](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)raadpleeg Veelgestelde vragen over [authenticator-apps](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) voor veelgestelde vragen en hoe u deze kunt oplossen.
 
**Aanbevolen video's**

[Authenticator-app instellen op een nieuwe telefoon (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).
