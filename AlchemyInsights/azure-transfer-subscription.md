---
title: Eigendom van Azure-facturering overdragen
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
- "6849"
ms.openlocfilehash: fc02a64807cad61cfeecf04d1f8e38666402583f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820605"
---
# <a name="transfer-azure-billing-ownership"></a>Eigendom van Azure-facturering overdragen

Meld u aan op de [Azure Portal](https://portal.azure.com/) als beheerder van het factureringsaccount met het abonnement dat u wilt overdragen. Als u niet zeker weet of u een beheerder bent of als u wilt bepalen wie dat is, raadpleegt u [Accountfactureringsbeheerder bepalen](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Zoek naar _Kostenbeheer en facturering_.
1. Kies **Abonnementen** in het linkerdeelvenster. Afhankelijk van de toegang, moet u mogelijk een factureringsbereik kiezen en vervolgens **Abonnementen** of **Azure-abonnementen**.
1. Kies **Eigendom van facturering overdragen** voor het abonnement dat u wilt overdragen.
1. Voer het e-mailadres in van een gebruiker die factureringsbeheerder van het account is en de nieuwe eigenaar van het abonnement moet worden en kies vervolgens **Overdrachtsaanvraag verzenden**.
1. De gebruiker ontvangt een e-mail met instructies om uw overdrachtsaanvraag te beoordelen. Om de overdrachtsaanvraag goed te keuren, kiest de gebruiker de koppeling in de e-mail en volgt de instructies.

Denk eraan dat alle [Rolgebaseerde toegangscontrole (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)-opdrachten voor het beheren van bronnen in het abonnement permanent worden verwijderd als u eigendom van facturering van uw abonnement overdraagt naar een gebruikersaccount in een andere Azure AD-tenant. Alleen de nieuwe eigenaar heeft toegang voor het beheren van bronnen in het abonnement. Voor meer informatie over het wijzigen van een map voor een abonnement, raadpleegt u [Het overdragen van abonnementen naar een gebruiker in een andere Azure AD-tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Belangrijke impact op uw facturen**_: Als u eigendom van facturering voor een Azure-abonnement heeft overgedragen, zullen uw kosten proportioneel zijn. U heeft op de volgende manier toegang tot de facturen:  

1. Kies uw abonnement op de [Abonnementenpagina](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in de Azure Portal als [gebruiker met toegang tot facturen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support) en kies vervolgens **Facturen**.
1. Klik op **Factuur downloaden** om uw PDF-factuur te bekijken. Raadpleeg [Waarom zie ik geen factuur voor de laatste factureringsperiode?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice) als u de melding _Niet beschikbaar_ krijgt.
1. U kunt uw dagelijks gebruik ook bekijken door te klikken op de **factuurperiode** om een PDF-bestand te verkrijgen van uw factuur en een exmplaar van uw gedetailleerd dagelijks gebruik-bestand (.csv). Raadpleeg [Factuur en gebruiksgegevens ophalen](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support) voor meer informatie.

**Aanbevolen documenten**

- [Het eigendom van een Azure-abonnement overdragen naar een ander account](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Info over het overdragen van eigendom van facturering voor een Azure-abonnement](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Het overdragen van Visual Studio, Microsoft Partner Network (MPN) en Pay as you go- dev-/testabonnementen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Veelgestelde vragen over het overdragen van eigendom](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Problemen met het overdragen van eigendom oplossen](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
