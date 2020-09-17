---
title: Er is een fout opgetreden bij het valideren van een toegangstoken fout tijdens de bureaublad analyse op het bord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783546"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fout ' er is een fout opgetreden bij het valideren van een toegangstoken ' tijdens de bureaublad analyse

Deze fout wordt normaal geconstateerd wanneer het authenticatietoken verloopt. Meestal wordt de token vernieuwd wanneer u de pagina vernieuwt. Dit probleem kan echter zich voordoen als er voorwaardelijke toegangsbeleidsregels gelden voor het account dat wordt gebruikt voor de on-board Analytics Desk. U kunt de aanmeldingslogboeken van Azure AD in de Azure-Portal bekijken om te zien of er aanmeldingsfouten zijn voor het account dat wordt gebruikt voor het onboarden van bureaublad analyses.

Ga naar [uw implementatie voor voorwaardelijke toegang plannen](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)voor meer informatie over voorwaardelijke toegang.