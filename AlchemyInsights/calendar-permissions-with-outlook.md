---
title: Agendamachtigingen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862058"
---
# <a name="calendar-permissions"></a>Agendamachtigingen

Gebruikers kunnen hun eigen agendamachtigingen wijzigen met Outlook op het web of andere clients, maar als beheerder moet u dit mogelijk ook onderzoeken.  
Met Exchange PowerShell-cmdlet ziet u de toestemming voor de agenda van een gebruiker:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Zie het volgende voor meer informatie:

- [Ophalen van postvakmappen Permissie](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-mailboxfolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Invoegpostenmappen](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Agendamachtigingen worden gebruikt bij het delen van agenda's, om meer informatie te zien over het delen van een Outlook-agenda, zie deze artikelen:

- [Een Outlook-agenda met anderen delen](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Uw agenda delen in de webversie van Outlook voor bedrijven](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Als u agendamachtiging wilt oplossen, u het hulpprogramma [Ondersteuning en Herstelassistent](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) gebruiken.