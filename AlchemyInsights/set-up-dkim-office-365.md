---
title: DKIM instellen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808702"
---
# <a name="setup-dkim"></a>DKIM instellen

De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Microsoft 365 vindt u [hier](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Voor **elke** aangepaste domein moet u **twee** dkim CNAME-records maken bij de DNS-hostingservice van uw domein (meestal de domeinregistratie). Voorbeeld van contoso.com en fourthcoffee.com zijn er vier DKIM CNAME-records nodig: twee voor contoso.com en twee voor fourthcoffee.com.

   Voor de DKIM CNAME-records voor **elk** aangepast domein worden de volgende indelingen gebruikt:

   - **Naam host**: `selector1._domainkey.<CustomDomain>`

     **Verwijst naar adres of waarde**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Naam host**: `selector2._domainkey.<CustomDomain>`

     **Verwijst naar adres of waarde**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> de tekst links van `.mail.protection.outlook.com` de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor de domein contoso.com). \<InitialDomain\> het domein is dat u hebt gebruikt toen u zich aanmeldde voor Microsoft 365 (bijvoorbeeld contoso.onmicrosoft.com).

2. Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies uit:

   a. Meld u met uw werk-of schoolaccount [aan bij Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) .

   b. Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheer**.

   c. Vouw in het navigatievenster aan de linkerkant **Beheerder** uit en kies **Exchange**.

   d. Ga naar **Protection**  >  **dkim**.

   e. Selecteer het domein en kies vervolgens **inschakelen** voor **Onderteken berichten voor dit domein met dkim handtekeningen**. Herhaal deze stap voor elk aangepast domein.
