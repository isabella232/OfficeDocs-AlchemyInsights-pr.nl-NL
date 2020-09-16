---
title: Agendamachtigingen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748788"
---
# <a name="calendar-permissions"></a>Agendamachtigingen

Gebruikers kunnen hun eigen Agendamachtigingen wijzigen voor de webversie van Outlook of andere clients, maar als een beheerder die u ook moet onderzoeken.  
Met een Exchange PowerShell-cmdlet ziet u de machtiging voor de agenda van een gebruiker:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Voor meer informatie raadpleegt u de volgende informatie:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Agendamachtigingen worden gebruikt in het delen van agenda's, zie de volgende artikelen voor meer informatie over het delen van een Outlook-agenda:

- [Een Outlook-agenda met anderen delen](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Uw agenda delen in de webversie van Outlook voor bedrijven](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Als u problemen met Agendamachtigingen wilt oplossen, kunt u het hulpprogramma voor [ondersteuning en de assistent voor ondersteuning](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) gebruiken.