---
title: Een organisatierelatie maken om uw gebruikers in staat te stellen samen te werken met een andere organisatie
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
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816123"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="342f3-102">Een organisatierelatie maken om uw gebruikers in staat te stellen samen te werken met een andere organisatie</span><span class="sxs-lookup"><span data-stu-id="342f3-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="342f3-103">Ga vanuit het dashboard van het Microsoft 365-beheercentrum naar  >  **Admin Exchange.**</span><span class="sxs-lookup"><span data-stu-id="342f3-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="342f3-104">Ga naar **delen van**  >  **organisaties.**</span><span class="sxs-lookup"><span data-stu-id="342f3-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="342f3-105">Klik **onder Delen van** organisaties op **Nieuw.**</span><span class="sxs-lookup"><span data-stu-id="342f3-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="342f3-106">Typ **in de nieuwe organisatierelatie** in het vak **Relatienaam** een vriendelijke naam voor de organisatierelatie.</span><span class="sxs-lookup"><span data-stu-id="342f3-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="342f3-107">Typ in **het vak Domeinen** om te delen met het domein voor de externe office 365- of Exchange-on-premises organisatie die u uw agenda's wilt laten zien.</span><span class="sxs-lookup"><span data-stu-id="342f3-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="342f3-108">Als u meer dan één domein wilt invoeren, scheidt u de domeinnamen met een komma.</span><span class="sxs-lookup"><span data-stu-id="342f3-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="342f3-109">U kunt bijvoorbeeld contoso.com, service.contoso.com.</span><span class="sxs-lookup"><span data-stu-id="342f3-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="342f3-110">Schakel het **selectievakje Agenda gratis/bezet delen inschakelen** in om delen van agenda's in te stellen met de domeinen die u hebt vermeld.</span><span class="sxs-lookup"><span data-stu-id="342f3-110">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed.</span></span> <span data-ttu-id="342f3-111">Stel het niveau voor delen in voor informatie over het delen van agenda's en stel in welke gebruikers agenda-informatie gratis/bezet kunnen delen.</span><span class="sxs-lookup"><span data-stu-id="342f3-111">Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="342f3-112">Als u het gratis/bezet toegangsniveau wilt instellen, selecteert u een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="342f3-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="342f3-113">**Agendabeschikbaarheidsinfo met alleen tijd**</span><span class="sxs-lookup"><span data-stu-id="342f3-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="342f3-114">**Agenda vrij/bezet met tijd, onderwerp en locatie**</span><span class="sxs-lookup"><span data-stu-id="342f3-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="342f3-115">Selecteer een van de volgende opties om in te stellen welke gebruikers de agenda gratis/bezet zullen delen:</span><span class="sxs-lookup"><span data-stu-id="342f3-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="342f3-116">**Iedereen in uw organisatie**</span><span class="sxs-lookup"><span data-stu-id="342f3-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="342f3-117">**Een opgegeven beveiligingsgroep**</span><span class="sxs-lookup"><span data-stu-id="342f3-117">**A specified security group**</span></span>  

<span data-ttu-id="342f3-118">Klik **op Bladeren** om de beveiligingsgroep uit een lijst te kiezen en klik vervolgens op **OK.**</span><span class="sxs-lookup"><span data-stu-id="342f3-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="342f3-119">Klik **op Opslaan** om de organisatierelatie te maken.</span><span class="sxs-lookup"><span data-stu-id="342f3-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="342f3-120">**Opmerking:** Configuraties met verschillende tenants ondersteunen geen persoonlijke contactpersonen voor gratis/bezet zoeken.</span><span class="sxs-lookup"><span data-stu-id="342f3-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="342f3-121">Contactpersonen moeten worden opgenomen in de algemene adreslijst voor gratis/bezet zoeken om te kunnen werken.</span><span class="sxs-lookup"><span data-stu-id="342f3-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="342f3-122">**Voor een volledig begrip van dit onderwerp, lees:**</span><span class="sxs-lookup"><span data-stu-id="342f3-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="342f3-123">Een organisatierelatie maken in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="342f3-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="342f3-124">Een organisatierelatie wijzigen in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="342f3-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="342f3-125">Een organisatierelatie verwijderen in Exchange Online</span><span class="sxs-lookup"><span data-stu-id="342f3-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
