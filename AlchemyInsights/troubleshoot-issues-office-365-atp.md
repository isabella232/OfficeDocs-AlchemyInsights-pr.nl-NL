---
title: Problemen oplossen met Microsoft Defender voor Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801402"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="9ffa2-102">Problemen oplossen met Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="9ffa2-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="9ffa2-103">**Merkt u vertraging op de bezorging van een e-mailbericht** ?</span><span class="sxs-lookup"><span data-stu-id="9ffa2-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="9ffa2-104">Gebruik de optie voor dynamische bezorging van de beleidsregels voor veilige bijlagen.</span><span class="sxs-lookup"><span data-stu-id="9ffa2-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="9ffa2-105">Hiermee voorkomt u de bezorgings vertraging van e-mailberichten bij het beschermen van de ontvangers tegen kwaadwillende bestanden</span><span class="sxs-lookup"><span data-stu-id="9ffa2-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="9ffa2-106">**Wilt u onjuiste positieve of onjuiste negatieven melden** ?</span><span class="sxs-lookup"><span data-stu-id="9ffa2-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="9ffa2-107">Gebruik deze koppeling om het bestand in te dienen voor analyse: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="9ffa2-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="9ffa2-108">**Wist u dat u de bescherming van ATP voor veilige koppelingen kunt inschakelen voor e-mail die wordt verzonden tussenpersonen in uw organisatie** ?</span><span class="sxs-lookup"><span data-stu-id="9ffa2-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="9ffa2-109">Ga als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="9ffa2-109">Follow these steps:</span></span>
    1. <span data-ttu-id="9ffa2-110">Ga naar https://protection.office.com en meld u aan.</span><span class="sxs-lookup"><span data-stu-id="9ffa2-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="9ffa2-111">Ga naar **Threat management**  >  **Policy**  >  **veilige koppelingen** voor het beleid voor risicobeheer.</span><span class="sxs-lookup"><span data-stu-id="9ffa2-111">Go to **Threat management** > **Policy** > **Safe Links** .</span></span>
    3. <span data-ttu-id="9ffa2-112">Onder **beleidsregels die van toepassing zijn op bepaalde geadresseerden** , een beleid bewerken (of toevoegen).</span><span class="sxs-lookup"><span data-stu-id="9ffa2-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="9ffa2-113">Selecteer **veilige koppelingen toepassen op berichten die binnen de organisatie worden verzonden** .</span><span class="sxs-lookup"><span data-stu-id="9ffa2-113">Select **Apply safe links to messages sent within the organization** .</span></span>
    5. <span data-ttu-id="9ffa2-114">Sla uw beleid op en zorg ervoor dat uw wijzigingen worden doorgevoerd in de bewerkings interface van uw datacenter.</span><span class="sxs-lookup"><span data-stu-id="9ffa2-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="9ffa2-115">Zie [Microsoft Defender voor Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)voor meer informatie over ATP.</span><span class="sxs-lookup"><span data-stu-id="9ffa2-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>