---
title: Invoegvoegingen implementeren voor Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233516"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="6940a-102">Invoegvoegingen implementeren voor Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="6940a-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="6940a-103">Gecentraliseerde implementatie is de aanbevolen manier om Office te implementeren voor gebruikers en groepen binnen uw organisatie.</span><span class="sxs-lookup"><span data-stu-id="6940a-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="6940a-104">Als u invoegvoegingen wilt implementeren, volgt u de onderstaande stappen:</span><span class="sxs-lookup"><span data-stu-id="6940a-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="6940a-105">**Opmerking:** Zie Invoegvoegingen weergeven, beheren en installeren in Office programma's als u invoegprogramma's wilt installeren voor Office [als individuele gebruiker.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="6940a-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="6940a-106">Zorg er ook voor dat individuele overname van Office Store-invoegvoegingen is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="6940a-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> <span data-ttu-id="6940a-107">Zie Invoegdownloads voorkomen door de store Office alle clients uit te schakelen [(behalve Outlook) voor meer informatie.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)</span><span class="sxs-lookup"><span data-stu-id="6940a-107">For details, see [Prevent add-in downloads by turning off the Office Store across all clients (Except Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).</span></span>

1. <span data-ttu-id="6940a-108">Zorg ervoor dat uw omgeving voldoet aan de vereisten voor de implementatie van invoegvoegingen met gecentraliseerde implementatie.</span><span class="sxs-lookup"><span data-stu-id="6940a-108">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="6940a-109">Zie Vereisten voor [meer informatie.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)</span><span class="sxs-lookup"><span data-stu-id="6940a-109">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="6940a-110">Ga naar **Instellingen**  >  **Geïntegreerde apps Apps**  >  **downloaden** in het Microsoft 365-beheercentrum om invoegvoegingen te implementeren.</span><span class="sxs-lookup"><span data-stu-id="6940a-110">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="6940a-111">Opmerkingen:</span><span class="sxs-lookup"><span data-stu-id="6940a-111">Notes:</span></span> 

- <span data-ttu-id="6940a-112">Geïntegreerde apps vereist dat de beheerder globale beheerders- of Exchange beheerdersmachtigingen heeft.</span><span class="sxs-lookup"><span data-stu-id="6940a-112">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="6940a-113">Bij het implementeren van invoegvoegingen voor meerdere gebruikers is het raadzaam om opdrachten te maken met behulp van groepen in plaats van afzonderlijke gebruikers.</span><span class="sxs-lookup"><span data-stu-id="6940a-113">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="6940a-114">Zie Overwegingen bij het toewijzen van een [invoegvoeging aan gebruikers en groepen](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="6940a-114">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="6940a-115">Gecentraliseerde implementatie biedt geen ondersteuning voor gebruikers in geneste groepen of groepen met bovenliggende groepen.</span><span class="sxs-lookup"><span data-stu-id="6940a-115">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="6940a-116">Zie Gebruikers- en [groepstoewijzingen voor meer informatie.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="6940a-116">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="6940a-117">Zorg ervoor dat de Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is ingeschakeld voor gebruikers om zich aan te melden.</span><span class="sxs-lookup"><span data-stu-id="6940a-117">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="6940a-118">Zie App-eigenschappen [configureren voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="6940a-118">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="6940a-119">Als u problemen hebt met het implementeren van invoegvoegingen met behulp van geïntegreerde apps, kunt u deze implementeren met behulp van [invoegvoegingen.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="6940a-119">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="6940a-120">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="6940a-120">For more information, see:</span></span>

<span data-ttu-id="6940a-121">[Invoegvoegingen implementeren in het beheercentrum](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Invoegvoegingen beheren in het beheercentrum](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [De PowerShell-cmdlets voor](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) gecentraliseerde implementatie gebruiken om invoegingen te beheren 
 Invoeg Office via gecentraliseerde implementatie publiceren [via het Microsoft 365 beheercentrum](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Probleem oplossen: Gebruiker ziet geen invoegvoegingen](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Gebruikersfouten oplossen met Office-invoegingen](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="6940a-121">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>