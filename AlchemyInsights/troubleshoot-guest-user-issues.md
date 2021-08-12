---
title: Problemen met gastgebruikers oplossen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939374"
---
# <a name="troubleshoot-guest-user-issues"></a>Problemen met gastgebruikers oplossen

1. Zie Gasttoegang beheren met [Azure AD-toegangsbeoordelingen](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)voor informatie over het beheren van gasttoegang tot toepassingen.
1. Gastgebruikers toevoegen aan uw adreslijst in de [Azure-portal:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)in dit snelstartproces voegt u een nieuwe gastgebruiker toe aan uw Azure AD-adreslijst via de Azure-portal, verzendt u een uitnodiging en ziet u hoe het inwisselingsproces van de gastgebruiker eruitziet.
1. [Een gastgebruiker toevoegen met PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)in deze snelstart gebruikt u de opdracht New-AzureADMSInvitation om één gastgebruiker toe te voegen aan uw Azure-tenant.
1. Zie Gebruikerstoewijzing voor een app beheren in Azure Active Directory (Azure AD) vanuit de Azure-portal of met PowerShell voor meer informatie over het toewijzen van gebruikers en groepen aan ondernemingstoepassingen [in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory B2B-samenwerking (Azure AD) werkt met de meeste apps die zijn geïntegreerd met Azure AD. In dit [artikel lezen](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)we instructies voor het configureren van enkele populaire SaaS-apps voor gebruik met Azure AD B2B.
1. Als een organisatie die Azure Active Directory (Azure AD) B2B-samenwerkingsmogelijkheden gebruikt om gastgebruikers van partnerorganisaties uit te nodigen voor uw Azure AD, kunt u deze B2B-gebruikers nu toegang geven tot on-premises apps. Deze on-premises apps kunnen SAML-verificatie of Integrated Windows Authentication (IWA) gebruiken met kerberos beperkte delegatie (KCD). Zie [B2B-gebruikers in Azure AD](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)toegang verlenen tot uw on-premises toepassingen voor meer informatie.
1. Lees hoe u [lokaal beheerde partneraccounts toegang verleent tot cloudresources met behulp van Azure AD B2B-samenwerking.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)