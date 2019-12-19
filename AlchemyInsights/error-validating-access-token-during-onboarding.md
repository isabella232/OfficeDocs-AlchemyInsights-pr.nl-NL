---
title: Er is een fout opgetreden bij het valideren van toegangstoken fout tijdens het on-boarding van Desktop Analytics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741154"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Foutbericht ' er is een fout bij het valideren van toegangstoken ' tijdens het onboarding van Desktop Analytics

Deze fout wordt meestal waargenomen wanneer het verificatietoken is verlopen. Normaalgesproken vernieuwen van de pagina wordt het token vernieuwd. Dit probleem kan echter blijven bestaan als er beleid voor voorwaardelijke toegang is toegepast op het account dat wordt gebruikt voor on-Board Desktop Analytics. U de Azure AD-aanmelding in de logboeken in de Azure-Portal om te zien of er fouten optreden voor het account dat wordt gebruikt voor de onboarding van Desktop Analytics controleren.

Ga naar de [implementatie van uw voorwaardelijke toegang plannen](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)voor meer informatie over voorwaardelijke toegang.