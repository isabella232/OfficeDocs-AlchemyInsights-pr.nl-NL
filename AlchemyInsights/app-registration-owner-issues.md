---
title: Problemen met de eigenaar van app-registratie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404454"
---
# <a name="app-registration-owner-issues"></a>Problemen met de eigenaar van app-registratie

Hieronder volgen de beschikbare methoden om principals toe te voegen als eigenaren voor app-registraties:

- Azure AD PowerShell-module gebruiken -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Verwijzing: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI gebruiken - `az ad app owner add`

    Verwijzing: [eigenaar van az-ad-app](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graph gebruiken -

    Verwijzing: [Eigenaar toevoegen - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- De Azure AD Portal gebruiken: ga naar [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Selecteer uw toepassing > Eigenaren > Eigenaren toevoegen

**Kunt u uw toepassing niet weergeven op app-registraties, ook al bent u de eigenaar van die toepassing?**

Eigenaar van een app is geen administratieve rol. Als de instelling Toegang tot Azure AD-beheerportal beperken is ingeschakeld, kan alleen de beheerder de toepassingen bekijken in de app-registratieportal. [](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) Als een eigenaar de toepassingen wil kunnen bekijken, schakelt u deze instelling uit (Dit instellen op NEE) of wijst u de beheerdersrol toe aan de eigenaar voor alleen de specifieke toepassing. Hiervoor moet u echter een Azure AD Premium P2-licentie hebben en [Privileged Identity Management inschakelen.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
