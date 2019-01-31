---
title: E-mailberichten naar de archiefmap Postvak verplaatsen
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660372"
---
<span data-ttu-id="b7f5b-p101">Problemen bij het archiveren van items in de postbus archiveren. Zorg ervoor dat u de volgende stappen hebt uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="b7f5b-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="b7f5b-p102">Bevestigen dat een **postbus archiveren** is ingeschakeld. Als dit niet het geval is, stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) gebruiken om te schakelen van de archiefmap Postvak.</span><span class="sxs-lookup"><span data-stu-id="b7f5b-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="b7f5b-106">In het beheercentrum van Exchange **Tags bewaren** onder **Beheer van de conformiteit**selecteert, een **inhouding code** maken met de actie **verplaatsen naar het archief** met de gewenste **Leeftijd vasthouden**.</span><span class="sxs-lookup"><span data-stu-id="b7f5b-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="b7f5b-107">Selecteer **Bewaarbeleid**in het beheercentrum van Exchange, **Bewaarbeleid** maken en uw behoud **verplaatsen naar archief** tag toevoegen aan dat beleid.</span><span class="sxs-lookup"><span data-stu-id="b7f5b-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="b7f5b-p103">[Het bewaarbeleid toewijzen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan de specifieke postbus van gebruiker. Hetzelfde beleid zullen worden toegepast op zowel de **primaire** als de **archiefmap** postvak.</span><span class="sxs-lookup"><span data-stu-id="b7f5b-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="b7f5b-p104">De postbus van gebruiker hebt nu een archiveringsbeleid items te verplaatsen naar de archiefmap Postvak. Deze zijn nodig om de beheerde map-assistent (MVR gesloten) uit te voeren en de nieuwe instellingen toepassen op het postvak van de gebruiker. Voer de volgende opdracht [verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tijdens het starten van de beheerde map-assistent van een bepaalde postbus:</span><span class="sxs-lookup"><span data-stu-id="b7f5b-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="b7f5b-113">Wilt u meer informatie over het instellen van een archiveringsbeleid, kunt u [een beleid voor archiveren en verwijderen van postbussen instellen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="b7f5b-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

