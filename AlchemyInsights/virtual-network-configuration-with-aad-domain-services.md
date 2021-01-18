---
title: Virtuele configuratie met AAD-domeinservices
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884977"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuele configuratie met AAD-domeinservices

Virtuele configuratie met AAD-domein service omvat de volgende stappen: 

1. De status van uw domein controleren op de Azure-Portal https://aka.ms/aadds-health
2. Controleren van uw NSG voor regels waarmee de benodigde poorten voor synchronisatie in azure AD Domain Services op de portal worden geblokkeerd https://aka.ms/aadds-networking
3. Zorg ervoor dat uw virtuele netwerk in hetzelfde Azure-gebied is geïmplementeerd als uw Azure AD Domain Services-beheerd domein.
4. Zorg ervoor dat u geen bestaand domein hebt met dezelfde domeinnaam die beschikbaar is in het virtuele netwerk.

Zie voor meer informatie over het ontwerpen van de aandacht op het [virtuele netwerk van](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)Azure voor ondersteuning voor Aad Domain Services.

