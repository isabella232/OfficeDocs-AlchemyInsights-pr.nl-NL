---
title: Locatie van gegevens
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207256"
---
# <a name="data-location"></a><span data-ttu-id="bf386-102">Locatie van gegevens</span><span class="sxs-lookup"><span data-stu-id="bf386-102">Data location</span></span>

<span data-ttu-id="bf386-103">U de locatie van uw Office 365-Tenant weergeven in het Admin Center of door verbinding te maken met Exchange Online via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bf386-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="bf386-104">**Admin Center:**</span><span class="sxs-lookup"><span data-stu-id="bf386-104">**Admin center:**</span></span>
1. <span data-ttu-id="bf386-105">Meld u aan bij het [Admin Center](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="bf386-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="bf386-106">Selecteer **instellingen** > **organisatie profiel**.</span><span class="sxs-lookup"><span data-stu-id="bf386-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="bf386-107">Selecteer onder **gegevenslocatie**de optie **Details weergeven**.</span><span class="sxs-lookup"><span data-stu-id="bf386-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="bf386-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="bf386-108">**PowerShell:**</span></span>
1. <span data-ttu-id="bf386-109">Verbinding maken met Exchange Online met behulp van Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bf386-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="bf386-110">Voer de cmdlet [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) om een lijst met de eigenschappen van uw Tenant weer te geven.</span><span class="sxs-lookup"><span data-stu-id="bf386-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="bf386-111">Bekijk de eigenschap OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="bf386-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="bf386-112">Wanneer u de gegevenslocatie voor EXO en SPO hebt, u de gegevenslocatie bepalen voor andere services die u gebruiken vanaf [waar uw gegevens zich bevinden](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="bf386-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>