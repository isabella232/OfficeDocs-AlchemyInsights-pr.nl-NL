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
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505681"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="dbdb3-102">Een verwijderde Microsoft 365-groep herstellen</span><span class="sxs-lookup"><span data-stu-id="dbdb3-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="dbdb3-103">U kunt een verwijderde Microsoft 365-groep of Microsoft Teams binnen 30 dagen na de verwijdering herstellen.</span><span class="sxs-lookup"><span data-stu-id="dbdb3-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="dbdb3-104">Als u zich wilt aanmelden bij het Microsoft 365-beheercentrum en een lijst wilt maken met de verwijderde groepen en teams, gaat u naar het [Microsoft 365-beheercentrum.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="dbdb3-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="dbdb3-105">**Opmerking:** Meld u aan met het account dat is toegewezen aan de tenantbeheerder of de beheerdersrol voor groepen.</span><span class="sxs-lookup"><span data-stu-id="dbdb3-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="dbdb3-106">Selecteer de verwijderde Microsoft 365-groep/Teams die u wilt herstellen en klik op **groep herstellen.**</span><span class="sxs-lookup"><span data-stu-id="dbdb3-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="dbdb3-107">Als de groep niet kan worden hersteld vanwege een conflicterend SMTP-adres, gebruikt u de volgende opdracht om het object te zoeken dat conflict veroorzaakt en het SMTP-adres te verwijderen:</span><span class="sxs-lookup"><span data-stu-id="dbdb3-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="dbdb3-108">**Opmerking:** In sommige gevallen kan het 24 uur duren voordat de groep en alle gegevens zijn hersteld.</span><span class="sxs-lookup"><span data-stu-id="dbdb3-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="dbdb3-109">Zie Een [verwijderde Microsoft 365-groep](https://go.microsoft.com/fwlink/?linkid=867802)herstellen voor meer informatie of voor meer informatie over het herstellen van groepen met PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dbdb3-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>