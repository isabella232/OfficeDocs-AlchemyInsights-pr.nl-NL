---
title: Externe gebruikers toevoegen aan een distributiegroep
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737868"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="cf65e-102">Externe gebruikers toevoegen aan een distributiegroep</span><span class="sxs-lookup"><span data-stu-id="cf65e-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="cf65e-103">Het toevoegen van een externe contactpersoon aan een distributiegroep (DG) is een proces in twee stappen:</span><span class="sxs-lookup"><span data-stu-id="cf65e-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="cf65e-104">Een e-mail contactpersoon voor de externe gebruiker maken:</span><span class="sxs-lookup"><span data-stu-id="cf65e-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="cf65e-105">Ga in het Admin Center naar de pagina \*\*\*\* > [contactpersonen](https://admin.microsoft.com/adminportal/home#/Contact) van gebruikers.</span><span class="sxs-lookup"><span data-stu-id="cf65e-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="cf65e-106">Selecteer **een contactpersoon toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="cf65e-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="cf65e-107">Typ de informatie voor uw contactpersoon en selecteer **toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="cf65e-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="cf65e-108">Voeg het e-mail contact toe aan uw DG:</span><span class="sxs-lookup"><span data-stu-id="cf65e-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="cf65e-109">Ga in het Beheercentrum naar de pagina **groeps** > [groepen.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="cf65e-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="cf65e-110">Zoek het DG waaraan u de externe gebruiker wilt toevoegen en selecteer het om het dialoogvenster bewerken te openen.</span><span class="sxs-lookup"><span data-stu-id="cf65e-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="cf65e-111">Selecteer op het tabblad **leden** de optie **alle weergeven en leden beheren**.</span><span class="sxs-lookup"><span data-stu-id="cf65e-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="cf65e-112">Selecteer **leden toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="cf65e-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="cf65e-113">Selecteer de e-mail contactpersoon die u hebt gemaakt in de vorige stap en selecteer vervolgens **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="cf65e-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="cf65e-114">Als u na het volgen van deze stappen uw externe gebruikers geen e-mails kunnen sturen naar het DG of geen e-mails van deze ontvangen, kan het zijn dat het DG is gemarkeerd om alleen e-mails van interne gebruikers toe te staan.</span><span class="sxs-lookup"><span data-stu-id="cf65e-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="cf65e-115">U deze configuratie controleren en dit oplossen door de aanwijzingen [hier](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)te volgen.</span><span class="sxs-lookup"><span data-stu-id="cf65e-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="cf65e-116">**Opmerking:** Deze instructies zijn niet van toepassing als het type van uw groep ' Office 365 groep ' in plaats van ' distributiegroep ' is.</span><span class="sxs-lookup"><span data-stu-id="cf65e-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="cf65e-117">Als dat het geval is, u de externe gebruiker rechtstreeks vanuit Outlook aan de groep toevoegen.</span><span class="sxs-lookup"><span data-stu-id="cf65e-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="cf65e-118">Gedetailleerde informatie over Office 365 groepen gasten en instructies voor het toevoegen van externe gasten zijn te vinden in [dit artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="cf65e-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  