---
title: Er is een fout opgetreden bij het valideren van toegangs token tijdens het instappen in Desktop Analytics
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946610"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fout 'Er is een fout opgetreden bij het valideren van toegangs-token' tijdens de onboarding van Desktop Analytics

Deze fout wordt normaal gesproken waargenomen wanneer het verificatie-token verloopt. Meestal wordt het token vernieuwd door de pagina te vernieuwen. Dit probleem kan echter blijven bestaan als er beleid voor voorwaardelijke toegang is toegepast op het account dat wordt gebruikt voor desktopanalyse aan boord. U kunt de Aanmeldingslogboeken voor Azure AD bekijken in de Azure Portal om te zien of er aanmeldingsfouten zijn voor het account dat wordt gebruikt voor de onboarding van Desktop Analytics.

Ga naar Voorwaardelijke toegang plannen voor meer informatie over voorwaardelijke [toegang.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)