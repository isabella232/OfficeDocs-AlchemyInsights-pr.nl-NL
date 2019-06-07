---
title: E-mailberichten naar de archiefmap Postvak verplaatsen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762360"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="0d43f-102">E-mail naar de archiefmap Postvak verplaatsen</span><span class="sxs-lookup"><span data-stu-id="0d43f-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="0d43f-103">Bevestigen dat een **postbus archiveren** is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="0d43f-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="0d43f-104">Als dat niet het geval is, volg de stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) de postbus archiveren inschakelen.</span><span class="sxs-lookup"><span data-stu-id="0d43f-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="0d43f-105">U archiveert berichten automatisch naar de archiefmap Postvak in, moet een label bewaren met de actie **verplaatsen om te archiveren** worden ingesteld op **automatisch naar het postvak in zijn geheel (standaard)-code wordt toegepast**.</span><span class="sxs-lookup"><span data-stu-id="0d43f-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="0d43f-106">De stappen hier gebruik maken van de code: [tag archief standaard](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="0d43f-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="0d43f-107">Voeg vervolgens de tag **archief** aan het bewaarbeleid.</span><span class="sxs-lookup"><span data-stu-id="0d43f-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="0d43f-108">Kies in het beheercentrum van Exchange **Bewaarbeleid** > de **verplaatsen naar archief tag** toevoegen aan het beleid > **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="0d43f-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="0d43f-109">Nu [het bewaarbeleid toewijzen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan de specifieke postbus van gebruiker.</span><span class="sxs-lookup"><span data-stu-id="0d43f-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="0d43f-110">Hetzelfde beleid zullen worden toegepast op zowel de **primaire** als de **archiefmap** postvak.</span><span class="sxs-lookup"><span data-stu-id="0d43f-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="0d43f-111">Deze zijn nodig om de beheerde map-assistent (MVR gesloten) uit te voeren en de nieuwe instellingen toepassen op het postvak van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="0d43f-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="0d43f-112">Voer de volgende opdracht [verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tijdens het starten van de beheerde map-assistent van een bepaalde postbus:</span><span class="sxs-lookup"><span data-stu-id="0d43f-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="0d43f-113">Zie voor meer informatie over het instellen van een archiveringsbeleid [instellen van een beleid voor archiveren en verwijderen van postvakken](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="0d43f-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

