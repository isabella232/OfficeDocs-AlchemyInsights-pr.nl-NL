---
title: Gebruikersafbeelding wordt nog steeds weergegeven in het Microsoft Teams organigram
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422213"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Gebruikersafbeelding wordt nog steeds weergegeven in het Microsoft Teams organigram

Als een of meer personen in uw organisatie zijn uitgeschakeld of verwijderd en hun profielfoto nog steeds wordt weergegeven in de organigram, is het mogelijk dat de instelling **ShowInAddressLists** is ingesteld op Onwaar: 

1. Ga naar Microsoft 365-beheercentrum > [Actieve gebruikers](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) en selecteer de gebruiker met de foto die nog steeds wordt weergegeven. 
1. Selecteer het **tabblad E-mail** en zorg ervoor dat **Weergave in de algemene adreslijst** is ingesteld op **Nee.**

Als Het instellen **van ShowInAddressLists** op **Nee** niet werkt, controleert u het volgende: 

- De gebruiker wordt mogelijk weergegeven vanuit de lijst met geadresseerden in Exchange. Zie Adreslijsten beheren [in Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- De gebruiker wordt mogelijk weergegeven vanuit de adreslijst in Azure Active Directory. Zie [Set-AzureADUser voor](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)meer informatie. 