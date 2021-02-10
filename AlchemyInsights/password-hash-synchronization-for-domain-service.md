---
title: Wachtwoord-hashsynchronisatie voor domeinservice
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177417"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Wachtwoord-hashsynchronisatie voor domeinservice

**Als uw Azure AD DS-exemplaar u vraagt wachtwoordhashsynchronisatie in teschakelen**

Er is een scenario waarin u een hybride omgeving gebruikt waarin gebruikers worden gesynchroniseerd vanuit een on-premises AD DS-omgeving (Azure Active Directory Domain Services). Dit scenario doet zich voor ondanks dat u wachtwoordhashsynchronisatie hebt van de on-premises AD DS naar uw Azure AD-tenant.

**Oorzaak**

Dit gebeurt omdat standaard de oude NTLM (New Technology LAN Manager) en Kerberos-wachtwoordhashes die nodig zijn voor Azure AD DS, niet worden gesynchroniseerd met Azure AD Connect.

**Tijdelijke oplossing** 

U moet Azure AD Connect configureren om de wachtwoordhashes te synchroniseren die nodig zijn voor NTLM- en Kerberos-verificatie.

Nadat Azure AD Connect is geconfigureerd, worden tijdens een on-premises account ook de oude wachtwoordhashes gesynchroniseerd met Azure AD. Zie hier [voor](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) meer informatie over dit en voor hulp bij het inschakelen van wachtwoordsynchronisatie in hybride Azure AD DS-omgevingen.