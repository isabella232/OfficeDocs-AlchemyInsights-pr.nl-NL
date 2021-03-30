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
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404459"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>App Registration Client Secret or Certificate issues

Verloopt het geheim van de toepassingsclient?

Ongeacht hoe de geregistreerde toepassing is gemaakt, hetzij via het standaardregistratieproces in de app-registratieportal of als de serviceprincipaal in uw tenant is gemaakt met toepassings toestemming, moet er een nieuwe clientgeheim worden gemaakt vóór het verlopen van de huidige toepassing en worden bijgewerkt in de bijbehorende toepassingscode. De maximale geldigheidsduur is 2 jaar. Ter herinnering: de geheime waarde moet worden opgenomen omdat deze niet meer zichtbaar is nadat u de pagina App-registraties in de portal hebt verlaten. Zie Snel starten: Een app registreren op het [Microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) en [Best practices voor het Microsoft-identiteitsplatform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)voor meer informatie.

Zie Een [Azure AD-app maken & service principal in de portal - Microsoft-identiteitsplatform voor meer informatie.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)
