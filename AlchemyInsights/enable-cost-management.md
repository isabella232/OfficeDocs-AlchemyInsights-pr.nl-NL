---
title: Kostenbeheer inschakelen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677218"
---
# <a name="enable-cost-management"></a>Kostenbeheer inschakelen

**Wat betekenen de kosten voor uw organisatie?**

Organisaties die gebruikmaken van Enterprise Agreement (EA) of Microsoft Customer Agreement (MCA), kunnen de toegang tot kosteninformatie en prijsinformatie uitschakelen.

Nadat u zich hebt aangemeld bij een Azure-Portal, kunnen ze de bewerkings-Api's van de apps gebruiken om via programmatisch een factuur te krijgen (indien aangemeld) en gebruiksinformatie.

**Toestaan dat extra gebruikers toegang hebben tot facturen**

1. Ga naar **blad abonnementen** in azure Portal.
2. Selecteer **facturen** en vervolgens **toegang tot facturen**.
3. Schakel de toegang in, gevolgd door de wijzigingen op te slaan, zodat gebruikers met rollen met een abonnement kunnen facturen kunnen downloaden.

> [!NOTE]
> De account beheerder kan ook configureren dat facturen via e-mail worden verzonden. Zie [uw factuur via E-mail ontvangen](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)voor meer informatie.

**Gebruikers toevoegen aan de rol van facturerings lezer**

1. Ga naar **blad abonnementen** in azure Portal.
2. Selecteer **toegangsbeheer (IAM)** en klik op **toevoegen**.
3. Kies **facturerings lezer** op de pagina **Selecteer een rol** .
4. Typ het e-mailadres van de gebruiker die u wilt uitnodigen en klik op **OK** om de uitnodiging te verzenden.
5. Volg de instructies in de e-mail uitnodigen om u aan te melden als facturerings lezer. Zie voor meer informatie de optie [toegang tot facturering verlenen](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Aanbevolen documenten**

- [DA-en AO-weergaven inschakelen via EA Portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kosten in kostenbeheer](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Ondersteunde Microsoft Azure-aanbiedingen](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Kosten controleren in kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Toegang tot de factureringsgegevens geven](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Toegang tot een Microsoft-klant overeenkomst controleren](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






