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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Eén gebruiker ziet geen invoegtoepassingen in Outlook

De gebruiker maakt mogelijk deel uit van een rol die niet de juiste parameter AppsForOfficeEnabled heeft. Voer deze cmdlet uit om erachter te komen of de juiste rol is gekoppeld aan de gebruiker:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegeren van $false | Opmaak-tabel -Automatische rol,RoleAssigneeName,RoleAssigneeType

Zie [De beheerders en gebruikers opgeven die invoegtoepassingen voor Outlook kunnen installeren en beheren voor](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)meer informatie.
