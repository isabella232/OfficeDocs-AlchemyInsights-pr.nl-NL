---
title: E-mailberichten verplaatsen naar het postvak Archief
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713641"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="85059-102">E-mail verplaatsen naar het archiefpostvak</span><span class="sxs-lookup"><span data-stu-id="85059-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="85059-103">Controleer of een **archiefpostvak** is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="85059-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="85059-104">Als dit niet het zo is, gebruikt u de stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) om het archiefpostvak in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="85059-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="85059-105">Als u berichten automatisch wilt archiveren in het archiefpostvak, moet een bewaartag met de actie **Verplaatsen naar archief** automatisch worden toegepast op de volledige tag van het postvak **(standaard).**</span><span class="sxs-lookup"><span data-stu-id="85059-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="85059-106">Gebruik de stappen hier om de tag te maken: [Archive default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="85059-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="85059-107">Voeg vervolgens de **archieftag** toe aan uw bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="85059-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="85059-108">Kies in het Exchange-beheercentrum **Bewaarbeleid** > de **tag Verplaatsen naar archief** toevoegen aan het beleid > **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="85059-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="85059-109">[Wijs nu het bewaarbeleid toe](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan het postvak van de specifieke gebruiker.</span><span class="sxs-lookup"><span data-stu-id="85059-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="85059-110">Hetzelfde beleid wordt toegepast op zowel het **postvak Primair** als **archief.**</span><span class="sxs-lookup"><span data-stu-id="85059-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="85059-111">Het kan nodig zijn om de Managed Folder Assistant (MFA) uit te voeren en de nieuwe instellingen toe te passen op het postvak van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="85059-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="85059-112">Voer de volgende opdracht uit terwijl [u bent verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de beheerde mapassistent voor een specifiek postvak te starten:</span><span class="sxs-lookup"><span data-stu-id="85059-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="85059-113">Start-ManagedFolderAssistant -Identiteit<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="85059-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="85059-114">Zie [Een archief- en verwijderingsbeleid instellen voor postvakken voor](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)meer informatie over het instellen van een archiefbeleid.</span><span class="sxs-lookup"><span data-stu-id="85059-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  