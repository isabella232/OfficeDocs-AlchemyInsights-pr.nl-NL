---
title: DKIM instellen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509379"
---
# <a name="setup-dkim"></a>DKIM instellen

De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Microsoft 365 zijn [hier.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Voor **elk** aangepast domein moet u **twee** DKIM CNAME-records maken op de DNS-hostingservice van uw domein (meestal de domeinregistrar). contoso.com en fourthcoffee.com vereisen bijvoorbeeld vier DKIM CNAME-records: twee voor contoso.com en twee voor fourthcoffee.com.

   De DKIM CNAME-records voor **elk** aangepast domein gebruiken de volgende indelingen:

   - **Naam van de gastheer**:`selector1._domainkey.<CustomDomain>`

     **Adres- of waardepunten**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Naam van de gastheer**:`selector2._domainkey.<CustomDomain>`

     **Adres- of waardepunten**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>is de tekst links van `.mail.protection.outlook.com` in de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor het domein contoso.com). \<InitialDomain\>is het domein dat u hebt gebruikt toen u zich aanmeldde voor Microsoft 365 (bijvoorbeeld contoso.onmicrosoft.com).

2. Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies in:

   a. [meld u aan bij Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.

   b. Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheer**.

   c. Vouw in het navigatievenster aan de linkerkant **Beheerder** uit en kies **Exchange**.

   d. Ga naar **Bescherming**  >  **DKIM**.

   e. Selecteer het domein en kies **Vervolgens Berichten** voor **ondertekenen voor dit domein inschakelen met DKIM-handtekeningen**. Herhaal deze stap voor elk aangepast domein.
