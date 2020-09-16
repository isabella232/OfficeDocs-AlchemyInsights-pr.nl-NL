---
title: Een groep toevoegen aan een SharePoint-site
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771194"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemen bij het maken van een met een groep verbonden site in SharePoint

1. Enkele veelvoorkomende problemen die kunnen optreden bij het maken of opnieuw maken van een verbonden groepssite.
Als u een groep en de gekoppelde site hebt verwijderd en een andere site wilt maken met dezelfde URL, moet u de vorige site permanent verwijderen.

   - Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Zie aan de slag [met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)voor meer informatie over aan de slag met PowerShell.
   - Verwijder de site van verwijderde sites met behulp van de PowerShell [-cmdlet Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) . PowerShell is vereist voor het permanent verwijderen van groeps sites.

1. Als u een site met een groep wilt maken en een waarschuwing wilt ontvangen: er **bestaat al een andere groep met dezelfde alias**, Controleer de bestaande groepen in het [Microsoft 365-Beheercentrum](https://admin.microsoft.com/AdminPortal/Home#/groups). Als u het probleem wilt oplossen, verwijdert u de bestaande groep als deze niet meer nodig is of maakt u de site met een andere alias toegewezen.

1. U kunt moderne groepen met SharePoint op verschillende manieren maken en gebruiken.

   - U kunt bestaande sites verbinden met een Microsoft 365-groep. Zie [een Microsoft 365-groep verbinden met de gebruikersinterface van SharePoint](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie.
   - Als u een site met een Microsoft 365-groep wilt maken, moet u een [team site](https://admin.microsoft.com/sharepoint)maken.
