---
title: Een groep toevoegen aan een SharePoint-site
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750515"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a>Problemen bij het maken of groeperen van verbonden sites in SharePoint Online

Er zijn een aantal veelvoorkomende problemen opgetreden bij het maken of opnieuw maken van een groep verbonden site.

 Als u een groep en de bijbehorende site hebt verwijderd en een andere site met dezelfde URL wilt maken, moet u de vorige site definitief verwijderen.

Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)

 Zie voor meer informatie over aan de slag met PowerShell, aan de [slag met SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)

De site verwijderen uit verwijderde sites met behulp van de [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell-cmdlet.

Als u een groep verbonden site maakt en een waarschuwing ontvangt een andere groep met dezelfde alias al bestaat, controleert u de bestaande groepen van de [Office 365 vanuit het Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups). U lost het probleem op door de bestaande groep te verwijderen als deze niet meer nodig is of de site te maken waaraan een andere alias is toegewezen.

Er zijn verschillende manieren om moderne groepen met SharePoint te maken en te gebruiken.

U bestaande sites verbinden met een Office 365-groep. Zie [een Office 365-groep verbinden met de SharePoint-gebruiker ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)voor meer informatie.

Als u een verbonden site van Office 365 groep wilt maken, moet u een team site maken. Zie [een team site maken in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)voor meer informatie.

