---
title: Mijn app wordt niet weergegeven in App Governance
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454539"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Mijn app wordt niet weergegeven in App Governance

Als uw toepassing niet wordt weergegeven in App Governance, controleert u het volgende:

1. Ga naar [Azure AD](https://aad.portal.azure.com/) en zoek de app-id voor uw toepassing door te zoeken naar de naam van de app op de bovenste balk op de pagina Overzicht.

1. Access Graph Explorer en zoek naar de app-id binnen uw service-principal door deze query te gebruiken en te vervangen door de relevante <appId> app-id: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Als er geen resultaten worden geretourneerd, zoekt u naar de app-id in de toepassing door deze query te gebruiken en te vervangen door de relevante <appId> < https://graph.microsoft.com/v1.0/applications? app-id: $search= "appId: <appId> ">

Zie Ondersteuning krijgen als u problemen met de query [hebt.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Zie Meer informatie over zichtbaarheid en [inzichten](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)voor meer informatie of inzicht in uw apps in App Governance.

Zie Uw apps weergeven voor meer informatie over het weergeven [van uw apps.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
