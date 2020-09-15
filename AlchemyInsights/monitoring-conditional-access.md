---
title: Voorwaardelijke toegang controleren
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702898"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="e7b26-102">Voorwaardelijke toegang voor Exchange controleren</span><span class="sxs-lookup"><span data-stu-id="e7b26-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="e7b26-103">Gebruikers met voorwaardelijke toegang ontvangen een e-mail melding als ze niet voldoen aan de toegangsvereisten van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="e7b26-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e7b26-104">We raden een of meer van de volgende oplossingen aan om dit op te lossen:</span><span class="sxs-lookup"><span data-stu-id="e7b26-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="e7b26-105">Als u ervan wordt uitgegaan dat het apparaat is ingeschreven, adviseert u de gebruiker om naar de bedrijfsportal-app te gaan en controleert u of deze wordt weergegeven in de bedrijfsportal.</span><span class="sxs-lookup"><span data-stu-id="e7b26-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e7b26-106">Als dit niet het geval is, moet de gebruiker het apparaat registreren.</span><span class="sxs-lookup"><span data-stu-id="e7b26-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="e7b26-107">Ga in de Azure-Portal naar **naleving van intune- \> apparaten**.</span><span class="sxs-lookup"><span data-stu-id="e7b26-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e7b26-108">Klik **Monitor** onder monitor **op apparaatcompatibiliteit**.</span><span class="sxs-lookup"><span data-stu-id="e7b26-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="e7b26-109">Bekijk het nalevings rapport van uw apparaat om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.</span><span class="sxs-lookup"><span data-stu-id="e7b26-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="e7b26-110">Ga in de Azure-Portal naar **naleving van intune- \> apparaten**.</span><span class="sxs-lookup"><span data-stu-id="e7b26-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="e7b26-111">Klik onder **beheren**op **beleidsregels**.</span><span class="sxs-lookup"><span data-stu-id="e7b26-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="e7b26-112">Controleer in de lijst met nalevingsbeleid of een profiel is toegewezen aan het apparaat van uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="e7b26-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e7b26-113">Als u geen profiel hebt toegewezen, kan intune de nalevingsstatus van het apparaat niet bevestigen.</span><span class="sxs-lookup"><span data-stu-id="e7b26-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="e7b26-114">De voorwaardelijke toegang-opdracht van de gebruiker bewerken.</span><span class="sxs-lookup"><span data-stu-id="e7b26-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="e7b26-115">Ga in de Azure-Portal naar **intune- \> \> beleid voor voorwaardelijke toegang**</span><span class="sxs-lookup"><span data-stu-id="e7b26-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="e7b26-116">Selecteer een beleid in de lijst.</span><span class="sxs-lookup"><span data-stu-id="e7b26-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="e7b26-117">Klik op **gebruikers en groepen**</span><span class="sxs-lookup"><span data-stu-id="e7b26-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="e7b26-118">Als u een bepaald beleid op iemand wilt richten, voegt u deze toe **aan de lijst toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="e7b26-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="e7b26-119">Voeg ze toe aan de lijst **uitsluiten** om ervoor te zorgen dat iemand van het beleid weglaat.</span><span class="sxs-lookup"><span data-stu-id="e7b26-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="e7b26-120">Meer informatie: [voorwaardelijke toegangs apparaten volgen](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="e7b26-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

