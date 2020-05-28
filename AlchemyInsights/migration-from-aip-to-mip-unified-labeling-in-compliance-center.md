---
title: Migratie van AIP naar MIP/Unified Labeling in het Compliance Center
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236359"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="0339e-102">Migratie van AIP naar MIP/Unified Labeling in het Compliance Center</span><span class="sxs-lookup"><span data-stu-id="0339e-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="0339e-103">Ga als volgt te werk om van AIP-labels naar Unified Labeling in het beveiligings- en compliancecentrum te migreren:</span><span class="sxs-lookup"><span data-stu-id="0339e-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="0339e-104">**Beveiliging activeren vanuit de Azure-portal**</span><span class="sxs-lookup"><span data-stu-id="0339e-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="0339e-105">Als u dit nog niet hebt gedaan, opent u een nieuw browservenster en [meldt u zich aan bij de Azure-portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="0339e-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="0339e-106">Navigeer naar het azure **information protection-blad.**</span><span class="sxs-lookup"><span data-stu-id="0339e-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="0339e-107">Klik bijvoorbeeld in het hubmenu op **Alle services** en typ **gegevens** in het vak Filter.</span><span class="sxs-lookup"><span data-stu-id="0339e-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="0339e-108">Selecteer **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="0339e-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="0339e-109">Als u het Azure Information Protection-blad nog niet eerder hebt geopend, raadpleegt u de [eenmalige extra stappen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) om dit blad aan de portal toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="0339e-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="0339e-110">Als u het azure information protection-blad wilt openen, moet u een [Azure Information Protection Premium-abonnement](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) of een Office 365-abonnement hebben dat rechtenbeheer bevat.</span><span class="sxs-lookup"><span data-stu-id="0339e-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="0339e-111">Als u een van deze abonnementen hebt, maar een bericht ziet dat een geldig abonnement niet kan worden gevonden, neemt [u contact op met Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) of gebruikt u uw standaardondersteuningskanalen.</span><span class="sxs-lookup"><span data-stu-id="0339e-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="0339e-112">Zoek de **menuopties beheren** en selecteer **Beveiligingsactivering**.</span><span class="sxs-lookup"><span data-stu-id="0339e-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="0339e-113">Klik **op Activeren**en bevestig uw actie.</span><span class="sxs-lookup"><span data-stu-id="0339e-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="0339e-114">Wanneer de activering is voltooid, wordt op de informatiebalk **activering weergegeven die is voltooid.**</span><span class="sxs-lookup"><span data-stu-id="0339e-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="0339e-115">**Azure Information Protection-labels migreren naar Office 365-beveiliging & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="0339e-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="0339e-116">Zorg ervoor dat u bent ingelogd als gebruiker met toestemming van globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="0339e-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="0339e-117">Navigeer naar het azure **information protection-blad.**</span><span class="sxs-lookup"><span data-stu-id="0339e-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="0339e-118">Selecteer **Unified labeling**in de **menuoptie Beheren** .</span><span class="sxs-lookup"><span data-stu-id="0339e-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="0339e-119">Klik op het **Azure Information Protection - Unified-labelblad** op **Activeren** en volg de online instructies.</span><span class="sxs-lookup"><span data-stu-id="0339e-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="0339e-120">**Opmerking:** controleer of u over de juiste machtigingen beschikt voordat u de migratie van security & Compliance Center activeert.</span><span class="sxs-lookup"><span data-stu-id="0339e-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="0339e-121">Zie deze artikelen voor meer info:</span><span class="sxs-lookup"><span data-stu-id="0339e-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="0339e-122">Moet u een globale beheerder zijn om Azure Information Protection te configureren of kan ik delegeren aan andere beheerders?</span><span class="sxs-lookup"><span data-stu-id="0339e-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="0339e-123">Belangrijke informatie over administratieve rollen na migratie naar Security & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="0339e-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="0339e-124">Zie [Labels migreren](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)voor meer informatie over de AIP naar Unified Labeling-migratie naar Beveiligings- en Compliancecenter.</span><span class="sxs-lookup"><span data-stu-id="0339e-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
