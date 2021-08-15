---
title: Kan niet aanmelden bij Teams vanwege fout autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038395"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Kan niet aanmelden bij Teams vanwege fout autologon.microsoftazuread-sso dot com:443

Als naadloze SSO is ingeschakeld als O365-verificatie, moet de URL 'autologon.microsoftazuread-sso.com ' mogelijk worden toegevoegd aan intranet sites.  Als deze eerder is toegevoegd aan vertrouwde websites en naadloze SSO wordt gebruikt, moet deze worden verwijderd uit vertrouwde sites.

Bekijk de [Controlelijst voor probleemoplossing bij naadloze SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Voer de volgende stappen uit om een URL toe te voegen aan de lijst met intranet sites:

1. Open Internet Explorer door te klikken op de knop **Start**. Typ in het zoekvak Internet Explorer en klik vervolgens in de lijst met resultaten op **Internet Explorer**.
2. Klik op het menu **Extra** en klik vervolgens op **Internetopties**.
3. Klik op het tabblad **Beveiliging**.
4. Klik nu op **Lokale intranet sites** en klik vervolgens op de knop **Sites** en vervolgens op **Geavanceerd**.
5. Voer de URL van de website in en klik op **Toevoegen**.
6. Als u gereed bent, klikt u op **Sluiten**.

Zie voor meer informatie [Documentatie voor het implementeren van de naadloze SSO voor O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (dit omvat een op beleid gebaseerd proces voor het toevoegen van een URL aan intranet sites in Stap 3).
