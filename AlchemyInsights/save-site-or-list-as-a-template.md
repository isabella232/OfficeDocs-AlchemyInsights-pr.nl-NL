---
title: Site of lijst opslaan als sjabloon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727526"
---
# <a name="save-site-or-list-as-a-template"></a>Site of lijst opslaan als sjabloon

SharePoint-sitesjablonen zijn vooraf gedefinieerde definities voor een bepaalde zakelijke behoefte. Zie voor meer informatie [sjablonen gebruiken om verschillende soorten SharePoint-sites te maken](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Hier volgen enkele veelvoorkomende problemen en oplossingen in verband met het opslaan van een site of lijst als een sjabloon in SharePoint Online.

De **knop site-of lijstsjabloon opslaan is niet beschikbaar of ontbreekt**. 

- Beheerders moeten aangepaste scripts toestaan om de sjabloon functies in te schakelen. Zie voor meer informatie over voorbeelden en overwegingen [aangepaste scripts toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- De opdracht site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de publicatie-infrastructuur van SharePoint Server.


**De sitesjabloon kan niet worden gemaakt of werkt niet goed**

- De sjabloon mist mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd. Als de functie niet beschikbaar is voor het activeren van de huidige siteverzameling, kunt u de sitesjabloon niet gebruiken om een site te maken.


- Kijk of een lijst of bibliotheek de [drempelwaarde voor limieten voor de lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000-items mag overschrijden, omdat dit kan het maken van een sitesjabloon blokkeren.


- Het is mogelijk dat er te veel resources worden gebruikt op de site en dat de sitesjabloon de limiet van 50 MB (megabyte) overschrijdt.


- Er zijn problemen met het weergeven van gegevens in een lijst die een opzoekkolom gebruikt. Zie voor meer informatie [sjabloon met gegenereerde lijst worden geen gegevens uit de juiste opzoeklijst weergegeven in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Voor uitgebreide informatie over veelvoorkomende problemen en oplossingen raadpleegt [u sitesjablonen maken en gebruiken](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

