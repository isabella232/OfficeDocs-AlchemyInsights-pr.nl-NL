---
title: Services overzetten-alle RDFE-Services naar een ander abonnement verplaatsen
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
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691979"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="a2530-102">Services overzetten-alle RDFE-Services naar een ander abonnement verplaatsen</span><span class="sxs-lookup"><span data-stu-id="a2530-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="a2530-103">**Resources verplaatsen**</span><span class="sxs-lookup"><span data-stu-id="a2530-103">**Move resources**</span></span>

<span data-ttu-id="a2530-104">Azure-resources kunnen worden verplaatst naar een ander Azure-abonnement of resourcegroep onder hetzelfde abonnement met behulp van Azure Portal, Azure PowerShell, Azure CLI of de REST API om bronnen te verplaatsen.</span><span class="sxs-lookup"><span data-stu-id="a2530-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="a2530-105">Zie de volgende artikelen voor informatie over het verplaatsen van bronnen.</span><span class="sxs-lookup"><span data-stu-id="a2530-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="a2530-106">Controlelijst voor het verplaatsen van resources</span><span class="sxs-lookup"><span data-stu-id="a2530-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="a2530-107">Services die kunnen worden verplaatst</span><span class="sxs-lookup"><span data-stu-id="a2530-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a2530-108">De verhuizing valideren</span><span class="sxs-lookup"><span data-stu-id="a2530-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="a2530-109">Richtlijnen voor services</span><span class="sxs-lookup"><span data-stu-id="a2530-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="a2530-110">U kunt de volgende bronnen gebruiken om bestaande bronnen te verplaatsen naar een andere resourcegroep of een ander abonnement:</span><span class="sxs-lookup"><span data-stu-id="a2530-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="a2530-111">Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="a2530-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="a2530-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a2530-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="a2530-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a2530-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="a2530-114">REST-API</span><span class="sxs-lookup"><span data-stu-id="a2530-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="a2530-115">Zelfstudie: [Azure-resources naar een andere resourcegroep of een ander abonnement verplaatsen](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="a2530-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="a2530-116">**Fouten oplossen met Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="a2530-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="a2530-117">Raadpleeg de volgende artikelen voor meer informatie over veelvoorkomende fouten en informatie over het oplossen van fouten in Azure.</span><span class="sxs-lookup"><span data-stu-id="a2530-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="a2530-118">Als u de foutcode voor de implementatiefout niet kunt vinden, raadpleegt u [foutcode zoeken](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="a2530-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="a2530-119">Implementatiefouten oplossen</span><span class="sxs-lookup"><span data-stu-id="a2530-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="a2530-120">Problemen met het verplaatsen van Azure-resources naar nieuwe resourcegroep of een abonnement oplossen</span><span class="sxs-lookup"><span data-stu-id="a2530-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="a2530-121">Als u een upgrade van uw Azure-abonnement wilt uitvoeren, bijvoorbeeld over het overstappen van gratis naar betaald, moet u uw abonnement converteren.</span><span class="sxs-lookup"><span data-stu-id="a2530-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="a2530-122">Als u een gratis proefversie wilt upgraden, raadpleegt u [uw gratis proefabonnement upgraden of een Microsoft-abonnement voor](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a2530-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="a2530-123">Zie [uw abonnement op Azure pay-to-go wijzigen in een andere aanbieding](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)als u een account voor betalen naar wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="a2530-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="a2530-124">**Een Azure-abonnement aan de Azure Active Directory-Tenant toevoegen of hieraan koppelen:**</span><span class="sxs-lookup"><span data-stu-id="a2530-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="a2530-125">Meld u aan en selecteer het abonnement dat u wilt gebruiken vanaf de [pagina Abonnementen in azure-Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="a2530-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="a2530-126">Selecteer **map wijzigen**.</span><span class="sxs-lookup"><span data-stu-id="a2530-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="a2530-127">Bekijk eventuele waarschuwingen die worden weergegeven en selecteer vervolgens **wijzigen**.</span><span class="sxs-lookup"><span data-stu-id="a2530-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="a2530-128">De map wordt voor het abonnement gewijzigd en er wordt een bericht weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a2530-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="a2530-129">Gebruik de *adreslijst* wisselaar om naar de nieuwe adreslijst te gaan.</span><span class="sxs-lookup"><span data-stu-id="a2530-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="a2530-130">Het duurt maximaal 10 minuten voordat alles correct wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a2530-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="a2530-131">**Aanbevolen documenten**</span><span class="sxs-lookup"><span data-stu-id="a2530-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="a2530-132">Eigendom van een Azure-abonnement overdragen</span><span class="sxs-lookup"><span data-stu-id="a2530-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="a2530-133">Resources verplaatsen naar een nieuwe resourcegroep of een ander abonnement</span><span class="sxs-lookup"><span data-stu-id="a2530-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="a2530-134">Bronnen beheren met behulp van Azure Portal</span><span class="sxs-lookup"><span data-stu-id="a2530-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
