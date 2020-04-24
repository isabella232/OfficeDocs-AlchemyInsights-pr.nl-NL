---
title: Automatische antwoorden instellen voor een postvak
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788877"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="95554-102">Automatische antwoorden instellen voor het postvak van een gebruiker</span><span class="sxs-lookup"><span data-stu-id="95554-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="95554-103">**Methode 1**</span><span class="sxs-lookup"><span data-stu-id="95554-103">**Method 1**</span></span>

1. <span data-ttu-id="95554-104">Meld u aan bij de Microsoft 365-portal.</span><span class="sxs-lookup"><span data-stu-id="95554-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="95554-105">Ga naar **Gebruikers > Actieve gebruikers** (of **Groepen > Gedeelde postvakken** als u dit instelt voor een gedeeld postvak).</span><span class="sxs-lookup"><span data-stu-id="95554-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="95554-106">Selecteer een gebruiker met een Microsoft Exchange-postvak.</span><span class="sxs-lookup"><span data-stu-id="95554-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="95554-107">Ga in het flyoutmenu aan de rechterkant naar **E-mailinstellingen > Automatische antwoorden** (als het een gedeeld postvak is, klikt u gewoon op **Automatische antwoorden** in de flyout).</span><span class="sxs-lookup"><span data-stu-id="95554-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="95554-108">**Methode 2**</span><span class="sxs-lookup"><span data-stu-id="95554-108">**Method 2**</span></span>

1. <span data-ttu-id="95554-109">Meld u aan bij de Microsoft 365-beheerportal met uw beheerdersreferenties.</span><span class="sxs-lookup"><span data-stu-id="95554-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="95554-110">Vouw **Beheercentrums** uit en klik vervolgens op **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="95554-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="95554-111">Klik in de rechterbovenhoek op de afbeelding, klik op **Andere gebruiker** en selecteer vervolgens het postvak van de gebruiker dat u wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="95554-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="95554-112">Selecteer aan de linkerkant **Opties**, klik op **E-mail ordenen** en klik vervolgens op **Automatische antwoorden.**</span><span class="sxs-lookup"><span data-stu-id="95554-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="95554-113">**Methode 3**</span><span class="sxs-lookup"><span data-stu-id="95554-113">**Method 3**</span></span>

<span data-ttu-id="95554-114">Voer de volgende cmdlet uit in Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="95554-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="95554-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="95554-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="95554-116">Zie [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) voor meer informatie over deze cmdlet.</span><span class="sxs-lookup"><span data-stu-id="95554-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
