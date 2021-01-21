---
title: Levensduur van tokens configureren en verlengen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916824"
---
# <a name="configure-and-extend-token-lifetimes"></a>Levensduur van tokens configureren en verlengen

U kunt de levensduur opgeven van een toegangs-, SAML-of ID-token dat is uitgegeven door Microsoft Identity platform. U kunt token levensduur instellen voor alle apps in uw organisatie, voor een toepassing via meerdere tenants of voor een bepaalde service-principal in uw organisatie. Voor meer informatie raadpleegt u de [levensduur van configureerbare tokens](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Zie voorbeelden [van de levensduur van tokens configureren](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)voor voorbeelden.

Zie [tokens configureren in azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)voor informatie over het configureren van de levensduur en de compatibiliteit van een token in azure Active Directory B2C (Azure AD B2C).

In het artikel wordt het gedrag van de verbinding voor eenmalige aanmelding (SSO) van Azure [Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beschreven en kunt u de meest geschikte SSO-methode kiezen wanneer u uw beleid configureert.

**Hoelang duurt het zo lang? Hoelang zijn ze geldig?**

Levensduur van tokens zijn 1 uur en de levensduur van een sessie is 24 uur. Dit betekent dat als er geen aanvragen binnen 24 uur zijn ingediend, u opnieuw moet inloggen voordat u een nieuw token aanvraagt.

> [!NOTE]
> Na 30 mei 2020 kan geen nieuwe Tenant gebruikmaken van het beleid voor de levenscyclus van configureerbare tokens om sessie-en vernieuwingstokens te configureren. De afschaffing valt binnen enkele maanden, wat betekent dat we niet meer voldoen aan bestaande sessies en vernieuwingstokens. U kunt de levensduur van toegangstokens na de afschaffing nog steeds configureren.






