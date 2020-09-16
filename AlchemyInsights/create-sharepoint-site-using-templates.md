---
title: Een site maken in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732213"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-sites maken met behulp van sjablonen

De mogelijkheid om een site op te slaan als een sjabloon, wordt niet ondersteund met moderne communicatie of team sites. Zie [een SharePoint-site opslaan, downloaden en uploaden als een sjabloon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)voor meer informatie over het gebruik van sjablonen.

Hier volgen enkele veelvoorkomende problemen en oplossingen in verband met het opslaan van een site of lijst als een sjabloon in SharePoint Online. 

**De knop site-of lijstsjabloon opslaan is niet beschikbaar of ontbreekt**

Beheerders moeten aangepaste scripts toestaan om de sjabloon functies in te schakelen. Zie voor gedetailleerde stappen, voorbeelden en overwegingen 

- [Aangepaste scripts toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- De opdracht site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de publicatie-infrastructuur van SharePoint Server.

**De sitesjabloon kan niet worden gemaakt of werkt niet goed**

De sjabloon mist mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd. Als de functie niet beschikbaar is voor het activeren van de huidige siteverzameling, kunt u de sitesjabloon niet gebruiken om een site te maken.

- Kijk of een lijst of bibliotheek de [drempelwaarde voor limieten voor de lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000-items mag overschrijden, omdat dit kan het maken van een sitesjabloon blokkeren.

- Het kan zijn dat op de site te veel resources worden gebruikt en de sitesjabloon daardoor groter is dan de limiet van 50 MB.


- Er zijn problemen met het weergeven van gegevens in een lijst die een opzoekkolom gebruikt. Zie voor meer informatie [sjabloon met gegenereerde lijst worden geen gegevens uit de juiste opzoeklijst weergegeven in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Raadpleeg [sitesjablonen maken en gebruiken](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)voor meer informatie over veelvoorkomende problemen en oplossingen.



