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
ms.openlocfilehash: c3623aee9ab3592254ffb25aade7d52a2c7ddd49fde939956162cd4008d5ba19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003564"
---
# <a name="enable-cost-management"></a>Kostenbeheer inschakelen

**Wat betekent 'kosten zijn uitgeschakeld voor uw organisatie'?**

Organisaties die gebruikmaken Enterprise Agreement (EA) of MCA-accounts (Microsoft Customer Agreement) kunnen de toegang tot kostengegevens en prijsinformatie uitschakelen.

Nadat ze zich hebben aanmelden bij de Azure-portal, kunnen ze de facturerings-API's gebruiken om facturen (eenmaal opt-in) en gebruiksgegevens te ontvangen.

**Extra gebruikers toegang geven tot facturen**

1. Ga naar **Subscriptions blade** in Azure Portal.
2. Selecteer **Facturen** en vervolgens **Toegang tot facturen.**
3. Schakel de toegang in, gevolgd door de wijzigingen op te slaan, zodat gebruikers in rollen met abonnementsbereik facturen kunnen downloaden.

> [!NOTE]
> De accountbeheerder kan ook configureren dat facturen per e-mail worden verzonden. Zie Uw factuur per e-mail [ontvangen voor meer informatie.](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)

**Gebruikers toevoegen aan de rol Factureringslezer**

1. Ga naar **Subscriptions blade** in Azure Portal.
2. Selecteer **Access-besturingselement (IAM)** en klik vervolgens op **Toevoegen.**
3. Kies **Factureringslezer** op de **pagina Selecteer een** rol.
4. Typ de e-mail van de gebruiker die u wilt uitnodigen en klik vervolgens op **OK** om de uitnodiging te verzenden.
5. Volg instructies in de e-mail uitnodigen om u aan te melden als factureringslezer. Zie Toegang verlenen tot facturering voor [meer informatie.](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)

**Aanbevolen documenten**

- [DA- en AO-weergaven inschakelen via de EA-portal](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Kosten inbegrepen in Kostenbeheer](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Ondersteunde Microsoft Azure aanbiedingen](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Kosten controleren in kostenanalyse](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Toegang geven tot factureringsgegevens](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Toegang tot een Microsoft-klantovereenkomst controleren](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






