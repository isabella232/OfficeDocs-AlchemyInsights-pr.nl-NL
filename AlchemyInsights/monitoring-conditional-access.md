---
title: Voorwaardelijke toegang bewaken
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708669"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a0b0f-102">Voorwaardelijke toegang voor Exchange bewaken</span><span class="sxs-lookup"><span data-stu-id="a0b0f-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a0b0f-103">Gebruikers aan wie voorwaardelijke toegang is gericht, ontvangen een e-mailmelding als ze niet aan de toegangsvereisten van uw organisatie voldoen.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a0b0f-104">U wordt aangeraden een of meer van de volgende oplossingen op te lossen:</span><span class="sxs-lookup"><span data-stu-id="a0b0f-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="a0b0f-105">Als ervan wordt uitgegaan dat het apparaat is geregistreerd, adviseert u de gebruiker naar de bedrijfsportal-app te gaan en te controleren of deze wordt weergegeven in de bedrijfsportal.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a0b0f-106">Als dat niet zo is, moet de gebruiker het apparaat registreren.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="a0b0f-107">Ga in de Azure-portal naar Intune > apparaat compliance.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a0b0f-108">Klik onder Beeldscherm op Apparaat compliance.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="a0b0f-109">Bekijk het apparaat compliance-rapport om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="a0b0f-110">Ga in de Azure-portal naar Intune > apparaat compliance.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a0b0f-111">Klik onder Beheren op Beleid.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-111">Under Manage, click Policies.</span></span> <span data-ttu-id="a0b0f-112">Controleer in de lijst met nalevingsbeleidsregels of een profiel is toegewezen aan het apparaat van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a0b0f-113">Als er geen profiel is toegewezen, kan Intune de compatibiliteitsstatus van het apparaat niet bevestigen.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="a0b0f-114">Bewerk de toewijzing van voorwaardelijke toegang van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="a0b0f-115">Ga in de Azure-portal naar Beleid voor voorwaardelijke toegang **in Intune.**  >    >  </span><span class="sxs-lookup"><span data-stu-id="a0b0f-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="a0b0f-116">Selecteer een beleid in de lijst.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="a0b0f-117">Klik op Gebruikers en groepen.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-117">Click Users and groups.</span></span>
4. <span data-ttu-id="a0b0f-118">Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de lijst Opnemen.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="a0b0f-119">Als u ervoor wilt zorgen dat een persoon in het beleid wordt weggelaten, voegt u deze toe aan de lijst Uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="a0b0f-120">Handige koppelingen:</span><span class="sxs-lookup"><span data-stu-id="a0b0f-120">Helpful links:</span></span>

[<span data-ttu-id="a0b0f-121">Overzicht van apparaat compliance</span><span class="sxs-lookup"><span data-stu-id="a0b0f-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="a0b0f-122">Problemen met CA oplossen</span><span class="sxs-lookup"><span data-stu-id="a0b0f-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="a0b0f-123">Beleid voor probleemoplossing</span><span class="sxs-lookup"><span data-stu-id="a0b0f-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="a0b0f-124">Intune-apparaat compliance bewaken</span><span class="sxs-lookup"><span data-stu-id="a0b0f-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="a0b0f-125">Opmerking: deze stappen zijn alleen handig bij het oplossen van problemen met de voorwaardelijke toegang van de Azure Active Directory-functie.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="a0b0f-126">Het is ook mogelijk om een apparaat in quarantaine te plaatsen dat e-mailtoegang blokkeert met Exchange-beleid.</span><span class="sxs-lookup"><span data-stu-id="a0b0f-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="a0b0f-127">Meer informatie over Exchange-apparaatbeheer vindt u [hier]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="a0b0f-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
