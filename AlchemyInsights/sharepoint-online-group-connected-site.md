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
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719477"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Groep verbonden site in SharePoint Online maken

<p><strong>Er zijn een aantal veelvoorkomende problemen opgetreden bij het maken van of opnieuw een groep site verbonden.&nbsp;</strong></p>  <p>1.Als u een groep en haar verbonden site hebt verwijderd en een andere site te maken met dezelfde URL, moet u de vorige site permanent te verwijderen.</p>  <ul>  <li>Download <a title="gesimuleerde Productieorder Management Shell" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">Gesimuleerde Productieorder Management Shell</a> - Zie voor meer informatie over aan de slag met powershell, <a title="aan de slag met SharePoint Online Management Shell" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Aan de slag met SharePoint Online Management Shell</a>. <br /><br /></li>  <li>De Site verwijderen uit websites verwijderd met behulp van de <a title="verwijderen SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Verwijderen SPODeletedSite</a> powershell-cmdlet.</li>  </ul>  <p>Als u een groep verbonden site maakt en een waarschuwing <strong>'een andere groep met dezelfde alias al bestaat'</strong>wordt weergegeven, controleert u de bestaande groepen van de <a title="Office 365 vanuit het beheercentrum" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 vanuit de Admin Center</a>. Het probleem is opgelost, de bestaande groep verwijderen als deze niet meer nodig is of de site maken met een ander alias toegewezen.&nbsp;</p>  <p><strong>Er zijn verschillende manieren maken en moderne groepen gebruiken met SharePoint.&nbsp;</strong></p>  <ol>  <li>U kunt bestaande sites verbinden met een Office 365-groep. Zie voor meer info <a title="verbinding maken met een Office 365-groep met behulp van de SharePoint-gebruiker ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Verbinding maken met een Office 365-groep met de SharePoint gebruiker ineterface</a>.</li>  <li>Als een Office 365 groep verbonden site maakt, moet u een Team Site te maken. Zie voor meer info <a title="maken van een teamsite in SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Maak een teamsite in SharePoint.</a></li>  </ol>

