---
title: Een site maken in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770418"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="0a321-102">SharePoint-sites maken met sjablonen</span><span class="sxs-lookup"><span data-stu-id="0a321-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="0a321-103">De mogelijkheid om een site op te slaan als sjabloon wordt niet ondersteund met moderne communicatie- of teamsites.</span><span class="sxs-lookup"><span data-stu-id="0a321-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="0a321-104">Zie [Een SharePoint-site opslaan, downloaden en uploaden als sjabloon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)voor meer informatie over het gebruik van sjablonen.</span><span class="sxs-lookup"><span data-stu-id="0a321-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="0a321-105">Hier volgen enkele veelvoorkomende problemen/oplossingen met betrekking tot het opslaan van een site of lijst als sjabloon in Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="0a321-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="0a321-106">**Knop Site/lijstsjabloon opslaan is niet beschikbaar of ontbreekt**</span><span class="sxs-lookup"><span data-stu-id="0a321-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="0a321-107">Beheerders moeten Aangepast script toestaan om de sjabloonfuncties in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="0a321-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="0a321-108">Zie voor gedetailleerde stappen, voorbeelden en overwegingen</span><span class="sxs-lookup"><span data-stu-id="0a321-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="0a321-109">Aangepast script toestaan of voorkomen</span><span class="sxs-lookup"><span data-stu-id="0a321-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="0a321-110">De opdracht Site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die de publicatieinfrastructuur van SharePoint Server gebruiken.</span><span class="sxs-lookup"><span data-stu-id="0a321-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="0a321-111">**De sitesjabloon kan niet worden gemaakt of werkt niet correct**</span><span class="sxs-lookup"><span data-stu-id="0a321-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="0a321-112">De sjabloon mist mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="0a321-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="0a321-113">Als de functie niet beschikbaar is om te activeren in de huidige siteverzameling, u de sitesjabloon niet gebruiken om een site te maken.</span><span class="sxs-lookup"><span data-stu-id="0a321-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="0a321-114">Controleer of lijsten of bibliotheken de [drempelwaarde voor lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000 items overschrijden, omdat dit het maken van een sitesjabloon kan blokkeren.</span><span class="sxs-lookup"><span data-stu-id="0a321-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="0a321-115">De site kan te veel bronnen gebruiken en daarom overschrijdt de sitesjabloon de limiet van 50 MB.</span><span class="sxs-lookup"><span data-stu-id="0a321-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="0a321-116">Er zijn problemen met het weergeven van gegevens uit een lijst die een opzoekkolom gebruikt.</span><span class="sxs-lookup"><span data-stu-id="0a321-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="0a321-117">Zie De [lijst met gegenereerde gegevens uit de juiste opzoeklijst in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)wordt niet weergegeven voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="0a321-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="0a321-118">Voor meer gedetailleerde informatie over veelvoorkomende problemen en oplossingen raadpleegt u [Sitesjablonen maken en gebruiken.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)</span><span class="sxs-lookup"><span data-stu-id="0a321-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



