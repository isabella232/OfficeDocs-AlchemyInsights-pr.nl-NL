---
title: Ondersteunde abonnements typen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807361"
---
# <a name="supported-subscription-types"></a>Ondersteunde abonnements typen

Controleer de ondersteunde abonnements typen om verder te gaan.

[Ondersteunde abonnements typen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Facturering van eigendom overzetten**

Azure-portal als [account beheerder](https://ms.portal.azure.com/) van het factuur account met het abonnement dat u wilt overzetten

- Zoek op **kostenbeheer + facturering** . Selecteer **abonnementen** in het linkerdeelvenster. Afhankelijk van de toegang moet u mogelijk een factuur bereik selecteren en vervolgens **abonnementen** of **Azure-abonnementen** .
- Selecteer het eigendom van de facturering voor het abonnement dat u wilt overzetten
- Voer het e-mailadres in van een gebruiker die een factureringsbeheerder is van het account dat de nieuwe eigenaar wordt van het abonnement en selecteer vervolgens **overdrachtsaanvraag verzenden** .
- De gebruiker ontvangt een e-mail met instructies om uw overdrachtsaanvraag te controleren. De gebruiker kan de koppeling in het e-mailbericht selecteren en de instructies volgen om de overdrachtsaanvraag goed te keuren.

Opmerking: als u het eigendom van uw abonnement overdraagt naar het account van een gebruiker in een andere Azure AD-Tenant, worden alle toewijzingen met [toegangsbeheer voor rollen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) voor het beheren van resources in het abonnement blijvend verwijderd. Alleen de nieuwe eigenaar kan de bronnen in het abonnement beheren. Zie voor meer informatie [een abonnement overzetten naar een gebruiker in een andere Azure AD-Tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Eigendom van een abonnement overzetten**

Eigenaar van het abonnement overzetten op basis van toegang (RBAC) voor het beheren van resources in het abonnement, verliezen hun toegang. Zie [een Azure-abonnement koppelen of toevoegen aan Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)voor meer informatie over het toevoegen van een bestaand abonnement aan een Tenant.

- Abonnements overschrijving met een bestaand openstaand bedrag van de huidige factureringscyclus wordt niet overgezet naar het nieuwe betaal instrument in het nieuwe account. De enige voor de gebruikers in het nieuwe account beschikbare gegevens zijn de kosten van de afgelopen maand voor uw abonnement. De rest van de gebruiks-en factureringsgeschiedenis wordt niet met het abonnement overgebracht.
- Het overdragen van facturerings machtigingen van Enterprise Agreement (EA) wordt momenteel ondersteund in de portal voor Enterprise Agreement
- Voor het overzetten van een abonnement op een krediet, zoals Visual Studio, BizSpark, Microsoft-partnernetwerk, moet een nieuwe gebruiker een netwerk licentie voor Visual Studio/Microsoft-partners hebben om de overdrachtsaanvraag te accepteren
- Alle bronnen zoals virtuele machines, schijven en websites worden overschreven naar het nieuwe account. De volgende bronnen kunnen worden beïnvloed in een overdracht van een ander Tenant abonnement:

**Azure AD Domain Services**

Azure-sleutel kluizen

- [SQL-gerelateerde gebruikers en-databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) kunnen worden beïnvloed, met name als de klant met een Azure Active Directory gerelateerde verificatie werkt.
- **App-Services** die zijn geconfigureerd met Azure Active Directory-verificatie, kunnen worden beïnvloed
- **Visual Studio Team** Services-accounts die zijn gekoppeld aan Azure-abonnementen, verliezen mogelijk tijdelijk toegang als het verbonden Azure-abonnement is geannuleerd

**Aanbevolen documenten**

Stappen na het accepteren van het eigendom van de factuur:

- Als u het eigendom van de factuur wilt behouden, maar het type abonnement wilt wijzigen, raadpleegt u: [een abonnement op uw Azure-abonnement omzetten in een andere aanbieding](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [De overdracht van Visual Studio, Microsoft Partner Network (MPN) en betalen naar gebruik-ontwikkelaars/proefabonnementen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Facturerings machtigingen van een Enterprise Agreement-abonnement (EA) overdragen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Veelgestelde vragen over het overdragen van eigendom](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problemen met de overdracht van eigendom oplossen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)