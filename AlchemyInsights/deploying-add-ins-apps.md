---
title: Invoegvoegingen implementeren voor Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124966"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Invoegvoegingen implementeren voor Microsoft 365-apps

Gecentraliseerde implementatie is de aanbevolen manier om Office te implementeren voor gebruikers en groepen binnen uw organisatie. Als u invoegvoegingen wilt implementeren, volgt u de onderstaande stappen:

**Opmerking:** Zie Invoegvoegingen weergeven, beheren en installeren in Office programma's als u invoegprogramma's wilt installeren voor Office [als individuele gebruiker.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Zorg er ook voor dat individuele overname van Office Store-invoegvoegingen is ingeschakeld. 

1. Zorg ervoor dat uw omgeving voldoet aan de vereisten voor de implementatie van invoegvoegingen met gecentraliseerde implementatie. Zie Vereisten voor [meer informatie.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Ga naar **Instellingen**  >  **Geïntegreerde apps Apps**  >  **downloaden** in het Microsoft 365-beheercentrum om invoegvoegingen te implementeren. 

Opmerkingen: 

- Geïntegreerde apps vereist dat de beheerder globale beheerders- of Exchange beheerdersmachtigingen heeft.

- Bij het implementeren van invoegvoegingen voor meerdere gebruikers is het raadzaam om opdrachten te maken met behulp van groepen in plaats van afzonderlijke gebruikers. Zie Overwegingen bij het toewijzen van een [invoegvoeging aan gebruikers en groepen](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)voor meer informatie.

- Gecentraliseerde implementatie biedt geen ondersteuning voor gebruikers in geneste groepen of groepen met bovenliggende groepen. Zie Gebruikers- en [groepstoewijzingen voor meer informatie.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Zorg ervoor dat de Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is ingeschakeld voor gebruikers om zich aan te melden. Zie App-eigenschappen [configureren voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Als u problemen hebt met het implementeren van invoegvoegingen met behulp van geïntegreerde apps, kunt u deze implementeren met behulp van [invoegvoegingen.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Zie voor meer informatie:

[Invoegvoegingen implementeren in het beheercentrum](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Invoegvoegingen beheren in het beheercentrum](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [De PowerShell-cmdlets voor](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) gecentraliseerde implementatie gebruiken om invoegingen te beheren 
 Invoeg Office via gecentraliseerde implementatie publiceren [via het Microsoft 365 beheercentrum](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Probleem oplossen: Gebruiker ziet geen invoegvoegingen](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Gebruikersfouten oplossen met Office-invoegingen](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)