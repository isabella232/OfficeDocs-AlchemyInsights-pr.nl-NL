---
title: Een e-mailbericht intrekken of vervangen in de bureaubladversie van Outlook
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663985"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="d0758-102">Een e-mailbericht intrekken of vervangen in Outlook</span><span class="sxs-lookup"><span data-stu-id="d0758-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="d0758-103">Als beheerder kunt u **berichten intrekken namens gebruikers met behulp van PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="d0758-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="d0758-104">U kunt geen berichten intrekken vanuit het Beheercentrum.</span><span class="sxs-lookup"><span data-stu-id="d0758-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="d0758-105">U kunt **alleen berichten intrekken die zijn verzonden naar personen in uw organisatie**.</span><span class="sxs-lookup"><span data-stu-id="d0758-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="d0758-106">Als het bericht is verzonden naar een Gmail-adres, kunt u dit bijvoorbeeld niet intrekken.</span><span class="sxs-lookup"><span data-stu-id="d0758-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="d0758-107">U kunt **alleen berichten intrekken die vanuit Outlook 2016 op de PC zijn verzonden**.</span><span class="sxs-lookup"><span data-stu-id="d0758-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="d0758-108">Als een gebruiker een bericht verzendt met Outlook voor Mac of de webversie van Outlook, kunt u dit niet intrekken.</span><span class="sxs-lookup"><span data-stu-id="d0758-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="d0758-109">Een e-mailbericht intrekken of vervangen:</span><span class="sxs-lookup"><span data-stu-id="d0758-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="d0758-110">Selecteer in het deelvenster map aan de linkerkant van het Outlook-venster de map Verzonden items.</span><span class="sxs-lookup"><span data-stu-id="d0758-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="d0758-111">Dubbelklik op het bericht dat u wilt intrekken om het te openen.</span><span class="sxs-lookup"><span data-stu-id="d0758-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="d0758-112">Selecteer het tabblad **bericht** en selecteer vervolgens **actie**  >  **Dit bericht intrekken**.</span><span class="sxs-lookup"><span data-stu-id="d0758-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="d0758-113">Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht**en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="d0758-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="d0758-114">Als u een vervangend bericht verzendt, stelt u het bericht op en selecteert u vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="d0758-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="d0758-115">Het slagen of mislukken van het intrekken van een bericht is afhankelijk van de instellingen van de geadresseerde in Outlook.</span><span class="sxs-lookup"><span data-stu-id="d0758-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="d0758-116">Zie het [volgende artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)voor de stappen voor het intrekken van een bericht.</span><span class="sxs-lookup"><span data-stu-id="d0758-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="d0758-117">E-mailberichten in uw organisatie zoeken en verwijderen</span><span class="sxs-lookup"><span data-stu-id="d0758-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="d0758-118">Als u geen globale beheerder bent, moet uw account worden toegevoegd aan de rol van eDiscovery-beheerder of zoekbeheer voor compliance om te zoeken naar berichten.</span><span class="sxs-lookup"><span data-stu-id="d0758-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="d0758-119">Als u berichten wilt verwijderen, moet u lid worden van de rollen groep Organisatiebeheer of de rol zoeken en wissen.</span><span class="sxs-lookup"><span data-stu-id="d0758-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="d0758-120">Machtigingen voor deze rollen worden toegewezen in het [beveiligings-en compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="d0758-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="d0758-121">[Maak een zoekopdracht naar inhoud](https://docs.microsoft.com/microsoft-365/compliance/content-search) om te zoeken naar het bericht dat u wilt verwijderen.</span><span class="sxs-lookup"><span data-stu-id="d0758-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="d0758-122">[Maak verbinding met het beveiligings-en compliance-centrum PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d0758-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="d0758-123">Als u multi-factor Authentication gebruikt, raadpleegt u [verbinding maken met de PowerShell-beveiliging en compliance van Microsoft 365 via meervoudige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="d0758-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>