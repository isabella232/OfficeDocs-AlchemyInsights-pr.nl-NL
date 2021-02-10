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
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="a7b79-102">Wachtwoord-hashsynchronisatie voor domeinservice</span><span class="sxs-lookup"><span data-stu-id="a7b79-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="a7b79-103">**Als uw Azure AD DS-exemplaar u vraagt wachtwoordhashsynchronisatie in teschakelen**</span><span class="sxs-lookup"><span data-stu-id="a7b79-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="a7b79-104">Er is een scenario waarin u een hybride omgeving gebruikt waarin gebruikers worden gesynchroniseerd vanuit een on-premises AD DS-omgeving (Azure Active Directory Domain Services).</span><span class="sxs-lookup"><span data-stu-id="a7b79-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="a7b79-105">Dit scenario doet zich voor ondanks dat u wachtwoordhashsynchronisatie hebt van de on-premises AD DS naar uw Azure AD-tenant.</span><span class="sxs-lookup"><span data-stu-id="a7b79-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="a7b79-106">**Oorzaak**</span><span class="sxs-lookup"><span data-stu-id="a7b79-106">**Cause**</span></span>

<span data-ttu-id="a7b79-107">Dit gebeurt omdat standaard de oude NTLM (New Technology LAN Manager) en Kerberos-wachtwoordhashes die nodig zijn voor Azure AD DS, niet worden gesynchroniseerd met Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a7b79-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="a7b79-108">**Tijdelijke oplossing**</span><span class="sxs-lookup"><span data-stu-id="a7b79-108">**Workaround**</span></span> 

<span data-ttu-id="a7b79-109">U moet Azure AD Connect configureren om de wachtwoordhashes te synchroniseren die nodig zijn voor NTLM- en Kerberos-verificatie.</span><span class="sxs-lookup"><span data-stu-id="a7b79-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="a7b79-110">Nadat Azure AD Connect is geconfigureerd, worden tijdens een on-premises account ook de oude wachtwoordhashes gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a7b79-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="a7b79-111">Zie hier [voor](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) meer informatie over dit en voor hulp bij het inschakelen van wachtwoordsynchronisatie in hybride Azure AD DS-omgevingen.</span><span class="sxs-lookup"><span data-stu-id="a7b79-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>