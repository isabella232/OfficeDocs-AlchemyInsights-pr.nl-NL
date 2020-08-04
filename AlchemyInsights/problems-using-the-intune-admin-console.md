---
title: Problemen met het gebruik van de Intune-beheerconsole
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555036"
---
# <a name="problems-using-the-intune-admin-console"></a>Problemen met het gebruik van de Intune-beheerconsole

**'Toegang geweigerd' bij het navigeren door de Intune-beheerportal.**

- Als u lid bent van een aangepaste Functie in Intune, moet u ervoor zorgen dat een Intune- of Enterprise Mobility Suite-licentie (EMS) aan uw account wordt toegewezen.
- Als u Configuration Manager gebruikt om apparaten te beheren, controleert u of u geen deel uitmaakt van de Intune-gebruikersverzameling voor Configuratiebeheer MDM.
- Controleer of u de juiste RBAC-machtigingen (Role-based Administration Control) hebt gekregen in het intune-rollenblad.
- Controleer of de gebruikte groep geen distributielijst is. Intune in de Azure-portal ondersteunt alleen gebruikersaccounts die deel uitmaken van Azure Active Directory-beveiligingsgroepen. Controleer uw groepen in de Azure-portal > **Intune-groepen**  >  **Groups**of in Azure-portal > Azure **Active Directory**.

**Gebruiker heeft te veel machtigingen voor toegewezen Intune-rol**

Adviseer de gebruiker om naar **Intune**  >  **Intune-rollen**te gaan  >  **Mijn machtigingen**  >  **exporteren** om verleende machtigingen te controleren.

**Ik heb een scopegroep aan een rol toegevoegd, maar gebruikers in die rol zien nog steeds andere gebruikers of apparaten.**

Scopegroepen filteren geen gebruikers of apparaten uit. Scopegroepen:

- Beperk aan wie gebruikers beleid of toepassingen kunnen toewijzen.
- Sta alleen specifieke gebruikers toe om externe taken uit te voeren op apparaten.

Zie [Role-based access control (RBAC) met Microsoft Intune voor](https://docs.microsoft.com/intune/role-based-access-control)meer informatie over scopegroepen.

**Ik heb een gebruiker toegevoegd aan een Intune-rol, maar ze hebben nog steeds volledige toegang tot de Intune-beheerconsole.**

Navigeer naar Intune > **Gebruikers** in de Azure-portal en controleer of de gebruiker niet is toegewezen aan een van de volgende rollen in de Azure-portal:

- Globale beheerder
- Intune-servicebeheerder
- SharePoint-beheerder

Zie [Role-based access control (RBAC) met Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control)voor meer informatie.

**Toegangsproblemen**

Zie [U zich niet aanmelden bij Office 365, Azure of Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)voor meer informatie.