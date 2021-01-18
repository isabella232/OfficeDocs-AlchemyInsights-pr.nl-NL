---
title: LDAP configureren
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884959"
---
# <a name="configure-ldap"></a>LDAP configureren

Ga als volgt te werk om LDAP te configureren:

1. Controleer de status van uw domein op de [Azure-Portal](https://aka.ms/aadds-health).
1. Er is een geldig Azure AD-abonnement beschikbaar en Azure AD Domain Services is ingeschakeld.
1. Het certificaat dat is vereist voor het inschakelen van beveiligde LDAP, moet afkomstig zijn van een vertrouwde openbare certificeringsinstantie of een zelfondertekend certificaat.
1. Zorg ervoor dat het certificaat de vereiste [richtlijnen](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)volgt.

**Ongeldig certificaat**
1. Als u een certificaat wilt verlengen, volgt u de stappen om een nieuw certificaat te maken en opnieuw te uploaden: [LDAP configureren](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Zie [LDAP-waarschuwingen oplossen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)voor informatie over het oplossen van een bekend probleem met beveiligde LDAP-waarschuwingen in azure Active Directory Domain Services.
