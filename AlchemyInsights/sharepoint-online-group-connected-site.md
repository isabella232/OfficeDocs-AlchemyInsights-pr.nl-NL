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
ms.openlocfilehash: 049ef5acd80d64e00315ba07f274567e6a251904
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642139"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemen bij het maken van een met een groep verbonden site in SharePoint

1. Er zijn enkele veelvoorkomende problemen opgetreden bij het maken of opnieuw maken van een met een groep verbonden site.
Als u een groep en de bijbehorende site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site permanent verwijderen.

   - [SPO Management Shell downloaden](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Zie [Aan de slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)voor meer informatie over aan de slag met Powershell.
   - Verwijder de site uit verwijderde sites met de cmdlet [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell is vereist om groepssites permanent te verwijderen.

1. Als u een met een groep verbonden site maakt en een waarschuwing ontvangt: **een andere groep met dezelfde alias bestaat al,** controleert u de bestaande groepen in het Microsoft [365-beheercentrum](https://admin.microsoft.com/AdminPortal/Home#/groups). Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere alias toegewezen.

1. Er zijn verschillende manieren om moderne groepen te maken en te gebruiken met SharePoint.

   - U bestaande sites koppelen aan een Office 365-groep. Zie [Een Office 365-groep verbinden met de gebruikersinterface van SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie .
   - Als u een site met office 365-groep wilt maken, moet u een [teamsite maken.](https://admin.microsoft.com/sharepoint)
