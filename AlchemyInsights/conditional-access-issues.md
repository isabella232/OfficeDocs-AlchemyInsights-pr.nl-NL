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
# <a name="conditional-access-issues"></a>Problemen met voorwaardelijke toegang

**Problemen oplossen met de diagnostische gegevens**

U kunt snel nagaan wat er is gebeurd of problemen met de aanmelding van gebruikers oplossen met behulp van de [Diagnostische gegevens](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).

1. Start de diagnostische aanmelding.
1. Zoek de gebeurtenis die u wilt analyseren door gegevens in te voeren die u hebt ingevoerd voor de gebruiker, toepassing, tijdstip van aanmelding, aanvraag-id of correlatie-id.
1. Bekijk de diagnostische resultaten met de details van wat er is gebeurd en welke acties u moet uitvoeren om wijzigingen aan te brengen (als u wijzigingen nodig hebt).

**Stappen voor het oplossen van problemen met een aanmelding** 

1. Ga naar de aanmeldingspagina van Azure AD.
1. Meld u aan op een gebruiker, tijdsbereik, toepassing, status, client-app, enzovoort.
1. Selecteer een aanmeld gebeurtenis en Bekijk het tabblad voorwaardelijke toegang om te zien welke beleidsregels zijn geëvalueerd.
1. Klik op de rij van een beleid om de beleidsdetails te bekijken en te begrijpen waarom de beleidsdetails zijn toegepast.

**Hulpmiddelen voor het oplossen van problemen met een voorwaardelijk toegangsbeleid**

- Met de modus voor alleen rapporten kunt u een beleid evalueren zonder dat dit invloed heeft op de gebruikers.
- Met What-als-functie kunt u aanmeld gebeurtenissen simuleren en bekijken welke beleidsregels van toepassing zijn.
- De werkmap inzichten en rapporten laat de realtime impact van elk beleid weergeven.

**Beleidsregels voor basisbescherming**

Beleidsregels voor basisbescherming van basislijn zijn verouderd. De persoon wordt niet meer afgedwongen en wordt binnenkort verwijderd van Azure Portal. U wordt aangeraden [beveiligingsstandaarden](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)in te schakelen.

Zie voor meer informatie over voorwaardelijke toegang:

[Aanbevolen procedures voor voorwaardelijke toegang in azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Voorwaarden in voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Besturingselementen in voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Locaties in voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
