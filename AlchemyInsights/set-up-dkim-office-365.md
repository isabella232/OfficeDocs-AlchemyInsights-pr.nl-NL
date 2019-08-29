---
title: DKIM instellen in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666259"
---
# <a name="setup-dkim-in-office-365"></a>DKIM instellen in Office 365

De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Office 365 zijn [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Voor **elk** aangepast domein moet u **twee** dkim CNAME-records maken in de DNS-hosting service van uw domein (meestal de domeinregistrar). Contoso.com en fourthcoffee.com vereisen bijvoorbeeld vier DKIM CNAME-records: twee voor contoso.com en twee voor fourthcoffee.com.

   De DKIM CNAME-records voor **elk** aangepast domein gebruiken de volgende notaties:

   - **Hostnaam**:`selector1._domainkey.<CustomDomain>`

     **Verwijst naar adres of waarde**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostnaam**:`selector2._domainkey.<CustomDomain>`

     **Verwijst naar adres of waarde**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<Domaingd\> is de tekst links van `.mail.protection.outlook.com` in de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor het domein contoso.com). \<InitialDomain\> is het domein dat u hebt gebruikt toen u zich aanmeldde voor Office 365 (bijvoorbeeld contoso.onmicrosoft.com).

2. Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies:

   A. [Meld u aan bij Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.

   B. Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheerder**.

   C. Vouw in de linkerbenedenhoek van de navigatie **admin** en kies **Exchange**.

   D. Ga naar **bescherming** > **dkim**.

   E. Selecteer het domein en kies vervolgens **inschakelen** voor **Aanmeldingsberichten voor dit domein met dkim-handtekeningen**. Herhaal deze stap voor elk aangepast domein.
