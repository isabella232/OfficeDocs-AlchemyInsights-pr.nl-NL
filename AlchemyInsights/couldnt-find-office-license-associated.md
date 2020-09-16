---
title: Repareren van Microsoft 365-apps kan geen Office-licenties vinden die aan het bericht zijn gekoppeld
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747690"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="d2838-102">Bericht over het herstellen van Office-licenties die niet kunnen worden gevonden in Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="d2838-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="d2838-103">Als dit bericht wordt weergegeven, probeert u het volgende:</span><span class="sxs-lookup"><span data-stu-id="d2838-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d2838-104">Controleer uw firewall, antivirussoftware en proxy-instellingen om te controleren of de Internet toegang tot Microsoft 365-apps niet wordt geblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="d2838-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d2838-105">Zie [url's en IP-adresbereiken voor Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d2838-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="d2838-106">Verwijder de Office-licentie voor de desbetreffende gebruiker en [wijs deze opnieuw toe](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) .</span><span class="sxs-lookup"><span data-stu-id="d2838-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="d2838-107">Open een Office-app en meld u af [bij](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) bestaande gebruikersaccounts.</span><span class="sxs-lookup"><span data-stu-id="d2838-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="d2838-108">Ga naar Windows-instellingen **>**  >  **e-mail &** accounts en verwijder alle werk accounts, behalve het desbetreffende account.</span><span class="sxs-lookup"><span data-stu-id="d2838-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="d2838-109">Ga naar Windows-instellingen **Accounts**>  >  **toegang tot uw werk of school**voor accounts en Verbreek de verbinding met alle werk accounts, met uitzondering van het desbetreffende account.</span><span class="sxs-lookup"><span data-stu-id="d2838-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="d2838-110">Stel de activeringsstatus van Office opnieuw in.</span><span class="sxs-lookup"><span data-stu-id="d2838-110">Reset the Office activation state.</span></span> <span data-ttu-id="d2838-111">[Meer informatie](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="d2838-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="d2838-112">[Meld u aan](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) met het desbetreffende gebruikersaccount.</span><span class="sxs-lookup"><span data-stu-id="d2838-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="d2838-113">Zie [fouten met producten zonder licentie en activeringsfouten in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)voor aanvullende oplossingen voor het oplossen van problemen.</span><span class="sxs-lookup"><span data-stu-id="d2838-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>