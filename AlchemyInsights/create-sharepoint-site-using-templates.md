---
title: Een site maken in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770418"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-sites maken met sjablonen

De mogelijkheid om een site op te slaan als sjabloon wordt niet ondersteund met moderne communicatie- of teamsites. Zie [Een SharePoint-site opslaan, downloaden en uploaden als sjabloon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)voor meer informatie over het gebruik van sjablonen.

Hier volgen enkele veelvoorkomende problemen/oplossingen met betrekking tot het opslaan van een site of lijst als sjabloon in Sharepoint Online. 

**Knop Site/lijstsjabloon opslaan is niet beschikbaar of ontbreekt**

Beheerders moeten Aangepast script toestaan om de sjabloonfuncties in te schakelen. Zie voor gedetailleerde stappen, voorbeelden en overwegingen 

- [Aangepast script toestaan of voorkomen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- De opdracht Site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die de publicatieinfrastructuur van SharePoint Server gebruiken.

**De sitesjabloon kan niet worden gemaakt of werkt niet correct**

De sjabloon mist mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd. Als de functie niet beschikbaar is om te activeren in de huidige siteverzameling, u de sitesjabloon niet gebruiken om een site te maken.

- Controleer of lijsten of bibliotheken de [drempelwaarde voor lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000 items overschrijden, omdat dit het maken van een sitesjabloon kan blokkeren.

- De site kan te veel bronnen gebruiken en daarom overschrijdt de sitesjabloon de limiet van 50 MB.


- Er zijn problemen met het weergeven van gegevens uit een lijst die een opzoekkolom gebruikt. Zie De [lijst met gegenereerde gegevens uit de juiste opzoeklijst in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)wordt niet weergegeven voor meer informatie.

Voor meer gedetailleerde informatie over veelvoorkomende problemen en oplossingen raadpleegt u [Sitesjablonen maken en gebruiken.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



