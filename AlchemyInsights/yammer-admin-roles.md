---
title: Informatie over Yammer-beheerders
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
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2021
ms.locfileid: "51035730"
---
# <a name="about-yammer-admins"></a>Informatie over Yammer-beheerders

**Netwerkbeheerders**

Globale beheerders worden automatisch gepromoveerd naar de rol geverifieerde beheerder in een Yammer-netwerk. In de volgende gevallen kan deze promotie niet correct worden uitgevoerd:

- Er bestaan meerdere Yammer-netwerken en de beheerder wordt aangemeld bij de verkeerde. [Netwerkconsolidatie](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is vereist om één Yammer-netwerk te kunnen gebruiken.
- Azure PIM wordt gebruikt. De gebruiker wordt mogelijk niet lang genoeg gepromoveerd tot globale beheerder om de promotie te kunnen doen. Een toekomstige update voor Yammer kan dit probleem oplossen, maar het is het beste om gebruikers handmatig te promoveren naar globale beheerder.
- Er is een synchronisatieprobleem met het Yammer-netwerk. In dit geval is een ondersteuningsaanvraag vereist voor verder onderzoek.

Zie Yammer-beheerders beheren voor meer informatie over [Yammer-beheerdersrollen.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)

**Groepsbeheerders**

Groepsbeheerders voor verbonden groepen van Microsoft 365 worden gesynchroniseerd met groepslidmaatschap vanuit Azure AD. Voor grote groepen kan deze synchronisatie een langere periode duren.
