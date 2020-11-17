---
title: Rollen van geprivilegieerde identiteitsbeheer
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088678"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="ae3af-102">De rol van bevoorrechte identiteitsbeheer (PIM)</span><span class="sxs-lookup"><span data-stu-id="ae3af-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="ae3af-103">**Machtigingen worden niet toegekend na het activeren van een rol**</span><span class="sxs-lookup"><span data-stu-id="ae3af-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="ae3af-104">Wanneer u een rol activeert in azure AD geprivilegieerde identiteitsbeheer (PIM), wordt de activering mogelijk niet onmiddellijk doorgegeven aan alle portals die de rol met bevoegdheden vereisen.</span><span class="sxs-lookup"><span data-stu-id="ae3af-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="ae3af-105">Soms kan het gebeuren dat de wijziging niet onmiddellijk van invloed is op webcaches in een portal, zelfs als de wijziging wordt doorgevoerd.</span><span class="sxs-lookup"><span data-stu-id="ae3af-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="ae3af-106">Voer de volgende stappen uit als uw activering is vertraagd:</span><span class="sxs-lookup"><span data-stu-id="ae3af-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="ae3af-107">Meld u af bij de Azure-Portal en meld u vervolgens weer aan.</span><span class="sxs-lookup"><span data-stu-id="ae3af-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="ae3af-108">Wanneer u een functie van Azure AD of een Azure-resource activeert, ziet u de fasen van de activering.</span><span class="sxs-lookup"><span data-stu-id="ae3af-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="ae3af-109">Wanneer alle fasen zijn voltooid, wordt de link Afmelden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="ae3af-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="ae3af-110">U kunt deze koppeling gebruiken om u af te melden. Hiermee kunt u de meeste aanvragen voor activerings vertraging oplossen.</span><span class="sxs-lookup"><span data-stu-id="ae3af-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="ae3af-111">Zorg er in PIM voor dat u wordt vermeld als lid van de rol.</span><span class="sxs-lookup"><span data-stu-id="ae3af-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="ae3af-112">Zorg dat u zich afmeldt en opnieuw aanmeldt als u de rol van Exchange-beheerder activeert.</span><span class="sxs-lookup"><span data-stu-id="ae3af-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="ae3af-113">Als het probleem zich blijft voordoen, opent u een ondersteuningsticket en verhoogt u dit als probleem.</span><span class="sxs-lookup"><span data-stu-id="ae3af-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="ae3af-114">Als u de rol van Exchange-beheerder gebruikt om toegang te krijgen tot het beveiligings-en compliance-centrum, raadpleegt u de volgende stap.</span><span class="sxs-lookup"><span data-stu-id="ae3af-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="ae3af-115">Als u een rol activeert om toegang te krijgen tot het beleid voor beveiliging en compliance, of als u de SharePoint-beheerdersrol activeert, kunt u de activerings vertraging van enkele minuten tot enkele minuten tot een paar uur weer krijgen.</span><span class="sxs-lookup"><span data-stu-id="ae3af-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="ae3af-116">Dit is een bekend probleem en we werken actief met deze teams om dit probleem zo snel mogelijk op te lossen.</span><span class="sxs-lookup"><span data-stu-id="ae3af-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="ae3af-117">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="ae3af-117">For more information, see:</span></span>

- [<span data-ttu-id="ae3af-118">Mijn Azure AD-rollen in PIM activeren</span><span class="sxs-lookup"><span data-stu-id="ae3af-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="ae3af-119">Mijn Azure-resourcerollen in PIM activeren</span><span class="sxs-lookup"><span data-stu-id="ae3af-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="ae3af-120">**Machtigingen worden niet verwijderd na het deactiveren van een rol of de activering van rollen is verloopt**</span><span class="sxs-lookup"><span data-stu-id="ae3af-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="ae3af-121">Wanneer u een rol deactiveert op een Azure AD-identiteitsbeheer of wanneer een activeringsperiode voor rollen verloopt, is er mogelijk een vertraging waarbij u nog steeds toegang hebt.</span><span class="sxs-lookup"><span data-stu-id="ae3af-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="ae3af-122">Voer de volgende stappen uit als uw deactivering vertraagd is:</span><span class="sxs-lookup"><span data-stu-id="ae3af-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="ae3af-123">Als u de rol van Exchange-beheerder of de activeringsperiode voor rollen deactiveert en u merkt dat de machtigingen niet worden verwijderd, opent u een ondersteuningsticket en laat u uw ondersteuningsmedewerker weten dat u een ticket met het DRM-team (geprivilegieerde toegangsbeheer) in Office kunt vinden over dit probleem.</span><span class="sxs-lookup"><span data-stu-id="ae3af-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="ae3af-124">Als de activeringsperiode is verlopen, maar de browsersessie nog steeds is geopend, sluit u de browser.</span><span class="sxs-lookup"><span data-stu-id="ae3af-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="ae3af-125">U kunt de rol blijven gebruiken totdat u deze sessie sluit.</span><span class="sxs-lookup"><span data-stu-id="ae3af-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="ae3af-126">Dit is een bekend probleem en we bekijken een mogelijke oplossing voor het actief intrekken van elke sessie wanneer de activering is verlopen.</span><span class="sxs-lookup"><span data-stu-id="ae3af-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="ae3af-127">Als uw vertraging afwijkt van deze twee scenario's, kunt u een ondersteuningsticket openen.</span><span class="sxs-lookup"><span data-stu-id="ae3af-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
