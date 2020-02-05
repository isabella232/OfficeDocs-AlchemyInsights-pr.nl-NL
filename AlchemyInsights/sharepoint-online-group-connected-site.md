---
title: Een groep toevoegen aan een SharePoint-site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: e7bfabe1555bb94e915f8544d460deecce6171be
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770346"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemen bij het maken van een met een groep verbonden site in SharePoint

1. Enkele veelvoorkomende problemen die zich voordoen bij het maken of opnieuw maken van een met een groep verbonden site.
Als u een groep en de verbonden site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site permanent verwijderen.

   - Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Zie Aan de [slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)voor meer informatie over aan de slag gaan met Powershell.
   - Verwijder de site van verwijderde sites met de [cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell is verplicht om groepssites permanent te verwijderen.

1. Als u een met een groep verbonden site maakt en een waarschuwing ontvangt: **er bestaat al een andere groep met dezelfde alias,** controleer de bestaande groepen uit office [365 vanuit het beheercentrum](https://admin.microsoft.com/AdminPortal/Home#/groups). Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere toegewezen alias.

1. Er zijn verschillende manieren om moderne groepen te maken en te gebruiken met SharePoint.

   - U bestaande sites verbinden met een Office 365-groep. Zie [Een Office 365-groep verbinden met de SharePoint-gebruikersinterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie.
   - Als u een met Office 365-groep verbonden site wilt maken, moet u een [teamsite](https://admin.microsoft.com/sharepoint)maken.
