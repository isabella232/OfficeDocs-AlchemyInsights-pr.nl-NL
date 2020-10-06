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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366423"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="910ad-102">Voorwaardelijke toegang voor Exchange controleren</span><span class="sxs-lookup"><span data-stu-id="910ad-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="910ad-103">Gebruikers met voorwaardelijke toegang ontvangen een e-mail melding als ze niet voldoen aan de toegangsvereisten van uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="910ad-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="910ad-104">We raden een of meer van de volgende oplossingen aan om dit op te lossen:</span><span class="sxs-lookup"><span data-stu-id="910ad-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="910ad-105">Als u ervan wordt uitgegaan dat het apparaat is ingeschreven, adviseert u de gebruiker om naar de bedrijfsportal-app te gaan en controleert u of deze wordt weergegeven in de bedrijfsportal.</span><span class="sxs-lookup"><span data-stu-id="910ad-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="910ad-106">Als dit niet het geval is, moet de gebruiker het apparaat registreren.</span><span class="sxs-lookup"><span data-stu-id="910ad-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="910ad-107">Ga in de Azure-Portal naar intune > apparaatcompatibiliteit.</span><span class="sxs-lookup"><span data-stu-id="910ad-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="910ad-108">Klik onder monitor op apparaatcompatibiliteit.</span><span class="sxs-lookup"><span data-stu-id="910ad-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="910ad-109">Bekijk het nalevings rapport van uw apparaat om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel.</span><span class="sxs-lookup"><span data-stu-id="910ad-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="910ad-110">Ga in de Azure-Portal naar intune > apparaatcompatibiliteit.</span><span class="sxs-lookup"><span data-stu-id="910ad-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="910ad-111">Klik onder beheren op beleidsregels.</span><span class="sxs-lookup"><span data-stu-id="910ad-111">Under Manage, click Policies.</span></span> <span data-ttu-id="910ad-112">Controleer in de lijst met nalevingsbeleid of een profiel is toegewezen aan het apparaat van uw gebruikers.</span><span class="sxs-lookup"><span data-stu-id="910ad-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="910ad-113">Als u geen profiel hebt toegewezen, kan intune de nalevingsstatus van het apparaat niet bevestigen.</span><span class="sxs-lookup"><span data-stu-id="910ad-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="910ad-114">De voorwaardelijke toegang-opdracht van de gebruiker bewerken.</span><span class="sxs-lookup"><span data-stu-id="910ad-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="910ad-115">Ga in de Azure-Portal naar **intune**-  >  beleid voor**voorwaardelijke toegang**  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="910ad-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="910ad-116">Selecteer een beleid in de lijst.</span><span class="sxs-lookup"><span data-stu-id="910ad-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="910ad-117">Klik op gebruikers en groepen.</span><span class="sxs-lookup"><span data-stu-id="910ad-117">Click Users and groups.</span></span>
4. <span data-ttu-id="910ad-118">Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de lijst toevoegen.</span><span class="sxs-lookup"><span data-stu-id="910ad-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="910ad-119">Voeg ze toe aan de lijst uitsluiten om ervoor te zorgen dat iemand van het beleid weglaat.</span><span class="sxs-lookup"><span data-stu-id="910ad-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="910ad-120">Handige koppelingen:</span><span class="sxs-lookup"><span data-stu-id="910ad-120">Helpful links:</span></span>

[<span data-ttu-id="910ad-121">Overzicht van apparaatcompatibiliteit</span><span class="sxs-lookup"><span data-stu-id="910ad-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="910ad-122">Oplossing van een certificeringsinstantie</span><span class="sxs-lookup"><span data-stu-id="910ad-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="910ad-123">Beleid voor probleemoplossing</span><span class="sxs-lookup"><span data-stu-id="910ad-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="910ad-124">Naleving van intune-apparaat controleren</span><span class="sxs-lookup"><span data-stu-id="910ad-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="910ad-125">Opmerking: deze stappen zijn alleen bedoeld voor het oplossen van de voorwaardelijke toegang van de Azure Active Directory-functie.</span><span class="sxs-lookup"><span data-stu-id="910ad-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="910ad-126">Het is ook mogelijk om een apparaat te gebruiken dat het e-mailadres van de e-mail met Exchange-beleid blokkeert.</span><span class="sxs-lookup"><span data-stu-id="910ad-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="910ad-127">[Hier](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)vindt u meer informatie over Exchange Device Management.</span><span class="sxs-lookup"><span data-stu-id="910ad-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
