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
# <a name="calendar-permissions"></a><span data-ttu-id="ea288-102">Agendamachtigingen</span><span class="sxs-lookup"><span data-stu-id="ea288-102">Calendar Permissions</span></span>

<span data-ttu-id="ea288-103">Gebruikers kunnen hun eigen Agendamachtigingen wijzigen voor de webversie van Outlook of andere clients, maar als een beheerder die u ook moet onderzoeken.</span><span class="sxs-lookup"><span data-stu-id="ea288-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="ea288-104">Met een Exchange PowerShell-cmdlet ziet u de machtiging voor de agenda van een gebruiker:</span><span class="sxs-lookup"><span data-stu-id="ea288-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="ea288-105">Voor meer informatie raadpleegt u de volgende informatie:</span><span class="sxs-lookup"><span data-stu-id="ea288-105">To see more information see the following:</span></span>

- [<span data-ttu-id="ea288-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="ea288-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="ea288-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="ea288-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="ea288-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="ea288-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="ea288-109">Agendamachtigingen worden gebruikt in het delen van agenda's, zie de volgende artikelen voor meer informatie over het delen van een Outlook-agenda:</span><span class="sxs-lookup"><span data-stu-id="ea288-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="ea288-110">Een Outlook-agenda met anderen delen</span><span class="sxs-lookup"><span data-stu-id="ea288-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="ea288-111">Uw agenda delen in de webversie van Outlook voor bedrijven</span><span class="sxs-lookup"><span data-stu-id="ea288-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="ea288-112">Als u problemen met Agendamachtigingen wilt oplossen, kunt u het hulpprogramma voor [ondersteuning en de assistent voor ondersteuning](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) gebruiken.</span><span class="sxs-lookup"><span data-stu-id="ea288-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>