---
title: Fout in Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786664"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="078f2-102">4c7-fout in Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="078f2-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="078f2-103">Deze fout treedt op omdat Voor Microsoft Teams Forms-verificatie is vereist.</span><span class="sxs-lookup"><span data-stu-id="078f2-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="078f2-104">Wanneer u Active Directory Federation Services (AD FS) implementeert, is Forms Authentication standaard niet ingeschakeld voor het intranet.</span><span class="sxs-lookup"><span data-stu-id="078f2-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="078f2-105">Als Windows Integrated Authentication mislukt, wordt u gevraagd u aan te melden met Forms Authentication.</span><span class="sxs-lookup"><span data-stu-id="078f2-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="078f2-106">Als u dit probleem wilt oplossen, schakelt u Forms Authentication in met behulp van de MMC-module (AD FS Microsoft Management Console) op de computer met de lokale kopie van Active Directory.</span><span class="sxs-lookup"><span data-stu-id="078f2-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="078f2-107">Ga hiervoor als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="078f2-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="078f2-108">Blader in het navigatiedeelvenster naar **Verificatiebeleid.**</span><span class="sxs-lookup"><span data-stu-id="078f2-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="078f2-109">Selecteer **onder Acties** in het detailvenster de optie Globale primaire verificatie **bewerken.**</span><span class="sxs-lookup"><span data-stu-id="078f2-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="078f2-110">Selecteer op **het tabblad Intranet** de optie **Formulierenverificatie**.</span><span class="sxs-lookup"><span data-stu-id="078f2-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="078f2-111">Selecteer **OK** (of **Toepassen).**</span><span class="sxs-lookup"><span data-stu-id="078f2-111">Select **OK** (or **Apply**).</span></span>