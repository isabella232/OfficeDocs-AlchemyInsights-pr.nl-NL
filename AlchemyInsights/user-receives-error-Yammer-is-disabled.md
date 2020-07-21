---
title: Gebruiker ontvangt fout AADSTS7000112 Yammer is uitgeschakeld
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197873"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="d99f9-102">Gebruiker ontvangt fout AADSTS7000112 Yammer is uitgeschakeld</span><span class="sxs-lookup"><span data-stu-id="d99f9-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="d99f9-103">Als u de foutmelding "AADSTS7000112: Application '00000005-0000-0ff1-ce00-00000000000000'(Yammer) ontvangt, is er een probleem met de servicehoofdpaal binnen Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d99f9-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="d99f9-104">Een beheerder heeft mogelijk de servicehoofdsom uitgeschakeld om de toegang tot Yammer te blokkeren.</span><span class="sxs-lookup"><span data-stu-id="d99f9-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="d99f9-105">Het uitschakelen van de service principal wordt niet aanbevolen en kan extra problemen veroorzaken.</span><span class="sxs-lookup"><span data-stu-id="d99f9-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="d99f9-106">Zie [Yammer-toegang uitschakelen voor Microsoft 365-gebruikers voor](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)meer informatie over de ondersteunde aanpak om de toegang van gebruikers tot Yammer te blokkeren.</span><span class="sxs-lookup"><span data-stu-id="d99f9-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="d99f9-107">Ga als volgt te werk om dit probleem in de Azure Portal te verhelpen en de gebruikerstoegang tot Yammer te herstellen:</span><span class="sxs-lookup"><span data-stu-id="d99f9-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="d99f9-108">Open de Azure Active Directory-pagina en selecteer **Enterprise-toepassingen** onder **Beheren** in het linkernavigatiedeelvenster.</span><span class="sxs-lookup"><span data-stu-id="d99f9-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="d99f9-109">Typ **Office 365 Yammer** in het zoekvak en selecteer de naam van de toepassing om instellingen te openen.</span><span class="sxs-lookup"><span data-stu-id="d99f9-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="d99f9-110">Selecteer **Eigenschappen** onder **Beheren** in het linkernavigatiedeelvenster.</span><span class="sxs-lookup"><span data-stu-id="d99f9-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="d99f9-111">De waarde instellen van Ingeschakeld voor gebruikers **Yes**om zich aan **Save** **te melden?**</span><span class="sxs-lookup"><span data-stu-id="d99f9-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="d99f9-112">Meld u opnieuw aan bij Yammer.</span><span class="sxs-lookup"><span data-stu-id="d99f9-112">Sign in to Yammer again.</span></span> <span data-ttu-id="d99f9-113">Het kan nodig zijn om cookies te wissen.</span><span class="sxs-lookup"><span data-stu-id="d99f9-113">You might need to clear cookies.</span></span>

<span data-ttu-id="d99f9-114">U ook PowerShell-opdrachten uitvoeren om de waarde in te stellen.</span><span class="sxs-lookup"><span data-stu-id="d99f9-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="d99f9-115">Zie [de fout 'Sorry, maar we hebben problemen met aanmelden' als u op de Yammer-tegel klikt in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d99f9-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 