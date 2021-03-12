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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744715"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="8a54a-102">E-mailberichten in uw organisatie zoeken en verwijderen</span><span class="sxs-lookup"><span data-stu-id="8a54a-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="8a54a-103">Ga als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="8a54a-103">Follow these steps:</span></span>

1. <span data-ttu-id="8a54a-104">Als u geen globale beheerder bent, moet u als u wilt zoeken naar berichten uw account worden toegevoegd aan de rollengroep **eDiscovery Manager** of **compliancezoekbeheerrol.**</span><span class="sxs-lookup"><span data-stu-id="8a54a-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="8a54a-105">Als u berichten wilt verwijderen, moet u lid worden van de rollengroep **Organisatiebeheer** of de rol **zoeken en verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="8a54a-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="8a54a-106">Machtigingen voor deze rollen worden toegewezen in het [beveiligings- & compliancecentrum.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="8a54a-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="8a54a-107">[Maak een inhoudszoekactie](https://docs.microsoft.com/office365/securitycompliance/content-search) om het bericht te vinden dat u wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8a54a-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="8a54a-108">[Maak verbinding met & Compliance Center PowerShell.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="8a54a-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="8a54a-109">Als u MFA gebruikt, bekijkt u deze instructies: Verbinding maken met [& Compliance center PowerShell met meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="8a54a-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="8a54a-110">Het bericht verwijderen: voer de `New-ComplianceSearchAction` cmdlet uit om het bericht te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="8a54a-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="8a54a-111">Verwijderde berichten worden verplaatst naar de map Herstelbare items van een gebruiker.</span><span class="sxs-lookup"><span data-stu-id="8a54a-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="8a54a-112">Zie Stap [3: Het bericht verwijderen](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization) voor een voorbeeldopdracht.</span><span class="sxs-lookup"><span data-stu-id="8a54a-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
