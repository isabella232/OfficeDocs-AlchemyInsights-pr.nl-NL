---
title: Migratie van AIP naar MIP/Unified Labeling in het compliancecentrum
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825366"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="3528f-102">Migratie van AIP naar MIP/Unified Labeling in het compliancecentrum</span><span class="sxs-lookup"><span data-stu-id="3528f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="3528f-103">Ga als volgt te werk om te migreren van AIP-labels naar Unified Labeling in het Beveiligings- en compliancecentrum:</span><span class="sxs-lookup"><span data-stu-id="3528f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="3528f-104">**Beveiliging activeren vanuit de Azure-portal**</span><span class="sxs-lookup"><span data-stu-id="3528f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="3528f-105">Als u dit nog niet hebt gedaan, opent u een nieuw browservenster en meld [u aan bij de Azure-portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="3528f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="3528f-106">Ga naar het **Azure Information Protection-blad.**</span><span class="sxs-lookup"><span data-stu-id="3528f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="3528f-107">Klik bijvoorbeeld in het hubmenu op **Alle services** en begin gegevens te **typen** in het vak Filter.</span><span class="sxs-lookup"><span data-stu-id="3528f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="3528f-108">Selecteer **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="3528f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="3528f-109">Als u het Azure Information Protection-blad nog niet eerder [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) hebt geopend, bekijkt u de een-tijd extra stappen om dit blad toe te voegen aan de portal.</span><span class="sxs-lookup"><span data-stu-id="3528f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="3528f-110">Als u het Azure Information Protection-blade wilt openen, moet u een [Azure Information Protection Premium-abonnement](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) hebben of een Office 365-abonnement met Rights Management.</span><span class="sxs-lookup"><span data-stu-id="3528f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="3528f-111">Als u een van deze abonnementen hebt, maar een bericht ziet dat een geldig abonnement niet kan worden gevonden, [neem dan contact](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) op met Microsoft Support of gebruik uw standaardondersteuningskanalen.</span><span class="sxs-lookup"><span data-stu-id="3528f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="3528f-112">Zoek de **menuopties** beheren en selecteer **Activering van beveiliging.**</span><span class="sxs-lookup"><span data-stu-id="3528f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="3528f-113">Klik **op Activeren** en bevestig uw actie.</span><span class="sxs-lookup"><span data-stu-id="3528f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="3528f-114">Wanneer de activering is voltooid, wordt op de informatiebalk **weergegeven dat activering is voltooid.**</span><span class="sxs-lookup"><span data-stu-id="3528f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="3528f-115">**Azure Information Protection-labels migreren naar Office 365 & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="3528f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="3528f-116">Zorg ervoor dat u bent aangemeld als gebruiker met de machtiging Globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="3528f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="3528f-117">Ga naar het **Azure Information Protection-blad.**</span><span class="sxs-lookup"><span data-stu-id="3528f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="3528f-118">Selecteer unified labeling in **de** optie Menu **beheren.**</span><span class="sxs-lookup"><span data-stu-id="3528f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="3528f-119">Klik op **azure information protection - Unified labeling** blade op **Activeren** en volg de onlineinstructies.</span><span class="sxs-lookup"><span data-stu-id="3528f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="3528f-120">**Opmerking:** Controleer of u de juiste machtigingen hebt voordat u de migratie van & Beveiligingscentrum activeert.</span><span class="sxs-lookup"><span data-stu-id="3528f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="3528f-121">Zie deze artikelen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="3528f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="3528f-122">Moet u een globale beheerder zijn om Azure Information Protection te configureren of kan ik delegeren aan andere beheerders?</span><span class="sxs-lookup"><span data-stu-id="3528f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="3528f-123">Belangrijke informatie over beheerdersrollen na de migratie naar & compliancecentrum.</span><span class="sxs-lookup"><span data-stu-id="3528f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="3528f-124">Zie Labels migreren voor meer informatie over de migratie van AIP naar Unified Labeling naar het Beveiligings- en [compliancecentrum.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="3528f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
