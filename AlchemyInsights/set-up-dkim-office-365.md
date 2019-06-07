---
title: Setup DKIM in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764989"
---
# <a name="setup-dkim-in-office-365"></a>Setup DKIM in Office 365

De volledige instructies voor het configureren van DKIM voor aangepaste domeinen in Office 365 zijn [hier](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. U moet voor **elke** aangepaste domein maken **twee** DKIM CNAME-records van uw domein DNS-hostingservice (meestal de domeinregistratieservice). Bijvoorbeeld contoso.com en fourthcoffee.com vier DKIM CNAME-records vereist: twee voor contoso.com en twee voor fourthcoffee.com.

   De DKIM CNAME-records voor **elke** aangepaste domein gebruikt de volgende indelingen:

   - **Hostnaam**:`selector1._domainkey.<CustomDomain>`

     **Verwijst naar het adres of de waarde**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Hostnaam**:`selector2._domainkey.<CustomDomain>`

     **Verwijst naar het adres of de waarde**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> is de tekst links van `.mail.protection.outlook.com` in de aangepaste MX-record voor het aangepaste domein (bijvoorbeeld `contoso-com` voor het domein contoso.com). \<InitialDomain\> is het domein dat u hebt gebruikt toen u zich voor Office 365 (bijvoorbeeld contoso.onmicrosoft.com aanmeldde).

2. Nadat u de CNAME-records voor uw aangepaste domeinen hebt gemaakt, voert u de volgende instructies:

   een. [Meld u aan bij Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) met uw werk- of schoolaccount.

   b. Selecteer het pictogram voor het startprogramma voor apps in de linkerbovenhoek en kies **Beheerder**.

   c. Vouw **Admin** en kiest u **Exchange**in de navigatie links.

   d. Ga naar **beveiliging** > **DKIM**.

   e. Selecteer het domein en kies vervolgens **inschakelen** voor **berichten voor dit domein met DKIM handtekeningen ondertekenen**. Herhaal deze stap voor elke aangepaste domein.
