---
title: App Registration Client Secret or Certificate issues
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
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951488"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>App Registration Client Secret or Certificate issues

Verloopt het geheim van de toepassingsclient?

Ongeacht hoe de geregistreerde toepassing is gemaakt, hetzij via het standaardregistratieproces in de app-registratieportal of als de serviceprincipaal in uw tenant is gemaakt met toepassings toestemming, moet er een nieuwe clientgeheim worden gemaakt vóór het verlopen van de huidige toepassing en worden bijgewerkt in de bijbehorende toepassingscode. De maximale geldigheidsduur is 2 jaar. Ter herinnering: de geheime waarde moet worden opgenomen omdat deze niet meer zichtbaar is nadat u de pagina App-registraties in de portal hebt verlaten. Zie Snel [starten: Een app](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) registreren in de Microsoft identity platform en Best [practices voor de Microsoft identity platform.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)

Zie Een [Azure AD-app maken & service principal in de portal - Microsoft identity platform.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
