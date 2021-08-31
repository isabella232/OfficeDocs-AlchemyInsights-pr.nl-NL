---
title: Afbeelding van gebruiker die niet wordt weergegeven in Microsoft Teams organigram
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792691"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Afbeelding van gebruiker die niet wordt weergegeven in Microsoft Teams organigram

Als een of meer personen in uw organisatie hun profielfoto in het organigram missen, is het mogelijk dat de instelling **ShowInAddressLists** is ingesteld op **Onwaar:**

1. Ga naar Microsoft 365-beheercentrum > [**Actieve gebruikers**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)en selecteer de gebruiker met de ontbrekende foto. 
1. Selecteer het **tabblad E-mail** en zorg ervoor dat **Weergave in de algemene adreslijst** is ingesteld op **Ja.** 

Als Het **instellen van ShowInAddressLists** op **Ja** niet werkt, gaat u als volgt te werk:

- De gebruiker is mogelijk verborgen in de lijst met geadresseerden in Exchange. Zie Adreslijsten beheren [in Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- De gebruiker is mogelijk verborgen in de adreslijst in Azure Active Directory. Zie [Set-AzureADUser voor](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)meer informatie. 
