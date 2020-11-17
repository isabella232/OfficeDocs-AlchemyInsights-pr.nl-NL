---
title: Een groep maken
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088687"
---
# <a name="create-a-group"></a><span data-ttu-id="cd073-102">Een groep maken</span><span class="sxs-lookup"><span data-stu-id="cd073-102">Create a group</span></span>

<span data-ttu-id="cd073-103">In dit onderwerp wordt het maken van groepen beschreven.</span><span class="sxs-lookup"><span data-stu-id="cd073-103">This topic describes group creation.</span></span>

<span data-ttu-id="cd073-104">**Machtiging om een groep te maken**</span><span class="sxs-lookup"><span data-stu-id="cd073-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="cd073-105">Zorg ervoor dat u gemachtigd bent om een nieuwe groep te maken.</span><span class="sxs-lookup"><span data-stu-id="cd073-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="cd073-106">Globale beheerders kunnen het maken van groepen in het Azure-portal of toegangsvenster uitschakelen.</span><span class="sxs-lookup"><span data-stu-id="cd073-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="cd073-107">U hebt mogelijk een beheerder nodig om de nieuwe groep voor u te maken of om u de juiste machtigingen te geven.</span><span class="sxs-lookup"><span data-stu-id="cd073-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="cd073-108">**Machtigingen voor het maken van groepen beheren**</span><span class="sxs-lookup"><span data-stu-id="cd073-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="cd073-109">Globale beheerders kunnen het maken van machtigingen voor het maken van groepen (voor beveiligingsredenen) of Office 365-groepen die zijn gemaakt in het Azure-portal of het deelvenster toegang beheren, door ' gebruikers kunnen beveiligingsgroepen maken in azure-portals ' of ' gebruikers kunnen Office 365-groepen maken in azure-portal ' in **alle groepen**  >  **Algemeen (instellingen)**.</span><span class="sxs-lookup"><span data-stu-id="cd073-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="cd073-110">U kunt ook het maken van groepen beperken voor het selecteren van een groep gebruikers als u een Azure Active Directory P1 Premium-licentie hebt.</span><span class="sxs-lookup"><span data-stu-id="cd073-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="cd073-111">**Welkom melding uitschakelen voor nieuwe leden van Office 365-groep**</span><span class="sxs-lookup"><span data-stu-id="cd073-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="cd073-112">De welkomst melding die wordt verzonden naar gebruikers die zijn toegevoegd aan Office 365-groepen kan worden uitgeschakeld door **UnifiedGroupWelcomeMessageEnabled** in te stellen op ONWAAR in PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cd073-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="cd073-113">Meer informatie over deze [instelling.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="cd073-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

