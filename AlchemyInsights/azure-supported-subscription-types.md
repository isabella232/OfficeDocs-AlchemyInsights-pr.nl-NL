---
title: Ondersteunde abonnementstypen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820677"
---
# <a name="supported-subscription-types"></a>Ondersteunde abonnementstypen

Bekijk de ondersteunde abonnementstypen om door te gaan.

[Ondersteunde abonnementstypen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Eigendom van facturering overdragen**

Meld u aan op Azure Portal als de [accountbeheerder](https://ms.portal.azure.com/) van het factureringsaccount met het abonnement dat u wilt overdragen

- Zoek op **Kostenbeheer en facturering**. Selecteer **Abonnementen** in het linkerdeelvenster. Afhankelijk van de toegang moet u mogelijk een factureringsbereik kiezen en vervolgens **Abonnementen** of **Azure-abonnementen**.
- Selecteer Eigendom van facturering overdragen voor het abonnement dat u wilt overdragen
- Voer het e-mailadres in van een gebruiker die factureringsbeheerder van het account is en de nieuwe eigenaar van het abonnement moet worden. Selecteer vervolgens **Overdrachtsaanvraag verzenden**
- De gebruiker ontvangt een e-mail met instructies om uw overdrachtsaanvraag te beoordelen. Om de overdrachtsaanvraag goed te keuren, kiest de gebruiker de koppeling in de e-mail en volgt de instructies.

Opmerking: alle [RBAC- (op rollen gebaseerd toegangsbeheer)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)opdrachten voor het beheren van bronnen in het abonnement worden definitief verwijderd als u eigendom van facturering van uw abonnement overdraagt naar een gebruikersaccount in een andere Azure AD-tenant. Alleen de nieuwe eigenaar heeft toegang voor het beheren van bronnen in het abonnement. Zie [Abonnementen overdragen naar een gebruiker in een andere Azure AD-tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support) voor meer informatie.

**Eigendom van abonnement overdragen**

Bij het overzetten van het abonnementseigendom vervalt de toegang voor het op rollen gebaseerd toegangsbeheer (RBAC) voor het beheren van resources in het abonnement. Zie [Een Azure-abonnement aan Azure Active Directory toevoegen of koppelen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support) voor meer informatie over het toevoegen van een bestaand abonnement aan een tenant.

- De abonnementsoverdracht met een uitstaand bedrag van de huidige factureringscyclus wordt niet overgedragen op het nieuwe betaalinstrument in het nieuwe account. De enige informatie die beschikbaar is voor de gebruikers in een nieuw account zijn de kosten van uw abonnement van de afgelopen maand. De rest van de gebruiks- en factureringsgeschiedenis wordt niet mee overgedragen met het abonnement.
- Het overdragen van het eigendom van facturering van EA-abonnementen (Enterprise Agreement) wordt momenteel alleen ondersteund in de Enterprise Agreement Portal
- Voor het overdragen van een kredietgeoriënteerd abonnement, zoals Visual Studio, BizSpark, Microsoft Partner Network, naar een nieuwe gebruiker, is een Visual Studio-/Microsoft-partnernetwerklicentie vereist om de overdrachtsaanvraag te accepteren.
- Alle resources, zoals virtuele machines, schijven en websites, worden naar het nieuwe account overgedragen. De overdracht van een abonnement tussen tenants kan van invloed zijn op de volgende resources:

**Azure AD Domain Services**

Azure-sleutelkluizen

- [SQL-gerelateerde gebruikers en databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kunnen worden beïnvloed, met name als de klant gebruikmaakt van verificatie met betrekking tot Azure Active Directory
- **App-services** die zijn geconfigureerd met Azure Active Directory-verificatie, kunnen worden beïnvloed
- **Visual Studio Team** Services-accounts die aan Azure-abonnementen zijn gekoppeld, kunnen tijdelijk de toegang verliezen wanneer het gekoppelde Azure-abonnement wordt opgezegd

**Aanbevolen documenten**

Stappen na het accepteren van het eigendom van facturering:

- Als u het eigendom van de facturering wilt behouden, maar het type abonnement wilt wijzigen, raadpleegt u: [Azure-abonnement overzetten naar een andere aanbieding](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Het overdragen van Visual Studio, Microsoft Partner Network (MPN) en Pay as you go Dev/Test-abonnementen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Factureringseigendom van EA-abonnementen (Enterprise Agreement) overdragen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Veelgestelde vragen over het overdragen van eigendom](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problemen met het overdragen van eigendom oplossen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)