---
title: Voorwaardelijke toegang voor Intune bewaken
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427424"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="e0c84-102">Voorwaardelijke toegang voor Intune bewaken</span><span class="sxs-lookup"><span data-stu-id="e0c84-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="e0c84-103">Gebruikers aan wie voorwaardelijke toegang is gericht, ontvangen een e-mailmelding als ze niet aan de toegangsvereisten van uw organisatie voldoen.</span><span class="sxs-lookup"><span data-stu-id="e0c84-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="e0c84-104">U wordt aangeraden een of meer van de volgende oplossingen op te lossen:</span><span class="sxs-lookup"><span data-stu-id="e0c84-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="e0c84-105">Als ervan wordt uitgegaan dat het apparaat is geregistreerd, adviseert u de gebruiker naar de bedrijfsportal-app te gaan en te controleren of deze wordt weergegeven in de bedrijfsportal.</span><span class="sxs-lookup"><span data-stu-id="e0c84-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e0c84-106">Als dat niet zo is, moet de gebruiker het apparaat registreren.</span><span class="sxs-lookup"><span data-stu-id="e0c84-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="e0c84-107">Ga in de Azure Portal naar **Intune**  >  **Device compliance.**</span><span class="sxs-lookup"><span data-stu-id="e0c84-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="e0c84-108">Als u het rapport apparaat compliance wilt bekijken om te controleren of het apparaat van de gebruiker is gemarkeerd als compatibel, klikt u onder **Beeldscherm** op **Apparaat compliance.**</span><span class="sxs-lookup"><span data-stu-id="e0c84-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="e0c84-109">Ga in de Azure Portal naar **Intune**  >  **Device compliance.**</span><span class="sxs-lookup"><span data-stu-id="e0c84-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="e0c84-110">Klik **onder Beheren op** **Beleid.**</span><span class="sxs-lookup"><span data-stu-id="e0c84-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="e0c84-111">Controleer in de lijst met nalevingsbeleidsregels of een profiel is toegewezen aan het apparaat van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="e0c84-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e0c84-112">Als er geen profiel is toegewezen, kan Intune de compatibiliteitsstatus van het apparaat niet bevestigen.</span><span class="sxs-lookup"><span data-stu-id="e0c84-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="e0c84-113">Bewerk de toewijzing van voorwaardelijke toegang van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="e0c84-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="e0c84-114">Navigeer in de Azure Portal naar **Intune-beleidsregels** voor voorwaardelijke toegang, selecteer een beleid in de lijst en klik  >    >  op Gebruikers **en groepen.**</span><span class="sxs-lookup"><span data-stu-id="e0c84-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="e0c84-115">Als u een bepaald beleid op iemand wilt richten, voegt u deze toe aan de **lijst Opnemen.**</span><span class="sxs-lookup"><span data-stu-id="e0c84-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="e0c84-116">Als u ervoor wilt zorgen dat een persoon in het beleid wordt **weggelaten,** voegt u deze toe aan de lijst Uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="e0c84-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="e0c84-117">**Handige koppelingen:**</span><span class="sxs-lookup"><span data-stu-id="e0c84-117">**Helpful links:**</span></span>

- [<span data-ttu-id="e0c84-118">Overzicht van apparaat compliance</span><span class="sxs-lookup"><span data-stu-id="e0c84-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="e0c84-119">Problemen met CA oplossen</span><span class="sxs-lookup"><span data-stu-id="e0c84-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="e0c84-120">Beleid voor probleemoplossing</span><span class="sxs-lookup"><span data-stu-id="e0c84-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="e0c84-121">Intune-apparaat compliance bewaken</span><span class="sxs-lookup"><span data-stu-id="e0c84-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="e0c84-122">Deze stappen zijn alleen nuttig bij het oplossen van problemen met de voorwaardelijke toegang van de Azure Active Directory-functie.</span><span class="sxs-lookup"><span data-stu-id="e0c84-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e0c84-123">Het is ook mogelijk om een apparaat in quarantaine te plaatsen dat e-mailtoegang blokkeert met Exchange-beleid.</span><span class="sxs-lookup"><span data-stu-id="e0c84-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e0c84-124">Meer informatie over Exchange-apparaatbeheer vindt u [**hier.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="e0c84-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
