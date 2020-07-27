---
title: Meerdere gebruikers krijgen fout toegang geweigerd tijdens het toevoegen van invoegtoepassingen in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423482"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Meerdere gebruikers krijgen fout toegang geweigerd tijdens het toevoegen van invoegtoepassingen in Outlook

U opgeven welke beheerders in uw organisatie machtigingen hebben voor het installeren en beheren van invoegtoepassingen voor Outlook. U ook opgeven welke gebruikers in uw organisatie toestemming hebben om invoegtoepassingen voor eigen gebruik te installeren en te beheren.

Zie De [beheerders en gebruikers opgeven die invoegtoepassingen voor Outlook kunnen installeren en beheren voor](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)meer informatie.

Als u wilt controleren of u machtigingen voor een gebruiker hebt toegewezen, vervangt u <Role Name> de naam van de functie om te verifiëren en voert u de volgende opdracht uit in Exchange Online PowerShell:

Get-ManagementRoleAssignment -Rol " <Role Name> - GetEffectiveUsers

In dit voorbeeld ziet u hoe u controleert wie u machtigingen hebt toegewezen om invoegtoepassingen te installeren vanuit de Office Store voor de organisatie.

Powershell

-Rol "Org Marketplace Apps" -GetEffectiveUsers

Bekijk in de resultaten Get-ManagementRoleAssignment de vermeldingen in de kolom Effectieve gebruikers.

Zie [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)voor gedetailleerde syntaxis en parametergegevens .
 