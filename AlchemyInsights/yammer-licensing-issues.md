---
title: Problemen met Yammer-licenties
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148237"
---
# <a name="yammer-licensing-issues"></a>Problemen met Yammer-licenties

Alle gebruikers moeten een licentie hebben om de Yammer Enterprise-service te gebruiken, maar standaard vereist Yammer niet dat gebruikers een licentie hebben om toegang te krijgen tot de service. Wanneer een beheerder de instelling wijzigt om Microsoft 365-gebruikers zonder Yammer-licenties te blokkeren, hebben gebruikers die geen Yammer Enterprise-licentie hebben toegewezen, geen toegang tot de Yammer-service. Zie [Yammer-gebruikerslicenties beheren in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) voor meer informatie 

Wanneer licenties van gebruikers worden verwijderd, wordt de Yammer-tegel niet meer weergegeven en kunnen andere services licentieverwijdering gebruiken om functies te verbergen. In andere gevallen kunnen functies nog steeds worden weergegeven, maar vereisen licentietoewijzing om te werken.  

**Licentie wordt niet bijgewerkt voor de gebruiker**  

Af en toe krijgt een gebruiker een licentie toegewezen, maar heeft hij nog steeds geen toegang tot Yammer. Vertragingen lopen vaker op wanneer er een massalicentietoewijzing aan de gang is. Yammer-gebruikers worden mogelijk niet in dezelfde volgorde bijgewerkt als licenties, worden gewijzigd in Azure AD omdat het systeem asynchroon wordt uitgevoerd. Wacht tot 24 uur voordat u een ondersteuningscase opent om problemen met licentiesynchronisatie te melden.  

**Toewijzing van bulklicenties**  

Licenties kunnen worden toegewezen via het beheercentrum of PowerShell-scripting. Zie [Licenties toewijzen aan gebruikers](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) en [Licenties toewijzen aan gebruikersaccounts met Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)voor meer informatie. 

Microsoft Support biedt geen hulp bij het maken van scripts, maar documentatie over Yammer-licentietoewijzing is beschikbaar. Zie [Yammer-licenties beheren met Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)voor meer informatie.