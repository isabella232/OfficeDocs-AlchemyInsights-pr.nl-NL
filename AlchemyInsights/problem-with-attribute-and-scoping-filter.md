---
title: Probleem met kenmerk en bereikfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481363"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="5908e-102">Probleem met kenmerk en bereikfilter</span><span class="sxs-lookup"><span data-stu-id="5908e-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="5908e-103">**Probleem met conflicterende UPN-waarden**</span><span class="sxs-lookup"><span data-stu-id="5908e-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="5908e-104">Op de werkdag naar AD User Provisioning Workday to AD User Provisioning wordt het foutbericht **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique weergegeven.**</span><span class="sxs-lookup"><span data-stu-id="5908e-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="5908e-105">De bewerking is mislukt omdat de UPN-waarde voor toevoeging/wijziging niet uniek is voor het hele bos.</span><span class="sxs-lookup"><span data-stu-id="5908e-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="5908e-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="5908e-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="5908e-107">De **userPrincipalName-waarde** die de Werkdag-connector probeert in te stellen bij het maken van het AD-gebruikersaccount bestaat al in het doel-AD-domein.</span><span class="sxs-lookup"><span data-stu-id="5908e-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="5908e-108">Dit houdt in dat ofwel (1) de gebruiker al bestaat en dat de bijbehorende id-controle is mislukt voor de gebruiker of (2) de UPN-generatieregel een conflicterende waarde genereert.</span><span class="sxs-lookup"><span data-stu-id="5908e-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="5908e-109">Hier volgen de voorgestelde stappen voor een oplossing:</span><span class="sxs-lookup"><span data-stu-id="5908e-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="5908e-110">Als het werkdagaccount niet kan worden gekoppeld aan het Active Directory-account door de overeenkomende id-controle, controleert u of het overeenkomende id-kenmerk (meestal werknemer-id) in zowel Werkdag als AD een exacte overeenkomst heeft.</span><span class="sxs-lookup"><span data-stu-id="5908e-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="5908e-111">Als ze geen overeenkomst hebben, is het een gegevensprobleem dat moet worden opgelost.</span><span class="sxs-lookup"><span data-stu-id="5908e-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="5908e-112">Als de werknemer-id op werkdag bijvoorbeeld 001052 is en in AD 1052, dan worden de twee accounts niet gekoppeld met de inrichtingsen engine en wordt geprobeerd een gebruiker te maken die al bestaat.</span><span class="sxs-lookup"><span data-stu-id="5908e-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="5908e-113">In dit geval kunt u de waarde **EmployeeID** in AD wijzigen om de voorvoeglijke nullen op te nemen, waardoor deze 001052 wordt.</span><span class="sxs-lookup"><span data-stu-id="5908e-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="5908e-114">Als de UPN-genererende expressie geen unieke waarde genereert, kunt u overwegen om de functie De duplicatie **SelectUniqueValue** te gebruiken om elke keer een unieke waarde te genereren.</span><span class="sxs-lookup"><span data-stu-id="5908e-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="5908e-115">**Werkdag naar AD User Provisioning stelt geen kenmerkwaarde voor manager in voor AD-gebruikersaccount**</span><span class="sxs-lookup"><span data-stu-id="5908e-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="5908e-116">Met de taak Werkdag naar AD-gebruikers inrichting wordt de kenmerkwaarde van het **managerkenmerk** niet voor AD-gebruikersaccounts instelling.</span><span class="sxs-lookup"><span data-stu-id="5908e-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="5908e-117">Er zijn twee scenario's mogelijk waarin dit gedrag wordt gezien:</span><span class="sxs-lookup"><span data-stu-id="5908e-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="5908e-118">De manager in werkdag kan niet worden opgelost met een bijbehorend ad-gebruikersaccount omdat de manager niet binnen het bereik valt.</span><span class="sxs-lookup"><span data-stu-id="5908e-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="5908e-119">In een **scenario met meerdere AD-domeinen** is de manager in werkdag niet aanwezig in hetzelfde domein als de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="5908e-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="5908e-120">Probeer de volgende stappen om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="5908e-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="5908e-121">Als u bereikfilters hebt gedefinieerd, controleert u eerst of de manager binnen het bereik valt en of de scoping-component wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="5908e-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="5908e-122">Als de manager niet voldoet aan het bereikfilter, wijzigt u het filter zodat de manager ook binnen het bereik van de inrichtingsbewerking valt.</span><span class="sxs-lookup"><span data-stu-id="5908e-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="5908e-123">Als u meerdere AD-domeinen hebt, geldt voor de connector een bekende beperking dat het niet mogelijk is om verwijzingen naar domeinbeheer op te lossen.</span><span class="sxs-lookup"><span data-stu-id="5908e-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="5908e-124">Zie Zelfstudie: Werkdag configureren voor het automatisch inrichten van gebruikers voor meer informatie over het configureren van de werkdag voor automatische [inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="5908e-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













