---
title: Een e-mailbericht intrekken of vervangen
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353501"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="7a34b-102">Een e-mailbericht intrekken of vervangen in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7a34b-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="7a34b-103">U kunt **alleen berichten intrekken die zijn verzonden naar personen in uw organisatie**.</span><span class="sxs-lookup"><span data-stu-id="7a34b-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="7a34b-104">Als het bericht bijvoorbeeld naar een Gmail-adres is verzonden, kunt u dit niet intrekken.</span><span class="sxs-lookup"><span data-stu-id="7a34b-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="7a34b-105">U kunt **alleen berichten intrekken die vanuit Outlook voor de PC zijn verzonden**.</span><span class="sxs-lookup"><span data-stu-id="7a34b-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="7a34b-106">Als een gebruiker een bericht verzendt met Outlook voor Mac of de webversie van Outlook, kunt u dit niet intrekken.</span><span class="sxs-lookup"><span data-stu-id="7a34b-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="7a34b-107">Als tenantbeheerder kunt u **berichten intrekken namens gebruikers met behulp van PowerShell** (Zie [e-mailberichten zoeken en verwijderen](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)voor meer informatie.)</span><span class="sxs-lookup"><span data-stu-id="7a34b-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="7a34b-108">U kunt geen berichten intrekken vanuit het Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="7a34b-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="7a34b-109">Schuif omlaag naar e-mailberichten in uw organisatie zoeken en verwijderen voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7a34b-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="7a34b-110">**Een verzonden e-mailbericht intrekken of vervangen**</span><span class="sxs-lookup"><span data-stu-id="7a34b-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="7a34b-111">Kies in het mappenvenster links van het Outlook-venster de map Verzonden items.</span><span class="sxs-lookup"><span data-stu-id="7a34b-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="7a34b-112">Open het bericht dat u wilt intrekken.</span><span class="sxs-lookup"><span data-stu-id="7a34b-112">Open the message that you want to recall.</span></span> <span data-ttu-id="7a34b-113">U dubbelklikt op het bericht om het te openen.</span><span class="sxs-lookup"><span data-stu-id="7a34b-113">You must double-click to open the message.</span></span> <span data-ttu-id="7a34b-114">Als u het bericht selecteert zodat het in het leesvenster wordt weergegeven, kunt u het bericht niet meer intrekken.</span><span class="sxs-lookup"><span data-stu-id="7a34b-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="7a34b-115">Selecteer op het tabblad bericht de optie **acties**  >  **Dit bericht intrekken**.</span><span class="sxs-lookup"><span data-stu-id="7a34b-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="7a34b-116">Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht** en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="7a34b-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="7a34b-117">Als u een vervangend bericht verzendt, stelt u het bericht op en selecteert u vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="7a34b-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="7a34b-118">Het slagen of mislukken van het intrekken van een bericht is afhankelijk van de instellingen van de ontvangers in Outlook.</span><span class="sxs-lookup"><span data-stu-id="7a34b-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="7a34b-119">Zie [een verzonden e-mailbericht intrekken of vervangen](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)voor meer informatie, waaronder het intrekken van een bericht.</span><span class="sxs-lookup"><span data-stu-id="7a34b-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="7a34b-120">Als u **_e-mailberichten in uw organisatie wilt zoeken en verwijderen_**, kunt u dit het beste doen als u een globale beheerder bent. Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rollen groep van de eDiscovery-beheerder of aan de rol zoekbeheer voor naleving.</span><span class="sxs-lookup"><span data-stu-id="7a34b-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="7a34b-121">Als u berichten wilt verwijderen, moet u lid worden van de rollen groep Organisatiebeheer of de rol zoeken en wissen.</span><span class="sxs-lookup"><span data-stu-id="7a34b-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="7a34b-122">Machtigingen voor deze rollen worden toegewezen in de [beveiligings & nalevings centrum](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="7a34b-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="7a34b-123">[Maak een zoekopdracht naar inhoud](https://docs.microsoft.com/microsoft-365/compliance/content-search) om te zoeken naar het bericht dat u wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="7a34b-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="7a34b-124">[Maak verbinding met beveiliging & nalevings centrum voor PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="7a34b-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="7a34b-125">Zie [verbinding maken met Microsoft 365-beveiliging & nalevings centrum voor PowerShell via meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)als u MFA gebruikt (multi-factor Authentication).</span><span class="sxs-lookup"><span data-stu-id="7a34b-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
