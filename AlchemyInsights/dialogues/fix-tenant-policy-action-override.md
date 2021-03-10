---
title: Tenantbeleid herstellen (actie overschrijven)
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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693256"
---
# <a name="fix-tenant-policy-action-override"></a>Tenantbeleid herstellen (actie overschrijven)

Dit bericht is beïnvloed door een antispambeleid in uw tenant. Ga als volgt te werk om het beleid te controleren:

1. Ga naar het [Office 365-& compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga naar Het beleid voor bedreigingsbeheer  >    >  [antispam.](https://go.microsoft.com/fwlink/?linkid=2101518)
2. Controleer of de **beleidsbron** het volgende aangeeft:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    Als dit het zo is, controleert u op **het** tabblad Aangepast de instellingen van het beleid dat van invloed is op het bericht. Mogelijk zijn de **standaardinstellingen** van toepassing op alle klanten van Exchange Online Protection die van invloed zijn op het bericht.

Zie Het spamfilterbeleid configureren voor meer informatie over het configureren van [spamfilterbeleid.](https://go.microsoft.com/fwlink/?linkid=2101431)
