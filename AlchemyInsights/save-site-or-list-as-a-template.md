---
title: Site of lijst opslaan als sjabloon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048719"
---
# <a name="save-site-or-list-as-a-template"></a>Site of lijst opslaan als sjabloon

SharePoint-sitesjablonen zijn vooraf gedefinieerde definities die zijn ontworpen rond een bepaalde zakelijke behoefte. Zie [sjablonen gebruiken om verschillende soorten SharePoint-sites te maken](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)voor meer informatie.

Hier volgen enkele veelvoorkomende problemen/oplossingen met betrekking tot het opslaan van een site of lijst als een sjabloon in SharePoint Online.

De **knop site/lijstsjabloon opslaan is niet beschikbaar of ontbreekt**. 

- Beheerders moeten het aangepaste script toestaan om de sjabloonfuncties in te schakelen. Zie voor gedetailleerde stappen, voorbeelden en overwegingen [toestaan of voorkomen dat aangepast script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- De opdracht site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de SharePoint Server Publishing-infrastructuur.


**De sitesjabloon kan niet worden gemaakt of werkt niet correct**

- De sjabloon ontbreekt mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd. Als de functie niet beschikbaar is om te activeren in de huidige siteverzameling, u de sitesjabloon niet gebruiken om een site te maken.


- Controleer of er lijsten of bibliotheken zijn die de [limiet drempel voor lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000 items overschrijden, omdat hierdoor het maken van een sitesjabloon kan worden geblokkeerd.


- De site gebruikt mogelijk te veel bronnen en daarom overschrijdt de sitesjabloon de limiet van 50 megabyte (MB).


- Er zijn problemen met het weergeven van gegevens uit een lijst die gebruikmaakt van een opzoekkolom. Zie voor meer informatie, [sjabloon gegenereerde lijstgegevens uit de juiste opzoeklijst in SharePoint Online niet weergegeven](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Voor meer gedetailleerde informatie over veelvoorkomende problemen en oplossingen raadpleegt u [sitesjablonen maken en gebruiken](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

