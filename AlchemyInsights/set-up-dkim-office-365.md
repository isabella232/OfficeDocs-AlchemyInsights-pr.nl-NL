---
title: Installatie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645667"
---
# <a name="setup-dkim"></a>Installatie DKIM

De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Microsoft 365 zijn [hier.](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)

1. Voor **elk** aangepast domein moet u **twee** DKIM CNAME-records maken op de DNS-hostingservice van uw domein (meestal de domeinregistrar). Voor contoso.com en fourthcoffee.com bijvoorbeeld vier DKIM CNAME-records: twee voor contoso.com en twee voor fourthcoffee.com.

   De DKIM CNAME-records voor **elk** aangepast domein gebruiken de volgende indelingen:

   - **Hostnaam**:`selector1._domainkey.<CustomDomain>`

     **Adres- of waardeaanspraken:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostnaam**:`selector2._domainkey.<CustomDomain>`

     **Adres- of waardeaanspraken:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> is de tekst `.mail.protection.outlook.com` links van in de aangepaste MX-record `contoso-com` voor het aangepaste domein (bijvoorbeeld voor het domein contoso.com). \<InitialDomain\> is het domein dat u hebt gebruikt toen u zich aanmeldde voor Microsoft 365 (bijvoorbeeld contoso.onmicrosoft.com).

2. Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies uit:

   a. [meld u aan bij Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.

   b. Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheer**.

   C. Vouw in het navigatievenster aan de linkerkant **Beheerder** uit en kies **Exchange**.

   D. Ga naar **Protection** > **DKIM**.

   E. Selecteer het domein en kies **Inschakelen** voor Berichten ondertekenen **voor dit domein met DKIM-handtekeningen**. Herhaal deze stap voor elk aangepast domein.
