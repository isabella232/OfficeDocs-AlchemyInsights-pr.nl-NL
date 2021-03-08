---
title: E-mailberichten in uw organisatie zoeken en verwijderen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523692"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="569ce-102">E-mailberichten in uw organisatie zoeken en verwijderen</span><span class="sxs-lookup"><span data-stu-id="569ce-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="569ce-103">Ga als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="569ce-103">Follow these steps:</span></span>

1. <span data-ttu-id="569ce-104">Als u geen globale beheerder bent, moet u voor het zoeken naar berichten uw account toevoegen aan de **rollengroep eDiscovery Manager** of de rol **compliancezoekbeheer.**</span><span class="sxs-lookup"><span data-stu-id="569ce-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="569ce-105">Als u berichten wilt verwijderen, moet u lid worden van de rollengroep **Organisatiebeheer** of de rol Zoeken **en wissen.**</span><span class="sxs-lookup"><span data-stu-id="569ce-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="569ce-106">Machtigingen voor deze rollen worden toegewezen in het [beveiligings- & compliancecentrum.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="569ce-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="569ce-107">[Maak een inhoudszoekactie](https://docs.microsoft.com/office365/securitycompliance/content-search) om te zoeken naar het bericht dat u wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="569ce-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="569ce-108">[Maak verbinding met beveiligings & Compliancecentrum PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="569ce-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="569ce-109">Als u MFA gebruikt, bekijkt u deze instructies: Verbinding maken met & [Compliancecentrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) met behulp van meervoudige verificatie</span><span class="sxs-lookup"><span data-stu-id="569ce-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="569ce-110">Het bericht verwijderen: voer de `New-ComplianceSearchAction` cmdlet uit om het bericht te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="569ce-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="569ce-111">Verwijderde berichten worden verplaatst naar de map Herstelbare items van een gebruiker.</span><span class="sxs-lookup"><span data-stu-id="569ce-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="569ce-112">Zie stap [3: Het bericht](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization) verwijderen voor een voorbeeldopdracht.</span><span class="sxs-lookup"><span data-stu-id="569ce-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
