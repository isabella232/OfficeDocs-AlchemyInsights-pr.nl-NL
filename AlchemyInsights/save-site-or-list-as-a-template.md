---
title: Site of lijst opslaan als een sjabloon
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243261"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="82113-102">Site of lijst opslaan als een sjabloon</span><span class="sxs-lookup"><span data-stu-id="82113-102">Save site or list as a template</span></span>

<span data-ttu-id="82113-103">SharePoint-sitesjablonen zijn vooraf gedefinieerde definities ontworpen rond een bepaalde zakelijke behoefte.</span><span class="sxs-lookup"><span data-stu-id="82113-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="82113-104">Zie [werken met sjablonen voor verschillende typen SharePoint-sites maken](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="82113-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="82113-105">Hier vindt u enkele algemene problemen/oplossingen met betrekking tot het opslaan van een Site of lijst als sjabloon in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="82113-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="82113-106">**Opslaan/sitelijst sjabloonknop is niet beschikbaar of ontbreekt**.</span><span class="sxs-lookup"><span data-stu-id="82113-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="82113-107">Aangepast Script dat moet beheerders waarmee de sjabloonfuncties.</span><span class="sxs-lookup"><span data-stu-id="82113-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="82113-108">Zie voor gedetailleerde stappen, voorbeelden en overwegingen [toestaan of voorkomen van aangepast script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="82113-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="82113-109">De site opslaan als sjabloon, opdracht wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de SharePoint Server Publishing infrastructuur.</span><span class="sxs-lookup"><span data-stu-id="82113-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="82113-110">**De sitesjabloon kan niet worden gemaakt of niet goed werkt**</span><span class="sxs-lookup"><span data-stu-id="82113-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="82113-111">De sjabloon een [onderdeel](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ontbreekt en won't activeren.</span><span class="sxs-lookup"><span data-stu-id="82113-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="82113-112">Als de functie niet beschikbaar in de huidige siteverzameling activeren is, kunt u de sjabloon niet gebruiken om een site te maken.</span><span class="sxs-lookup"><span data-stu-id="82113-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="82113-113">Controleer als lijsten of bibliotheken meer dan de [Drempelwaarde voor lijstweergave limiet](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000 artikelen als dit het maken van een sitesjabloon kunt blokkeren.</span><span class="sxs-lookup"><span data-stu-id="82113-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="82113-114">De site mogelijk te veel bronnen gebruikt en daarom de sitesjabloon bevat meer dan 50 megabyte (MB).</span><span class="sxs-lookup"><span data-stu-id="82113-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="82113-115">Er zijn problemen bij het weergeven van gegevens uit een lijst die een opzoekkolom gebruikt.</span><span class="sxs-lookup"><span data-stu-id="82113-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="82113-116">Zie voor meer informatie de [lijst sjabloon gegenereerde gegevens in de juiste opzoeklijst in SharePoint Online niet wordt weergegeven](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="82113-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="82113-117">Neem voor meer informatie over bekende problemen en oplossingen verwijzing, [sitesjablonen maken en gebruiken](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="82113-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

