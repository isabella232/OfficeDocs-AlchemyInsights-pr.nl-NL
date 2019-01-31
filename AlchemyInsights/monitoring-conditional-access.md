---
title: Toezicht op voorwaardelijke toegang
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656562"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="a0b2b-102">Toezicht op voorwaardelijke toegang</span><span class="sxs-lookup"><span data-stu-id="a0b2b-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="a0b2b-p101">Gericht met voorwaardelijke toegang ontvangen gebruikers een melding per e-mail als zij niet voldoen aan de toegangsvereisten van uw organisatie. Als u wilt oplossen, raden we aan een of meer van de volgende oplossingen:</span><span class="sxs-lookup"><span data-stu-id="a0b2b-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="a0b2b-p102">Als het apparaat wordt verondersteld te worden ingeschreven, adviseren de gebruiker naar de bedrijfsportal app gaan en controleren of deze wordt weergegeven in de bedrijfsportal. Als dat niet het geval is, moet de gebruiker het apparaat inschrijven.</span><span class="sxs-lookup"><span data-stu-id="a0b2b-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="a0b2b-p103">Ga in de Azure portal naar **Intune \> apparaat naleving**. Klik op **apparaat conformiteit**onder **Monitor** . Bekijk uw conformiteitsrapport apparaat om te controleren dat het apparaat van de gebruiker is gemarkeerd als compatibel.</span><span class="sxs-lookup"><span data-stu-id="a0b2b-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="a0b2b-p104">Ga in de Azure portal naar **Intune \> apparaat naleving**. Klik onder **beheren**, klikt u op het **beleid**. Controleren of een profiel is toegewezen aan het apparaat van de gebruiker in de lijst van het beleid voldaan. Als er geen profiel is toegewezen, vervolgens Intune worden niet kunnen bevestigen de bestendigheid van het apparaat.</span><span class="sxs-lookup"><span data-stu-id="a0b2b-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="a0b2b-114">Bewerken van voorwaardelijke toegang van de gebruiker is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="a0b2b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="a0b2b-115">Ga in de Azure portal naar **Intune \> voorwaardelijke toegang \> beleid**</span><span class="sxs-lookup"><span data-stu-id="a0b2b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="a0b2b-116">Selecteer een beleid in de lijst</span><span class="sxs-lookup"><span data-stu-id="a0b2b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="a0b2b-117">Klik op **gebruikers en groepen**</span><span class="sxs-lookup"><span data-stu-id="a0b2b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="a0b2b-p105">Als een bepaald beleid op iemand anders, moet u deze aan **de lijst** toevoegen. Om ervoor te zorgen dat een persoon wordt weggelaten uit het beleid, toevoegen aan de lijst **uitgesloten** .</span><span class="sxs-lookup"><span data-stu-id="a0b2b-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="a0b2b-120">Meer informatie: [hoe apparaten Monitor voorwaardelijke toegang](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="a0b2b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

