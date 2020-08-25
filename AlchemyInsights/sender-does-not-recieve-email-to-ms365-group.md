---
title: De afzender ontvangt geen e-mail die wordt verzonden naar de Microsoft 365-groep
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871728"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="75db9-102">De afzender ontvangt geen e-mail die wordt verzonden naar de Microsoft 365-groep</span><span class="sxs-lookup"><span data-stu-id="75db9-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="75db9-103">De afzender van een e-mailbericht aan een Microsoft 365-groep heeft standaard geen kopie van het bericht in het postvak in ontvangen, ook niet als de afzender lid is van de groep.</span><span class="sxs-lookup"><span data-stu-id="75db9-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="75db9-104">Gebruik deze EXO PowerShell-opdracht om ervoor te zorgen dat de afzender een kopie ontvangt van elk e-mailbericht dat ze verzenden naar de Microsoft 365-groep:</span><span class="sxs-lookup"><span data-stu-id="75db9-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="75db9-105">De instelling voor alle postvakken in één keer inschakelen:</span><span class="sxs-lookup"><span data-stu-id="75db9-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="75db9-106">**Opmerking** Het duurt maximaal een uur voordat deze instelling van kracht is.</span><span class="sxs-lookup"><span data-stu-id="75db9-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>