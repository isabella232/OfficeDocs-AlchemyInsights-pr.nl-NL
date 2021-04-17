---
title: Een groep maken
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816343"
---
# <a name="create-a-group"></a><span data-ttu-id="38a8f-102">Een groep maken</span><span class="sxs-lookup"><span data-stu-id="38a8f-102">Create a group</span></span>

<span data-ttu-id="38a8f-103">In dit onderwerp wordt het maken van groepen beschreven.</span><span class="sxs-lookup"><span data-stu-id="38a8f-103">This topic describes group creation.</span></span>

<span data-ttu-id="38a8f-104">**Machtiging voor het maken van een groep**</span><span class="sxs-lookup"><span data-stu-id="38a8f-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="38a8f-105">Zorg ervoor dat u gemachtigd bent om een nieuwe groep te maken.</span><span class="sxs-lookup"><span data-stu-id="38a8f-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="38a8f-106">Globale beheerders kunnen het maken van groepen uitschakelen in de Azure-portal of het Access-panel.</span><span class="sxs-lookup"><span data-stu-id="38a8f-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="38a8f-107">Mogelijk hebt u een beheerder nodig om de nieuwe groep voor u te maken of om u de juiste machtigingen te geven.</span><span class="sxs-lookup"><span data-stu-id="38a8f-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="38a8f-108">**Machtigingen voor het maken van groepen beheren**</span><span class="sxs-lookup"><span data-stu-id="38a8f-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="38a8f-109">Globale beheerders kunnen machtigingen voor het maken van groepen beheren (om beveiligingsredenen) of Office 365-groepen die zijn gemaakt in de Azure-portal of het Access-panel, door in Alle groepen Algemeen  >  **(Instellingen)** de opties 'Gebruikers kunnen beveiligingsgroepen maken in Azure-portals' of 'Gebruikers kunnen Office 365-groepen maken in Azure-portals'.</span><span class="sxs-lookup"><span data-stu-id="38a8f-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="38a8f-110">U kunt het maken van groepen ook beperken om een groep gebruikers te selecteren als u een Azure Active Directory P1 Premium-licentie hebt.</span><span class="sxs-lookup"><span data-stu-id="38a8f-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="38a8f-111">**Welkomstmelding uitschakelen voor nieuwe Office 365-groepsleden**</span><span class="sxs-lookup"><span data-stu-id="38a8f-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="38a8f-112">De welkomstmelding die wordt verzonden naar gebruikers die zijn toegevoegd aan Office 365-groepen, kan worden uitgeschakeld door **UnifiedGroupWelcomeMessageEnabled** in te stellen op Onwaar in Powershell.</span><span class="sxs-lookup"><span data-stu-id="38a8f-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="38a8f-113">Meer informatie over deze instelling [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="38a8f-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

