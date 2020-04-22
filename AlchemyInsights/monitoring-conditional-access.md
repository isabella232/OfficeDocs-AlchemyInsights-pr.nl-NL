---
title: Controle voorwaardelijke toegang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713713"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="1e6f6-102">Controle op voorwaardelijke toegang voor Exchange</span><span class="sxs-lookup"><span data-stu-id="1e6f6-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="1e6f6-103">Gebruikers die zijn getarget met voorwaardelijke toegang, ontvangen een e-mail met een melding als ze niet voldoen aan de toegangsvereisten van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="1e6f6-104">Om het probleem op te lossen, raden we een of meer van de volgende oplossingen aan:</span><span class="sxs-lookup"><span data-stu-id="1e6f6-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="1e6f6-105">Als het apparaat wordt verondersteld te zijn ingeschreven, adviseert u de gebruiker om naar de App Van bedrijfsportal te gaan en te verifiëren of het in de bedrijfsportal wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="1e6f6-106">Als dit niet het zo is, moet de gebruiker het apparaat inschrijven.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="1e6f6-107">Ga in de Azure-portal naar **Intune \> Device compliance**.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="1e6f6-108">Klik **onder Controleren** op Naleving van het **apparaat**.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="1e6f6-109">Bekijk het nalevingsrapport van uw apparaat om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="1e6f6-110">Ga in de Azure-portal naar **Intune \> Device compliance**.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="1e6f6-111">Klik **onder Beheren**op **Beleid**.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="1e6f6-112">Controleer in de lijst met nalevingsbeleid of een profiel is toegewezen aan het apparaat van uw gebruiker.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="1e6f6-113">Als er geen profiel is toegewezen, kan Intune de nalevingsstatus van het apparaat niet bevestigen.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="1e6f6-114">De voorwaardelijke toegangstoewijzing van de gebruiker bewerken.</span><span class="sxs-lookup"><span data-stu-id="1e6f6-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="1e6f6-115">Ga in de Azure-portal naar **Intune-beleid \> \> voor voorwaardelijke toegang**</span><span class="sxs-lookup"><span data-stu-id="1e6f6-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="1e6f6-116">Een beleid selecteren in de lijst</span><span class="sxs-lookup"><span data-stu-id="1e6f6-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="1e6f6-117">Klik **op Gebruikers en groepen**</span><span class="sxs-lookup"><span data-stu-id="1e6f6-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="1e6f6-118">Als u een bepaald beleid op iemand wilt targeten, voegt u deze toe aan de lijst **Opnemen.**</span><span class="sxs-lookup"><span data-stu-id="1e6f6-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="1e6f6-119">Als u ervoor wilt zorgen dat een persoon uit het beleid wordt weggelaten, voegt u deze toe aan de lijst **Uitsluiten.**</span><span class="sxs-lookup"><span data-stu-id="1e6f6-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="1e6f6-120">Lees meer: [Apparaten voor voorwaardelijke toegang controleren](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="1e6f6-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

