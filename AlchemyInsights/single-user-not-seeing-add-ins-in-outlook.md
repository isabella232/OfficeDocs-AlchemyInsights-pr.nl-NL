---
title: Eén gebruiker ziet geen invoegtoepassingen in Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197832"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="fc1dd-102">Eén gebruiker ziet geen invoegtoepassingen in Outlook</span><span class="sxs-lookup"><span data-stu-id="fc1dd-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="fc1dd-103">De gebruiker maakt mogelijk deel uit van een rol die niet de juiste parameter AppsForOfficeEnabled heeft.</span><span class="sxs-lookup"><span data-stu-id="fc1dd-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="fc1dd-104">Voer deze cmdlet uit om erachter te komen of de juiste rol is gekoppeld aan de gebruiker:</span><span class="sxs-lookup"><span data-stu-id="fc1dd-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="fc1dd-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegeren van $false | Opmaak-tabel -Automatische rol,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="fc1dd-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="fc1dd-106">Zie [De beheerders en gebruikers opgeven die invoegtoepassingen voor Outlook kunnen installeren en beheren voor](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fc1dd-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
