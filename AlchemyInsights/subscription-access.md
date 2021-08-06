---
title: Abonnementstoegang
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999235"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Kan Azure niet aanmelden vanwege browserproblemen (Browser blijft hangen, blijft draaien, wordt niet geladen, enz.)

Mogelijk wordt u beïnvloed door een uitval. Controleer of er een permanente uitval is: [Azure Health Status](https://status.azure.com/status/history/).

Meld u af bij alle actieve Azure-sessies. Start een in-private of incognitomodus van uw webbrowser.

U kunt ook proberen browser vernieuwen, een andere browser gebruiken, cachecookies verwijderen als bovenstaande niet werkt.

Meer informatie: [Aanmeldingsproblemen oplossen](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Geen toegang tot abonnementen**

Zorg er [in de Azure-portal](https://portal.azure.com/)voor dat de juiste Azure-adreslijst is geselecteerd vanuit het account rechtsboven.

Zorg er [in het Azure Account Center](https://account.windowsazure.com/Subscriptions)voor dat het gebruikte account de accountbeheerder is.

Meer informatie: [Problemen met geen abonnementen oplossen](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Geen toegang tot factureringsgeschiedenis**

De accountbeheerder moet ervoor zorgen dat de gebruiker die toegang heeft tot de factureringsgegevens wordt toegevoegd aan de Azure Active-adreslijst als gastgebruiker: Een nieuwe gebruiker [toevoegen of verwijderen.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)

De gebruiker moet dan een globale beheerdersrol krijgen: [Rol toewijzen aan gebruikers.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Aanbevolen documenten**

-   [Ik kan me niet aanmelden om mijn Azure-abonnement te beheren](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)