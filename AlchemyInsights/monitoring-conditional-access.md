---
title: Toezicht op voorwaardelijke toegang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538736"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="9fb29-102">Toezicht op voorwaardelijke toegang voor Exchange</span><span class="sxs-lookup"><span data-stu-id="9fb29-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="9fb29-103">Gericht met voorwaardelijke toegang ontvangen gebruikers een melding per e-mail als zij niet voldoen aan de toegangsvereisten van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="9fb29-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="9fb29-104">Als u wilt oplossen, raden we aan een of meer van de volgende oplossingen:</span><span class="sxs-lookup"><span data-stu-id="9fb29-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="9fb29-105">Als het apparaat wordt verondersteld te worden ingeschreven, adviseren de gebruiker naar de bedrijfsportal app gaan en controleren of deze wordt weergegeven in de bedrijfsportal.</span><span class="sxs-lookup"><span data-stu-id="9fb29-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="9fb29-106">Als dat niet het geval is, moet de gebruiker het apparaat inschrijven.</span><span class="sxs-lookup"><span data-stu-id="9fb29-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="9fb29-107">Ga in de Azure portal naar **Intune \> apparaat naleving**.</span><span class="sxs-lookup"><span data-stu-id="9fb29-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="9fb29-108">Klik op **apparaat conformiteit**onder **Monitor** .</span><span class="sxs-lookup"><span data-stu-id="9fb29-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="9fb29-109">Bekijk uw conformiteitsrapport apparaat om te controleren dat het apparaat van de gebruiker is gemarkeerd als compatibel.</span><span class="sxs-lookup"><span data-stu-id="9fb29-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="9fb29-110">Ga in de Azure portal naar **Intune \> apparaat naleving**.</span><span class="sxs-lookup"><span data-stu-id="9fb29-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="9fb29-111">Klik onder **beheren**, klikt u op het **beleid**.</span><span class="sxs-lookup"><span data-stu-id="9fb29-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="9fb29-112">Controleren of een profiel is toegewezen aan het apparaat van de gebruiker in de lijst van het beleid voldaan.</span><span class="sxs-lookup"><span data-stu-id="9fb29-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="9fb29-113">Als er geen profiel is toegewezen, vervolgens Intune worden niet kunnen bevestigen de bestendigheid van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="9fb29-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="9fb29-114">Bewerken van voorwaardelijke toegang van de gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="9fb29-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="9fb29-115">Ga in de Azure portal naar **Intune \> voorwaardelijke toegang \> beleid**</span><span class="sxs-lookup"><span data-stu-id="9fb29-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="9fb29-116">Selecteer een beleid in de lijst</span><span class="sxs-lookup"><span data-stu-id="9fb29-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="9fb29-117">Klik op **gebruikers en groepen**</span><span class="sxs-lookup"><span data-stu-id="9fb29-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="9fb29-118">Als een bepaald beleid op iemand anders, moet u deze aan **de lijst** toevoegen.</span><span class="sxs-lookup"><span data-stu-id="9fb29-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="9fb29-119">Om ervoor te zorgen dat een persoon wordt weggelaten uit het beleid, toevoegen aan de lijst **uitgesloten** .</span><span class="sxs-lookup"><span data-stu-id="9fb29-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="9fb29-120">Meer informatie: [hoe apparaten Monitor voorwaardelijke toegang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="9fb29-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

