---
title: Een groep toevoegen aan een SharePoint-site
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758726"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Groep verbonden site in SharePoint Online maken

Er zijn een aantal veelvoorkomende problemen opgetreden bij het maken van of opnieuw een groep site verbonden.

 Als u een groep en haar verbonden site hebt verwijderd en een andere site te maken met dezelfde URL, moet u de vorige site permanent te verwijderen.

[Gesimuleerde Productieorder Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) downloaden

 Zie voor meer informatie over aan de slag met powershell, [aan de slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

De Site verwijderen uit Verwijderde Sites met behulp van de powershell-cmdlet [Verwijderen SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .

Als u een groep verbonden site maakt en u ontvangt een waarschuwing bestaat al een groep met dezelfde alias, controleert u de bestaande groepen uit de [Office 365 vanuit de Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). Het probleem is opgelost, de bestaande groep verwijderen als deze niet meer nodig is of de site maken met een ander alias toegewezen.

Er zijn verschillende manieren maken en moderne groepen gebruiken met SharePoint.

U kunt bestaande sites verbinden met een Office 365-groep. Zie [verbinding maken met een Office 365-groep met de SharePoint gebruiker ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer info.

Als een Office 365 groep verbonden site maakt, moet u een Team Site te maken. Zie voor meer info, [een team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).

