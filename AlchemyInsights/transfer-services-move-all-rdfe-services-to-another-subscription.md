---
title: Transfer Services - Alle RDFE-services verplaatsen naar een ander abonnement
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940033"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Transfer Services - Alle RDFE-services verplaatsen naar een ander abonnement

**Resources verplaatsen**

Azure-resources kunnen worden verplaatst naar een ander Azure-abonnement of resourcegroep onder hetzelfde abonnement met behulp van Azure Portal, Azure PowerShell, Azure CLI of de REST-API om resources te verplaatsen.

Zie het volgende voordat u resources kunt verplaatsen:

- [Controlelijst voordat u resources verplaatst](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Services die kunnen worden verplaatst](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [De move valideren](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Richtlijnen voor services verplaatsen](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

Als u bestaande resources wilt verplaatsen naar een andere resourcegroep of een ander abonnement, kunt u het volgende gebruiken:

- [Azure-portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Zelfstudie: [Azure-resources verplaatsen naar een andere resourcegroep of een ander abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Fouten oplossen met Azure Resource Manager**

Raadpleeg de onderstaande artikelen voor meer informatie over enkele veelvoorkomende Azure-implementatiefouten en ontvang informatie om deze op te lossen. Zie Foutcode zoeken als u de foutcode voor de implementatiefout [niet kunt vinden.](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)

- [Implementatiefouten oplossen](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Problemen met het verplaatsen van Azure-resources naar nieuwe resourcegroep of -abonnement oplossen](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Houd er rekening mee dat als u uw Azure-abonnement wilt upgraden, zoals overstappen van gratis naar betalen per gebruik, u uw abonnement moet converteren.

- Als u een gratis proefabonnement wilt upgraden, zie Uw gratis proefabonnement of Microsoft-Imagine Azure-abonnement upgraden naar [Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- Zie Uw [Azure Pay-As-You-Go-abonnement wijzigen](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)in een andere aanbieding als u een pay-as-you-go-account wilt wijzigen.

**Een Azure-abonnement toevoegen of koppelen aan uw Azure Active Directory tenant:**

1. Meld u aan en selecteer het abonnement dat u wilt gebruiken op [de pagina Abonnementen in azure portal.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Selecteer **Adreslijst wijzigen.**
3. Controleer eventuele waarschuwingen die worden weergegeven en selecteer vervolgens **Wijzigen.**
4. De adreslijst wordt gewijzigd voor het abonnement en u krijgt een succesbericht.
5. Gebruik de *adreslijstwisselaar* om naar uw nieuwe adreslijst te gaan. Het kan tot 10 minuten duren voordat alles correct wordt uitgevoerd.

**Aanbevolen documenten**

- [Eigendom van een Azure-abonnement overdragen](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Resources verplaatsen naar nieuwe resourcegroep of -abonnement](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Resources beheren met Behulp van Azure Portal](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
