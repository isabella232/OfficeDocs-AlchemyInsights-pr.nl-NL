---
title: E-mailberichten verplaatsen naar het archief Postvak
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799775"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="46093-102">E-mail verplaatsen naar het archief Postvak</span><span class="sxs-lookup"><span data-stu-id="46093-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="46093-103">Als u wilt dat wij geautomatiseerde controles uitvoeren voor de instellingen die hieronder worden vermeld, selecteert u de knop terug <--boven aan deze pagina en voert u het e-mailadres in van de gebruiker die problemen heeft met het verplaatsen van e-mail naar het archief postvak.</span><span class="sxs-lookup"><span data-stu-id="46093-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="46093-104">Ga na of een **Archief postvak** is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="46093-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="46093-105">Als dat niet zo is, voert u de stappen in [dit artikel](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) uit om het archief postvak in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="46093-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="46093-106">Als u berichten automatisch wilt archiveren in het archief postvak, moet u een Bewaar label met de actie **verplaatsen naar archief** instellen om **automatisch toe te passen op een volledig postvak (standaard)**.</span><span class="sxs-lookup"><span data-stu-id="46093-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="46093-107">Voer de volgende stappen uit om de tag te maken: [standaardlabel voor archiveren](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="46093-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="46093-108">Vervolgens voegt u de tag **Archief** toe aan uw bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="46093-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="46093-109">Kies in het Exchange-Beheercentrum de optie **bewaarbeleid** > de **tag verplaatsen naar archief** toevoegen aan het beleid > **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="46093-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="46093-110">[Wijs het bewaarbeleid](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) nu toe aan het postvak van de specifieke gebruiker.</span><span class="sxs-lookup"><span data-stu-id="46093-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="46093-111">Het beleid wordt toegepast op zowel het **primaire** als het **Archief** postvak.</span><span class="sxs-lookup"><span data-stu-id="46093-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="46093-112">Mogelijk moet u de Managed folder Assistant (MFA) gebruiken om de nieuwe instellingen toe te passen op het postvak van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="46093-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="46093-113">Voer de volgende opdracht uit terwijl [u verbonden bent met Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) om de beheerde map voor een specifiek postvak te starten:</span><span class="sxs-lookup"><span data-stu-id="46093-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="46093-114">Start-ManagedFolderAssistant id <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="46093-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="46093-115">Zie voor meer informatie over het instellen van een archiefbeleid [een archief-en verwijderingsbeleid instellen voor postvakken](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="46093-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  