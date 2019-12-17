---
title: Site of lijst opslaan als sjabloon
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048719"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="a17c5-102">Site of lijst opslaan als sjabloon</span><span class="sxs-lookup"><span data-stu-id="a17c5-102">Save site or list as a template</span></span>

<span data-ttu-id="a17c5-103">SharePoint-sitesjablonen zijn vooraf gedefinieerde definities die zijn ontworpen rond een bepaalde zakelijke behoefte.</span><span class="sxs-lookup"><span data-stu-id="a17c5-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="a17c5-104">Zie [sjablonen gebruiken om verschillende soorten SharePoint-sites te maken](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a17c5-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="a17c5-105">Hier volgen enkele veelvoorkomende problemen/oplossingen met betrekking tot het opslaan van een site of lijst als een sjabloon in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="a17c5-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="a17c5-106">De **knop site/lijstsjabloon opslaan is niet beschikbaar of ontbreekt**.</span><span class="sxs-lookup"><span data-stu-id="a17c5-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="a17c5-107">Beheerders moeten het aangepaste script toestaan om de sjabloonfuncties in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="a17c5-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="a17c5-108">Zie voor gedetailleerde stappen, voorbeelden en overwegingen [toestaan of voorkomen dat aangepast script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="a17c5-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="a17c5-109">De opdracht site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de SharePoint Server Publishing-infrastructuur.</span><span class="sxs-lookup"><span data-stu-id="a17c5-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="a17c5-110">**De sitesjabloon kan niet worden gemaakt of werkt niet correct**</span><span class="sxs-lookup"><span data-stu-id="a17c5-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="a17c5-111">De sjabloon ontbreekt mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="a17c5-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="a17c5-112">Als de functie niet beschikbaar is om te activeren in de huidige siteverzameling, u de sitesjabloon niet gebruiken om een site te maken.</span><span class="sxs-lookup"><span data-stu-id="a17c5-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="a17c5-113">Controleer of er lijsten of bibliotheken zijn die de [limiet drempel voor lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000 items overschrijden, omdat hierdoor het maken van een sitesjabloon kan worden geblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="a17c5-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="a17c5-114">De site gebruikt mogelijk te veel bronnen en daarom overschrijdt de sitesjabloon de limiet van 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="a17c5-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="a17c5-115">Er zijn problemen met het weergeven van gegevens uit een lijst die gebruikmaakt van een opzoekkolom.</span><span class="sxs-lookup"><span data-stu-id="a17c5-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="a17c5-116">Zie voor meer informatie, [sjabloon gegenereerde lijstgegevens uit de juiste opzoeklijst in SharePoint Online niet weergegeven](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="a17c5-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="a17c5-117">Voor meer gedetailleerde informatie over veelvoorkomende problemen en oplossingen raadpleegt u [sitesjablonen maken en gebruiken](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="a17c5-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

