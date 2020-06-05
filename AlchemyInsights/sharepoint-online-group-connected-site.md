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
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582806"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemen bij het maken van een met groepen verbonden site in SharePoint

1. Er zijn veelvoorkomende problemen bij het maken of opnieuw maken van een groepsgekoppelde site.
Als u een groep en de verbonden site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site permanent verwijderen.

   - [SPO Management Shell downloaden](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Zie [Aan de slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)voor meer informatie over aan de slag met Powershell.
   - Verwijder de site uit verwijderde sites met de [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell-cmdlet. Powershell is vereist om groepssites permanent te verwijderen.

1. Als u een met groep verbonden site maakt en een waarschuwing ontvangt: **een andere groep met dezelfde alias bestaat al,** controleert u de bestaande groepen vanuit het Microsoft [365-beheercentrum](https://admin.microsoft.com/AdminPortal/Home#/groups). Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet langer nodig is of maakt u de site met een andere alias toegewezen.

1. Er zijn verschillende manieren om moderne groepen te maken en te gebruiken met SharePoint.

   - U bestaande sites koppelen aan een Microsoft 365-groep. Zie [Een Microsoft 365-groep verbinden met de Gebruikersinterface van SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie.
   - Als u een door Microsoft 365-groep verbonden site wilt maken, moet u een [teamsite maken.](https://admin.microsoft.com/sharepoint)
