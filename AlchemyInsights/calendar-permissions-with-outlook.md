---
title: Agendamachtigingen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046099"
---
# <a name="calendar-permissions"></a>Agendamachtigingen

Gebruikers kunnen hun eigen agendamachtigingen wijzigen met Outlook op internet of andere clients, maar als beheerder moet u dit mogelijk ook onderzoeken.  
Met Exchange PowerShell-cmdlet ziet u de machtiging voor de agenda van een gebruiker:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Zie het volgende voor meer informatie:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Agendamachtigingen worden gebruikt voor het delen van agenda's, zie deze artikelen voor meer informatie over het delen van een Outlook agenda:

- [Een Outlook-agenda met anderen delen](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Uw agenda delen in webversie van Outlook voor Bedrijven](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Als u problemen wilt oplossen met agendamachtigingen, [kunt u het Ondersteunings- en herstelassistent](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) gebruiken.