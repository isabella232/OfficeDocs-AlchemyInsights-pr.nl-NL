---
title: Problemen met Yammer-licenties
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148237"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="2da1f-102">Problemen met Yammer-licenties</span><span class="sxs-lookup"><span data-stu-id="2da1f-102">Yammer licensing issues</span></span>

<span data-ttu-id="2da1f-103">Alle gebruikers moeten een licentie hebben om de Yammer Enterprise-service te gebruiken, maar standaard vereist Yammer niet dat gebruikers een licentie hebben om toegang te krijgen tot de service.</span><span class="sxs-lookup"><span data-stu-id="2da1f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="2da1f-104">Wanneer een beheerder de instelling wijzigt om Microsoft 365-gebruikers zonder Yammer-licenties te blokkeren, hebben gebruikers die geen Yammer Enterprise-licentie hebben toegewezen, geen toegang tot de Yammer-service.</span><span class="sxs-lookup"><span data-stu-id="2da1f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="2da1f-105">Zie [Yammer-gebruikerslicenties beheren in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) voor meer informatie</span><span class="sxs-lookup"><span data-stu-id="2da1f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="2da1f-106">Wanneer licenties van gebruikers worden verwijderd, wordt de Yammer-tegel niet meer weergegeven en kunnen andere services licentieverwijdering gebruiken om functies te verbergen.</span><span class="sxs-lookup"><span data-stu-id="2da1f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="2da1f-107">In andere gevallen kunnen functies nog steeds worden weergegeven, maar vereisen licentietoewijzing om te werken.</span><span class="sxs-lookup"><span data-stu-id="2da1f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="2da1f-108">**Licentie wordt niet bijgewerkt voor de gebruiker**</span><span class="sxs-lookup"><span data-stu-id="2da1f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="2da1f-109">Af en toe krijgt een gebruiker een licentie toegewezen, maar heeft hij nog steeds geen toegang tot Yammer.</span><span class="sxs-lookup"><span data-stu-id="2da1f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="2da1f-110">Vertragingen lopen vaker op wanneer er een massalicentietoewijzing aan de gang is.</span><span class="sxs-lookup"><span data-stu-id="2da1f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="2da1f-111">Yammer-gebruikers worden mogelijk niet in dezelfde volgorde bijgewerkt als licenties, worden gewijzigd in Azure AD omdat het systeem asynchroon wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="2da1f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="2da1f-112">Wacht tot 24 uur voordat u een ondersteuningscase opent om problemen met licentiesynchronisatie te melden.</span><span class="sxs-lookup"><span data-stu-id="2da1f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="2da1f-113">**Toewijzing van bulklicenties**</span><span class="sxs-lookup"><span data-stu-id="2da1f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="2da1f-114">Licenties kunnen worden toegewezen via het beheercentrum of PowerShell-scripting.</span><span class="sxs-lookup"><span data-stu-id="2da1f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="2da1f-115">Zie [Licenties toewijzen aan gebruikers](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) en [Licenties toewijzen aan gebruikersaccounts met Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2da1f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="2da1f-116">Microsoft Support biedt geen hulp bij het maken van scripts, maar documentatie over Yammer-licentietoewijzing is beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="2da1f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="2da1f-117">Zie [Yammer-licenties beheren met Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2da1f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>