---
title: Fout teams 4c 7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796056"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="d9c36-102">4c 7 fout in Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="d9c36-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="d9c36-103">Deze fout treedt op omdat Microsoft teams Forms-verificatie vereist.</span><span class="sxs-lookup"><span data-stu-id="d9c36-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="d9c36-104">Wanneer u Active Directory Federation Services (AD FS) implementeert, is Forms-verificatie niet standaard ingeschakeld voor het intranet.</span><span class="sxs-lookup"><span data-stu-id="d9c36-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="d9c36-105">Als geïntegreerde Windows-verificatie mislukt, wordt u gevraagd u aan te melden met behulp van Forms-verificatie.</span><span class="sxs-lookup"><span data-stu-id="d9c36-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="d9c36-106">Dit probleem oplossen door Forms-verificatie inschakelen met behulp van de AD FS-module van Microsoft Management Console (MMC) op de computer met de lokale kopie van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d9c36-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="d9c36-107">Volg deze stappen om dit te doen:</span><span class="sxs-lookup"><span data-stu-id="d9c36-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="d9c36-108">Blader in het navigatiedeelvenster naar **verificatiebeleid**.</span><span class="sxs-lookup"><span data-stu-id="d9c36-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="d9c36-109">Onder **acties** in het detailvenster, selecteer **globale primaire verificatie bewerken**.</span><span class="sxs-lookup"><span data-stu-id="d9c36-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="d9c36-110">Selecteer op het tabblad **intranet** **Forms-verificatie**.</span><span class="sxs-lookup"><span data-stu-id="d9c36-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="d9c36-111">Selecteer **OK** (of **toepassen**).</span><span class="sxs-lookup"><span data-stu-id="d9c36-111">Select **OK** (or **Apply**).</span></span>