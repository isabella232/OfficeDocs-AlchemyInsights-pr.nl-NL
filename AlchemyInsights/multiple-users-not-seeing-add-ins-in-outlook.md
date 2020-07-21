---
title: Meerdere gebruikers zien geen invoegtoepassingen in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197840"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="d93e3-102">Meerdere gebruikers zien geen invoegtoepassingen in Outlook</span><span class="sxs-lookup"><span data-stu-id="d93e3-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="d93e3-103">Als u Outlook-invoegtoepassingen en geen enkele test, als eerste stap voor het oplossen van problemen, gebruikt u de cmdlet **Get-OrganizationConfig** PowerShell om de parameter _AppsForOfficeEnabled_ op te vragen.</span><span class="sxs-lookup"><span data-stu-id="d93e3-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="d93e3-104">Als de query een waarde van **False**retourneert, stelt u deze parameter in **op True** met behulp van de cmdlet **Set-OrganizationConfig,** zodat invoegtoepassingen worden weergegeven zoals verwacht.</span><span class="sxs-lookup"><span data-stu-id="d93e3-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="d93e3-105">We raden niet aan dat de parameter _AppsForOfficeEnabled_ is ingesteld op **False**.</span><span class="sxs-lookup"><span data-stu-id="d93e3-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="d93e3-106">Een waarde van **False** overschrijft alle bovenstaande instellingen voor beheerders- en gebruikersrol en voorkomt dat nieuwe apps worden geactiveerd door een gebruiker in de organisatie.</span><span class="sxs-lookup"><span data-stu-id="d93e3-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="d93e3-107">Zie [De beheerders en gebruikers opgeven die invoegtoepassingen voor Outlook kunnen installeren en beheren](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d93e3-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>