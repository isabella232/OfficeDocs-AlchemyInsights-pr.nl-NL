---
title: Implementatie van GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427257"
---
# <a name="gpo-deployment"></a>Implementatie van GPO

Instellingen voor gebruikers- en computerobjecten in Azure Active Directory Domain Services (Azure AD DS) worden vaak beheerd met GPOs (Group Policy Objects). Azure AD DS bevat ingebouwde GPOs voor de AADDC-gebruikers en AADDC-computerscontainers. U kunt deze ingebouwde GPOs aanpassen om groepsbeleid te configureren wanneer dat nodig is voor uw omgeving. Leden van de groep Azure AD DC-beheerders hebben beheerdersbevoegdheden voor groepsbeleid in het Azure AD DS-domein en kunnen ook aangepaste GPOs- en organisatie-eenheden (OUs) maken. Zie Overzicht van groepsbeleid voor meer informatie over wat groepsbeleid is en [hoe het werkt.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

In een hybride omgeving worden groepsbeleidsregels die zijn geconfigureerd in een on-premises AD DS-omgeving niet gesynchroniseerd met Azure AD DS. Als u configuratie-instellingen voor gebruikers of computers wilt definiëren in Azure AD DS, bewerkt u een van de standaard-GPOs's of maakt u een aangepast groep groep.

In dit [artikel wordt beschreven](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hoe u groepsbeleidsbeheerprogramma's installeert, hoe u de ingebouwde GPOS's bewerkt en hoe u aangepaste GPOs's maakt.
