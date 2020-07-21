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
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Meerdere gebruikers zien geen invoegtoepassingen in Outlook

Als u Outlook-invoegtoepassingen en geen enkele test, als eerste stap voor het oplossen van problemen, gebruikt u de cmdlet **Get-OrganizationConfig** PowerShell om de parameter _AppsForOfficeEnabled_ op te vragen. Als de query een waarde van **False**retourneert, stelt u deze parameter in **op True** met behulp van de cmdlet **Set-OrganizationConfig,** zodat invoegtoepassingen worden weergegeven zoals verwacht.

We raden niet aan dat de parameter _AppsForOfficeEnabled_ is ingesteld op **False**. Een waarde van **False** overschrijft alle bovenstaande instellingen voor beheerders- en gebruikersrol en voorkomt dat nieuwe apps worden geactiveerd door een gebruiker in de organisatie.

Zie [De beheerders en gebruikers opgeven die invoegtoepassingen voor Outlook kunnen installeren en beheren](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)voor meer informatie.