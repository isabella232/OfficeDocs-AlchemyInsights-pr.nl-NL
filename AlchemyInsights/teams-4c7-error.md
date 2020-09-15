---
title: 4c7 fout in teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700198"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="82343-102">4c7-fout in Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="82343-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="82343-103">Deze fout treedt op omdat Microsoft teams formulierverificatie vereist.</span><span class="sxs-lookup"><span data-stu-id="82343-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="82343-104">Wanneer u Active Directory Federation Services (AD FS) implementeert, wordt formulierverificatie niet standaard ingeschakeld voor het intranet.</span><span class="sxs-lookup"><span data-stu-id="82343-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="82343-105">Als Windows Integrated Authentication mislukt, wordt u gevraagd u aan te melden met behulp van formulierverificatie.</span><span class="sxs-lookup"><span data-stu-id="82343-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="82343-106">U kunt dit probleem oplossen door formulierverificatie in te schakelen via de MMC (Microsoft Management Console) van de Microsoft Management Console op de computer met de lokale kopie van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="82343-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="82343-107">Ga hiervoor als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="82343-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="82343-108">Blader in het navigatiedeelvenster naar **verificatiebeleid**.</span><span class="sxs-lookup"><span data-stu-id="82343-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="82343-109">Selecteer onder **acties** in het detailvenster de optie **globale primaire verificatie bewerken**.</span><span class="sxs-lookup"><span data-stu-id="82343-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="82343-110">Selecteer op het tabblad **intranet** de optie **formulierverificatie**.</span><span class="sxs-lookup"><span data-stu-id="82343-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="82343-111">Selecteer **OK** (of **toepassen**).</span><span class="sxs-lookup"><span data-stu-id="82343-111">Select **OK** (or **Apply**).</span></span>