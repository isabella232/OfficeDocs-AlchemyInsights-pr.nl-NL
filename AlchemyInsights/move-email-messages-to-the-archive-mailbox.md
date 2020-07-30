---
title: E-mailberichten verplaatsen naar het postvak Archiveren
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522766"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="aa8b8-102">E-mail verplaatsen naar het archiefpostvak</span><span class="sxs-lookup"><span data-stu-id="aa8b8-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="aa8b8-103">Als u wilt dat we geautomatiseerde controles uitvoeren voor de onderstaande instellingen, selecteert u de terugknop <- boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het verplaatsen van e-mail naar zijn archiefpostvak.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="aa8b8-104">Controleer of een **archiefpostvak** is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="aa8b8-105">Als dit niet het zo is, gebruikt u de stappen in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) om het archiefpostvak in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="aa8b8-106">Als u berichten automatisch wilt archiveren naar het archiefpostvak, moet een bewaartag met de actie **Verplaatsen naar archief** worden ingesteld om automatisch te worden toegepast op de tag hele **postvak (standaard).**</span><span class="sxs-lookup"><span data-stu-id="aa8b8-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="aa8b8-107">Gebruik de stappen hier om de tag te maken: [Archiefstandaardtag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="aa8b8-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="aa8b8-108">Voeg vervolgens de **archieftag** toe aan uw bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="aa8b8-109">Kies in het Exchange-beheercentrum **Bewaarbeleid** > voegt u de **tag Verplaatsen naar archief** toe aan het beleid > **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="aa8b8-110">[Wijs nu het bewaarbeleid toe](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan het postvak van de specifieke gebruiker.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="aa8b8-111">Hetzelfde beleid wordt toegepast op zowel het **postvak Primair** als **Archief.**</span><span class="sxs-lookup"><span data-stu-id="aa8b8-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="aa8b8-112">Het kan nodig zijn om de Managed Folder Assistant (MFA) te dwingen de nieuwe instellingen uit te voeren en toe te passen op het postvak van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="aa8b8-113">Voer de volgende opdracht uit terwijl [u is verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de assistent beheerde mappen voor een specifiek postvak te starten:</span><span class="sxs-lookup"><span data-stu-id="aa8b8-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="aa8b8-114">Start-ManagedFolderAssistant -Identiteit<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="aa8b8-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="aa8b8-115">Zie [Een archief- en verwijderingsbeleid voor postvakken instellen voor](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)meer informatie over het instellen van een archiefbeleid.</span><span class="sxs-lookup"><span data-stu-id="aa8b8-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  