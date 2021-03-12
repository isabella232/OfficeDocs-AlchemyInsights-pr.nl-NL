---
title: Tenantbeleid oplossen (actie overschrijven)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744478"
---
# <a name="fix-tenant-policy-action-override"></a>Tenantbeleid oplossen (actie overschrijven)

Dit bericht is beïnvloed door een antispambeleid in uw tenant. Ga als volgt te werk om het beleid te bekijken:

1. Ga naar het [Office 365-beveiligings- & compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga vervolgens naar **Threat management**  >  **Policy**  >  [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Controleer of **beleidsbron** het volgende aangeeft:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Als dat zo is, **controleert** u op het tabblad Aangepast de instellingen van het beleid dat van invloed is op het bericht. Het is mogelijk dat de standaardinstellingen **die** zijn toegepast op alle klanten van Exchange Online Protection, van invloed zijn op het bericht.

Zie Beleidsregels voor spamfilter configureren voor meer informatie over het configureren van beleidsregels voor [spamfilters.](https://go.microsoft.com/fwlink/?linkid=2101431)
