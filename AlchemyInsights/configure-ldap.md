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
# <a name="configure-ldap"></a><span data-ttu-id="8c8ff-102">LDAP configureren</span><span class="sxs-lookup"><span data-stu-id="8c8ff-102">Configure LDAP</span></span>

<span data-ttu-id="8c8ff-103">Ga als volgt te werk om LDAP te configureren:</span><span class="sxs-lookup"><span data-stu-id="8c8ff-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="8c8ff-104">Controleer de status van uw domein op de [Azure-Portal](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="8c8ff-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="8c8ff-105">Er is een geldig Azure AD-abonnement beschikbaar en Azure AD Domain Services is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="8c8ff-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="8c8ff-106">Het certificaat dat is vereist voor het inschakelen van beveiligde LDAP, moet afkomstig zijn van een vertrouwde openbare certificeringsinstantie of een zelfondertekend certificaat.</span><span class="sxs-lookup"><span data-stu-id="8c8ff-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="8c8ff-107">Zorg ervoor dat het certificaat de vereiste [richtlijnen](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)volgt.</span><span class="sxs-lookup"><span data-stu-id="8c8ff-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="8c8ff-108">**Ongeldig certificaat**</span><span class="sxs-lookup"><span data-stu-id="8c8ff-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="8c8ff-109">Als u een certificaat wilt verlengen, volgt u de stappen om een nieuw certificaat te maken en opnieuw te uploaden: [LDAP configureren](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8c8ff-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="8c8ff-110">Zie [LDAP-waarschuwingen oplossen](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)voor informatie over het oplossen van een bekend probleem met beveiligde LDAP-waarschuwingen in azure Active Directory Domain Services.</span><span class="sxs-lookup"><span data-stu-id="8c8ff-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
