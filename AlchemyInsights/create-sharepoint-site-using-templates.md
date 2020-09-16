---
title: Een site maken in SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732213"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="f9b27-102">SharePoint-sites maken met behulp van sjablonen</span><span class="sxs-lookup"><span data-stu-id="f9b27-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="f9b27-103">De mogelijkheid om een site op te slaan als een sjabloon, wordt niet ondersteund met moderne communicatie of team sites.</span><span class="sxs-lookup"><span data-stu-id="f9b27-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="f9b27-104">Zie [een SharePoint-site opslaan, downloaden en uploaden als een sjabloon](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)voor meer informatie over het gebruik van sjablonen.</span><span class="sxs-lookup"><span data-stu-id="f9b27-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="f9b27-105">Hier volgen enkele veelvoorkomende problemen en oplossingen in verband met het opslaan van een site of lijst als een sjabloon in SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f9b27-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="f9b27-106">**De knop site-of lijstsjabloon opslaan is niet beschikbaar of ontbreekt**</span><span class="sxs-lookup"><span data-stu-id="f9b27-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="f9b27-107">Beheerders moeten aangepaste scripts toestaan om de sjabloon functies in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="f9b27-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="f9b27-108">Zie voor gedetailleerde stappen, voorbeelden en overwegingen</span><span class="sxs-lookup"><span data-stu-id="f9b27-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="f9b27-109">Aangepaste scripts toestaan of voorkomen</span><span class="sxs-lookup"><span data-stu-id="f9b27-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="f9b27-110">De opdracht site opslaan als sjabloon wordt niet ondersteund en kan problemen veroorzaken op sites die gebruikmaken van de publicatie-infrastructuur van SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="f9b27-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="f9b27-111">**De sitesjabloon kan niet worden gemaakt of werkt niet goed**</span><span class="sxs-lookup"><span data-stu-id="f9b27-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="f9b27-112">De sjabloon mist mogelijk een [functie](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) en wordt niet geactiveerd.</span><span class="sxs-lookup"><span data-stu-id="f9b27-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="f9b27-113">Als de functie niet beschikbaar is voor het activeren van de huidige siteverzameling, kunt u de sitesjabloon niet gebruiken om een site te maken.</span><span class="sxs-lookup"><span data-stu-id="f9b27-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="f9b27-114">Kijk of een lijst of bibliotheek de [drempelwaarde voor limieten voor de lijstweergave](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) van 5000-items mag overschrijden, omdat dit kan het maken van een sitesjabloon blokkeren.</span><span class="sxs-lookup"><span data-stu-id="f9b27-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="f9b27-115">Het kan zijn dat op de site te veel resources worden gebruikt en de sitesjabloon daardoor groter is dan de limiet van 50 MB.</span><span class="sxs-lookup"><span data-stu-id="f9b27-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="f9b27-116">Er zijn problemen met het weergeven van gegevens in een lijst die een opzoekkolom gebruikt.</span><span class="sxs-lookup"><span data-stu-id="f9b27-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="f9b27-117">Zie voor meer informatie [sjabloon met gegenereerde lijst worden geen gegevens uit de juiste opzoeklijst weergegeven in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="f9b27-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="f9b27-118">Raadpleeg [sitesjablonen maken en gebruiken](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)voor meer informatie over veelvoorkomende problemen en oplossingen.</span><span class="sxs-lookup"><span data-stu-id="f9b27-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



