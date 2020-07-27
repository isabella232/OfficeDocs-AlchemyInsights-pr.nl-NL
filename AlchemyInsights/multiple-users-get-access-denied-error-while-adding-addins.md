---
title: Meerdere gebruikers krijgen fout toegang geweigerd tijdens het toevoegen van invoegtoepassingen in Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423482"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="f8411-102">Meerdere gebruikers krijgen fout toegang geweigerd tijdens het toevoegen van invoegtoepassingen in Outlook</span><span class="sxs-lookup"><span data-stu-id="f8411-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="f8411-103">U opgeven welke beheerders in uw organisatie machtigingen hebben voor het installeren en beheren van invoegtoepassingen voor Outlook.</span><span class="sxs-lookup"><span data-stu-id="f8411-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="f8411-104">U ook opgeven welke gebruikers in uw organisatie toestemming hebben om invoegtoepassingen voor eigen gebruik te installeren en te beheren.</span><span class="sxs-lookup"><span data-stu-id="f8411-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="f8411-105">Zie De [beheerders en gebruikers opgeven die invoegtoepassingen voor Outlook kunnen installeren en beheren voor](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f8411-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="f8411-106">Als u wilt controleren of u machtigingen voor een gebruiker hebt toegewezen, vervangt u <Role Name> de naam van de functie om te verifiëren en voert u de volgende opdracht uit in Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f8411-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="f8411-107">Get-ManagementRoleAssignment -Rol " <Role Name> - GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="f8411-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="f8411-108">In dit voorbeeld ziet u hoe u controleert wie u machtigingen hebt toegewezen om invoegtoepassingen te installeren vanuit de Office Store voor de organisatie.</span><span class="sxs-lookup"><span data-stu-id="f8411-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="f8411-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="f8411-109">PowerShell</span></span>

<span data-ttu-id="f8411-110">-Rol "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="f8411-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="f8411-111">Bekijk in de resultaten Get-ManagementRoleAssignment de vermeldingen in de kolom Effectieve gebruikers.</span><span class="sxs-lookup"><span data-stu-id="f8411-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="f8411-112">Zie [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)voor gedetailleerde syntaxis en parametergegevens .</span><span class="sxs-lookup"><span data-stu-id="f8411-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 