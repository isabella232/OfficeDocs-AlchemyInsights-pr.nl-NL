---
title: Automatische antwoorden instellen voor het postvak van een gebruiker
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
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506455"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="5bafc-102">Automatische antwoorden instellen voor het postvak van een gebruiker</span><span class="sxs-lookup"><span data-stu-id="5bafc-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="5bafc-103">**Methode 1**</span><span class="sxs-lookup"><span data-stu-id="5bafc-103">**Method 1**</span></span>

1. <span data-ttu-id="5bafc-104">Meld u aan bij de Office 365-portal.</span><span class="sxs-lookup"><span data-stu-id="5bafc-104">Sign in to the Office 365 portal.</span></span>

2. <span data-ttu-id="5bafc-105">Ga naar **Gebruikers > Actieve gebruikers** (of **Groepen > Gedeelde postvakken** als u dit instelt voor een gedeeld postvak).</span><span class="sxs-lookup"><span data-stu-id="5bafc-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="5bafc-106">Selecteer een gebruiker met een Microsoft Exchange-postvak.</span><span class="sxs-lookup"><span data-stu-id="5bafc-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="5bafc-107">Ga in het flyoutmenu aan de rechterkant naar **E-mailinstellingen > Automatische antwoorden** (als het een gedeeld postvak is, klikt u gewoon op **Automatische antwoorden** in de flyout).</span><span class="sxs-lookup"><span data-stu-id="5bafc-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="5bafc-108">**Methode 2**</span><span class="sxs-lookup"><span data-stu-id="5bafc-108">**Method 2**</span></span>

1. <span data-ttu-id="5bafc-109">Meld u aan bij de Office 365-beheerportal via beheerdersreferenties.</span><span class="sxs-lookup"><span data-stu-id="5bafc-109">Sign in to the Office 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="5bafc-110">Vouw **Beheercentrums** uit en klik vervolgens op **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="5bafc-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="5bafc-111">Klik in de rechterbovenhoek op de afbeelding, klik op **Andere gebruiker** en selecteer vervolgens het postvak van de gebruiker dat u wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="5bafc-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="5bafc-112">Selecteer aan de linkerkant **Opties**, klik op **E-mail ordenen** en klik vervolgens op **Automatische antwoorden.**</span><span class="sxs-lookup"><span data-stu-id="5bafc-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="5bafc-113">**Methode 3**</span><span class="sxs-lookup"><span data-stu-id="5bafc-113">**Method 3**</span></span>

<span data-ttu-id="5bafc-114">Voer de volgende cmdlet uit in Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="5bafc-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="5bafc-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="5bafc-115">PowerShellCopy</span></span>

    Set-MailboxAutoReplyConfiguration

<span data-ttu-id="5bafc-116">Zie [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) voor meer informatie over deze cmdlet.</span><span class="sxs-lookup"><span data-stu-id="5bafc-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
