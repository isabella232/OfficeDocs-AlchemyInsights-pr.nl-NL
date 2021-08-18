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
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897711"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Veelvoorkomende problemen bij het maken van een groep verbonden site in SharePoint

1. Als u een groep en de verbonden site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site definitief verwijderen.

   - [SPO Management Shell downloaden](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Zie Aan de slag met SharePoint [Online Management Shell voor](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)meer informatie over aan de slag met Powershell.
   - Verwijder de site van verwijderde sites met de [cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell. Powershell is vereist om groepssites permanent te verwijderen.

1. Als u een verbonden groepsite maakt en een waarschuwing ontvangt: Er bestaat al een andere groep met dezelfde **alias,** controleert u de bestaande groepen uit [de Microsoft 365-beheercentrum.](https://admin.microsoft.com/AdminPortal/Home#/groups) Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere alias toegewezen.

1. Er zijn verschillende manieren om moderne groepen te maken en te gebruiken met SharePoint.

   - U kunt bestaande sites koppelen aan een Microsoft 365 groep. Zie voor meer informatie [Verbinding maken een Microsoft 365 groep met de SharePoint gebruikersinterface.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Als u een Microsoft 365 groep verbonden site wilt maken, moet u een [teamsite maken.](https://admin.microsoft.com/sharepoint)
