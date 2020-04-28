---
title: Externe gebruikers toevoegen aan een distributiegroep
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910927"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="fada1-102">Externe gebruikers toevoegen aan een distributiegroep</span><span class="sxs-lookup"><span data-stu-id="fada1-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="fada1-103">Het toevoegen van een extern contact aan een distributiegroep (DG) is een proces in twee stappen:</span><span class="sxs-lookup"><span data-stu-id="fada1-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="fada1-104">Een e-mailcontactpersoon maken voor de externe gebruiker:</span><span class="sxs-lookup"><span data-stu-id="fada1-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="fada1-105">Ga in het beheercentrum naar de pagina > [Gebruikerscontactpersonen.](https://admin.microsoft.com/adminportal/home#/Contact) **Users**</span><span class="sxs-lookup"><span data-stu-id="fada1-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="fada1-106">Selecteer **Een contactpersoon toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="fada1-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="fada1-107">Typ de gegevens voor uw contactpersoon en selecteer **Toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="fada1-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="fada1-108">Voeg de mailcontact toe aan uw DG:</span><span class="sxs-lookup"><span data-stu-id="fada1-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="fada1-109">Ga in het beheercentrum naar de pagina **Groepen** > [groepen.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="fada1-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="fada1-110">Zoek de DG waaraan u de externe gebruiker wilt toevoegen en selecteer deze om het dialoogvenster bewerken te openen.</span><span class="sxs-lookup"><span data-stu-id="fada1-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="fada1-111">Selecteer op het tabblad **Leden** **alle leden weergeven en leden beheren**.</span><span class="sxs-lookup"><span data-stu-id="fada1-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="fada1-112">Selecteer **Leden toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="fada1-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="fada1-113">Selecteer de e-mailcontactpersoon die u in de vorige stap hebt gemaakt en selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="fada1-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="fada1-114">Als uw externe gebruikers na het volgen van deze stappen geen e-mails naar de DG kunnen verzenden of er geen e-mails van kunnen ontvangen, kan het zijn dat de DG is gemarkeerd om alleen e-mails van interne gebruikers toe te staan.</span><span class="sxs-lookup"><span data-stu-id="fada1-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="fada1-115">U deze configuratie controleren en deze herstellen volgens de aanwijzingen [hier.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="fada1-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="fada1-116">**Let op:** Deze instructies zijn niet van toepassing als het type van uw groep 'Microsoft 365-groep' is in plaats van 'Distributiegroep'.</span><span class="sxs-lookup"><span data-stu-id="fada1-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="fada1-117">Als dat het geval is, u de externe gebruiker rechtstreeks vanuit Outlook aan de groep toevoegen.</span><span class="sxs-lookup"><span data-stu-id="fada1-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="fada1-118">Gedetailleerde informatie over gasten van Microsoft 365 Groups en instructies voor het toevoegen van externe gasten vindt u in [dit artikel.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)</span><span class="sxs-lookup"><span data-stu-id="fada1-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  