---
title: Groepsbeleid
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256713"
---
# <a name="group-policy"></a>Groepsbeleid

Instellingen voor gebruikers- en computerobjecten in Azure Active Directory Domain Services (Azure AD DS) worden vaak beheerd met GPOs (Group Policy Objects). Azure AD DS bevat ingebouwde GPOs voor de AADDC-gebruikers en AADDC-computerscontainers. U kunt deze ingebouwde GPOs aanpassen om groepsbeleid te configureren wanneer dat nodig is voor uw omgeving. Leden van de beheerdersgroep Azure AD DC hebben bevoegdheden voor groepsbeleidsbeheer in het Azure AD DS-domein en kunnen ook aangepaste GPOs- en organisatie-eenheden (OUs) maken. Zie overzicht van groepsbeleid voor meer informatie over wat groepsbeleid is en [hoe dit werkt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

In een hybride omgeving worden groepsbeleidsregels die zijn geconfigureerd in een on-premises AD DS-omgeving niet gesynchroniseerd met Azure AD DS. Als u configuratie-instellingen voor gebruikers of computers wilt definiëren in Azure AD DS, bewerkt u een van de standaard-GPOs's of maakt u een aangepast groep groep.

In dit [artikel wordt beschreven](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hoe u groepsbeleidsbeheerprogramma's installeert, hoe u de ingebouwde GPOS's bewerkt en hoe u aangepaste GPOs's maakt.



