---
title: Externe gebruikers toevoegen aan een distributiegroep
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663508"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="ca86a-102">Externe gebruikers toevoegen aan een distributiegroep</span><span class="sxs-lookup"><span data-stu-id="ca86a-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="ca86a-103">Het toevoegen van een externe contactpersoon aan een distributiegroep (DG) bestaat uit twee stappen:</span><span class="sxs-lookup"><span data-stu-id="ca86a-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="ca86a-104">Een e-mail contactpersoon voor de externe gebruiker maken:</span><span class="sxs-lookup"><span data-stu-id="ca86a-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="ca86a-105">Ga naar de **Users**  >  pagina[contactpersonen](https://admin.microsoft.com/adminportal/home#/Contact) van gebruikers in het Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="ca86a-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="ca86a-106">Selecteer **een contactpersoon toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="ca86a-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="ca86a-107">Typ de gegevens voor de contactpersoon en selecteer **toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="ca86a-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="ca86a-108">De e-mail contactpersoon toevoegen aan de DG:</span><span class="sxs-lookup"><span data-stu-id="ca86a-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="ca86a-109">Ga in het Beheercentrum naar de pagina **groepen**  >  [groepen](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="ca86a-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="ca86a-110">Ga naar de DG waaraan u de externe gebruiker wilt toevoegen en selecteer deze om het dialoogvenster bewerken te openen.</span><span class="sxs-lookup"><span data-stu-id="ca86a-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="ca86a-111">Selecteer op het tabblad **leden** de optie **AllesWeergeven en leden beheren**.</span><span class="sxs-lookup"><span data-stu-id="ca86a-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="ca86a-112">Selecteer **leden toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="ca86a-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="ca86a-113">Selecteer de e-mail contactpersoon die u in de vorige stap hebt gemaakt en selecteer vervolgens **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="ca86a-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="ca86a-114">Als uw externe gebruikers na deze stappen niet e-mailberichten kunnen verzenden naar de DG of geen e-mailberichten ontvangen, is het mogelijk dat de DG alleen is gemarkeerd voor het toestaan van e-mailberichten van interne gebruikers.</span><span class="sxs-lookup"><span data-stu-id="ca86a-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="ca86a-115">U kunt deze configuratie controleren en deze oplossing volgen op de [onderstaande instructies.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)</span><span class="sxs-lookup"><span data-stu-id="ca86a-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="ca86a-116">**Opmerking:** Deze instructies zijn niet van toepassing als het type van de groep ' Microsoft 365 Group ' in plaats van ' distributiegroep ' is.</span><span class="sxs-lookup"><span data-stu-id="ca86a-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="ca86a-117">Als dat het geval is, kunt u de externe gebruiker rechtstreeks toevoegen aan de groep vanuit Outlook.</span><span class="sxs-lookup"><span data-stu-id="ca86a-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="ca86a-118">In [dit artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)vindt u meer informatie over gasten van microsoft 365 en de instructies voor het toevoegen van externe gast groepen.</span><span class="sxs-lookup"><span data-stu-id="ca86a-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  