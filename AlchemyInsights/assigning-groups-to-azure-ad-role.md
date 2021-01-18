---
title: Groepen toewijzen aan de functie Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884913"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="7db20-102">Groepen toewijzen aan de functie Azure AD</span><span class="sxs-lookup"><span data-stu-id="7db20-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="7db20-103">Voer de volgende stappen uit om een Azure AD-groep met bron autoriteit in azure AD toe te wijzen aan een Azure AD-rol:</span><span class="sxs-lookup"><span data-stu-id="7db20-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="7db20-104">Maak een nieuwe groep om een nieuwe groep te maken:</span><span class="sxs-lookup"><span data-stu-id="7db20-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="7db20-105">a.</span><span class="sxs-lookup"><span data-stu-id="7db20-105">a.</span></span> <span data-ttu-id="7db20-106">Meld u aan bij het Azure AD-Beheercentrum met bevoegdheden voor de **beheerder** of **globale beheerders** machtigingen.</span><span class="sxs-lookup"><span data-stu-id="7db20-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="7db20-107">b.</span><span class="sxs-lookup"><span data-stu-id="7db20-107">b.</span></span> <span data-ttu-id="7db20-108">Selecteer **Azure Active Directory-> groepen > alle groepen > nieuwe groep**.</span><span class="sxs-lookup"><span data-stu-id="7db20-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="7db20-109">c.</span><span class="sxs-lookup"><span data-stu-id="7db20-109">c.</span></span> <span data-ttu-id="7db20-110">Maak de groep.</span><span class="sxs-lookup"><span data-stu-id="7db20-110">Create the group.</span></span>

2. <span data-ttu-id="7db20-111">Wijs tijdens het maken van groepen een rol toe aan de groep of nadat de groep is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="7db20-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="7db20-112">a.</span><span class="sxs-lookup"><span data-stu-id="7db20-112">a.</span></span> <span data-ttu-id="7db20-113">Als u tijdens het maken van een groep een rol wilt toewijzen aan de groep, kunt u overstappen op de wisselknop **Azure AD** en de groep maken.</span><span class="sxs-lookup"><span data-stu-id="7db20-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="7db20-114">b.</span><span class="sxs-lookup"><span data-stu-id="7db20-114">b.</span></span> <span data-ttu-id="7db20-115">Als u een rol aan de groep wilt toewijzen nadat deze is gemaakt, gaat u naar het tabblad **toegewezen rollen** voor de nieuwe groep en wijst u de rol toe aan de groep.</span><span class="sxs-lookup"><span data-stu-id="7db20-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="7db20-116">**Lidmaatschap van een groep beheren die is toegewezen aan de rol van Azure AD**</span><span class="sxs-lookup"><span data-stu-id="7db20-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="7db20-117">Om de verhoging van bevoegdheden te voorkomen, kunnen standaard alleen geprivilegieerde beheerders en globale beheerders het lidmaatschap van een groep wijzigen die aan een rol is toegewezen.</span><span class="sxs-lookup"><span data-stu-id="7db20-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="7db20-118">Ze kunnen echter wel een eigenaar voor een dergelijke groep toewijzen en deze taak delegeren.</span><span class="sxs-lookup"><span data-stu-id="7db20-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="7db20-119">Zie voor meer informatie over het toewijzen van Cloud groepen aan Azure AD-rollen [een AD-rol toewijzen aan Cloud groep](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="7db20-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="7db20-120">Zie voor meer informatie over het oplossen van rollen die zijn toegewezen aan Cloud groepen, [problemen oplossen met rollen die zijn toegewezen aan Cloud groepen](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="7db20-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





