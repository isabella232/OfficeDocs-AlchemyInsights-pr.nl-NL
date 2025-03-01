---
title: Een groep toevoegen aan een SharePoint site
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318119"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Veelvoorkomende problemen bij het maken van een groep verbonden site in SharePoint

1. Als u een groep en de verbonden site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site definitief verwijderen.

   - [SPO Management Shell downloaden](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Zie Aan de slag met SharePoint Online Management Shell voor meer informatie over aan de slag [met Powershell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Verwijder de site van verwijderde sites met de [cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell is vereist om groepssites permanent te verwijderen.

1. Als u een groep verbonden site maakt en een waarschuwing ontvangt: Er bestaat al een andere groep met dezelfde **alias,** controleert u de bestaande groepen uit [de Microsoft 365-beheercentrum.](https://admin.microsoft.com/AdminPortal/Home#/groups) Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere alias toegewezen.

1. Er zijn verschillende manieren om moderne groepen te maken en te gebruiken met SharePoint.

   - U kunt bestaande sites koppelen aan een Microsoft 365 groep. Zie voor meer informatie [Verbinding maken een Microsoft 365 groep met de SharePoint gebruikersinterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Als u een Microsoft 365 met een groep verbonden site wilt maken, moet u een [teamsite maken.](https://admin.microsoft.com/sharepoint)
