---
title: Een verwijderde Microsoft 365-groep herstellen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645126"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="9fa8b-102">Een verwijderde Microsoft 365-groep herstellen</span><span class="sxs-lookup"><span data-stu-id="9fa8b-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="9fa8b-103">U kunt een verwijderde Microsoft 365-groep of Microsoft Teams binnen 30 dagen na de verwijdering herstellen.</span><span class="sxs-lookup"><span data-stu-id="9fa8b-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="9fa8b-104">Ga naar het [Microsoft 365-beheercentrum](https://aka.ms/RestoreDeletedGroup) om u aan te melden bij een lijst met de verwijderde groepen en teams.</span><span class="sxs-lookup"><span data-stu-id="9fa8b-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="9fa8b-105">**Opmerking:** Meld u aan met het account dat is toegewezen aan de tenantbeheerder of de beheerdersrol voor groepen.</span><span class="sxs-lookup"><span data-stu-id="9fa8b-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="9fa8b-106">Selecteer de verwijderde Microsoft 365-groep/Teams die u wilt herstellen en klik op **groep herstellen.**</span><span class="sxs-lookup"><span data-stu-id="9fa8b-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="9fa8b-107">Als de groep niet kan worden hersteld vanwege een conflicterend SMTP-adres, gebruikt u de volgende opdracht om het object te zoeken dat conflict veroorzaakt en het SMTP-adres te verwijderen:</span><span class="sxs-lookup"><span data-stu-id="9fa8b-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="9fa8b-108">**Opmerking:** In sommige gevallen kan het 24 uur duren voordat de groep en alle gegevens zijn hersteld.</span><span class="sxs-lookup"><span data-stu-id="9fa8b-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="9fa8b-109">Zie Een [verwijderde Microsoft 365-groep](https://go.microsoft.com/fwlink/?linkid=867802)herstellen voor meer informatie of voor meer informatie over het herstellen van groepen met PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9fa8b-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>