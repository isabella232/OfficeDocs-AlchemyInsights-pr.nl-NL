---
title: Het maken van een site in SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: a964751e52972875a8794ce311546f5816a36ca6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34753703"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="27c6b-102">SharePoint-sites met behulp van sjablonen maken</span><span class="sxs-lookup"><span data-stu-id="27c6b-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="27c6b-103">SharePoint-sitesjablonen zijn vooraf gedefinieerde definities ontworpen rond een bepaalde zakelijke behoefte.</span><span class="sxs-lookup"><span data-stu-id="27c6b-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="27c6b-104">Zie [werken met sjablonen voor verschillende typen SharePoint-sites maken](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="27c6b-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="27c6b-105">Hier vindt u enkele algemene problemen/oplossingen met betrekking tot het opslaan van een Site of lijst als sjabloon in Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="27c6b-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="27c6b-106">**Knop Opslaan/sitelijst-sjabloon is niet beschikbaar of ontbreekt**</span><span class="sxs-lookup"><span data-stu-id="27c6b-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="27c6b-107">Aangepast Script dat moet beheerders waarmee de sjabloonfuncties.</span><span class="sxs-lookup"><span data-stu-id="27c6b-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="27c6b-108">Zie voor gedetailleerde stappen voorbeelden en overwegingen</span><span class="sxs-lookup"><span data-stu-id="27c6b-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="27c6b-109">Toestaan of voorkomen van aangepast script</span><span class="sxs-lookup"><span data-stu-id="27c6b-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="27c6b-110">De site opslaan als sjabloon, opdracht wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de SharePoint Server Publishing infrastructuur.</span><span class="sxs-lookup"><span data-stu-id="27c6b-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="27c6b-111">De sitesjabloon kan niet worden gemaakt of niet goed werkt.</span><span class="sxs-lookup"><span data-stu-id="27c6b-111">The site template cannot be created or does not work correctly.</span></span>

<span data-ttu-id="27c6b-112">De sjabloon een [onderdeel](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ontbreekt en won't activeren.</span><span class="sxs-lookup"><span data-stu-id="27c6b-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="27c6b-113">Als de functie niet beschikbaar in de huidige siteverzameling activeren is, kunt u de sjabloon niet gebruiken om een site te maken.</span><span class="sxs-lookup"><span data-stu-id="27c6b-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="27c6b-114">Controleer als lijsten of bibliotheken meer dan de [Drempelwaarde voor lijstweergave limiet](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000 artikelen als dit het maken van een sitesjabloon kunt blokkeren.</span><span class="sxs-lookup"><span data-stu-id="27c6b-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="27c6b-115">De site mogelijk te veel bronnen gebruikt en daarom de sitesjabloon overschrijdt de limiet van 50 MB.</span><span class="sxs-lookup"><span data-stu-id="27c6b-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="27c6b-116">Er zijn problemen bij het weergeven van gegevens uit een lijst die een opzoekkolom gebruikt.</span><span class="sxs-lookup"><span data-stu-id="27c6b-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="27c6b-117">Zie voor meer informatie de [lijst sjabloon gegenereerde gegevens in de juiste opzoeklijst in SharePoint Online niet wordt weergegeven](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="27c6b-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="27c6b-118">Raadpleeg voor meer gedetailleerde informatie over algemene problemen en oplossingen, [sitesjablonen maken en gebruiken](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="27c6b-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



