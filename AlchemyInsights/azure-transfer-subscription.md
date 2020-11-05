---
title: Eigendom van Azure-facturering overbrengen
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
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922031"
---
# <a name="transfer-azure-billing-ownership"></a>Eigendom van Azure-facturering overbrengen

Meld u aan bij de [Azure-Portal](https://portal.azure.com/) als beheerder van het factuur account met het abonnement dat u wilt overzetten. Als u niet zeker weet of u een beheerder bent, of als u wilt bepalen wie dit doet, raadpleegt u de [rekening factureringsbeheerder bepalen](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

- Zoek op **kostenbeheer + facturering**.
- Selecteer **abonnementen** in het linkerdeelvenster. Afhankelijk van de toegang moet u mogelijk een factuur bereik selecteren en vervolgens **abonnementen** of **Azure-abonnementen**.
- Selecteer het eigendom van de **facturering** voor het abonnement dat u wilt overzetten
- Voer het e-mailadres in van een gebruiker die een factureringsbeheerder is van het account dat de nieuwe eigenaar wordt van het abonnement en selecteer vervolgens **overdrachtsaanvraag verzenden** .
- De gebruiker ontvangt een e-mail met instructies om uw overdrachtsaanvraag te controleren. De gebruiker kan de koppeling in het e-mailbericht selecteren en de instructies volgen om de overdrachtsaanvraag goed te keuren.

**Opmerking** : als u het eigendom van uw abonnement overdraagt naar het account van een gebruiker in een andere Azure AD-Tenant, worden alle toewijzingen met [toegangsbeheer voor rollen (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)voor het beheren van resources in het abonnement blijvend verwijderd. Alleen de nieuwe eigenaar kan de bronnen in het abonnement beheren. Zie voor meer informatie [een abonnement overzetten naar een gebruiker in een andere Azure AD-Tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Aanbevolen documenten**

- [Facturering van een Azure-abonnement overzetten naar een ander account](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Het eigendom van de facturering overzetten voor een Azure-abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [De overdracht van Visual Studio, Microsoft Partner Network (MPN) en betalen naar gebruik-ontwikkelaars/proefabonnementen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Veelgestelde vragen over het overdragen van eigendom](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problemen met de overdracht van eigendom oplossen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
