---
title: Kan niet aanmelden bij Teams vanwege fout autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931903"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="9c891-102">Kan niet aanmelden bij Teams vanwege fout autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="9c891-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="9c891-103">Als naadloze SSO is ingeschakeld als O365-verificatie, moet de URL 'autologon.microsoftazuread-sso.com ' mogelijk worden toegevoegd aan intranet sites.</span><span class="sxs-lookup"><span data-stu-id="9c891-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="9c891-104">Als deze eerder is toegevoegd aan vertrouwde websites en naadloze SSO wordt gebruikt, moet deze worden verwijderd uit vertrouwde sites.</span><span class="sxs-lookup"><span data-stu-id="9c891-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="9c891-105">Bekijk de [Controlelijst voor probleemoplossing bij naadloze SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="9c891-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="9c891-106">Voer de volgende stappen uit om een URL toe te voegen aan de lijst met intranet sites:</span><span class="sxs-lookup"><span data-stu-id="9c891-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="9c891-107">Open Internet Explorer door te klikken op de knop **Start**.</span><span class="sxs-lookup"><span data-stu-id="9c891-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="9c891-108">Typ in het zoekvak Internet Explorer en klik vervolgens in de lijst met resultaten op **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="9c891-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="9c891-109">Klik op het menu **Extra** en klik vervolgens op **Internetopties**.</span><span class="sxs-lookup"><span data-stu-id="9c891-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="9c891-110">Klik op het tabblad **Beveiliging**.</span><span class="sxs-lookup"><span data-stu-id="9c891-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="9c891-111">Klik nu op **Lokale intranet sites** en klik vervolgens op de knop **Sites** en vervolgens op **Geavanceerd**.</span><span class="sxs-lookup"><span data-stu-id="9c891-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="9c891-112">Voer de URL van de website in en klik op **Toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="9c891-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="9c891-113">Als u gereed bent, klikt u op **Sluiten**.</span><span class="sxs-lookup"><span data-stu-id="9c891-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="9c891-114">Zie voor meer informatie [Documentatie voor het implementeren van de naadloze SSO voor O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (dit omvat een op beleid gebaseerd proces voor het toevoegen van een URL aan intranet sites in Stap 3).</span><span class="sxs-lookup"><span data-stu-id="9c891-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
