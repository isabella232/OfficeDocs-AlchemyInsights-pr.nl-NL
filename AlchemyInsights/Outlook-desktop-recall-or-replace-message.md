---
title: Outlook Desktop intrekken of vervangen van een e-mailbericht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496106"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="ce1a5-102">Intrekken of vervangen van een e-mailbericht van Outlook</span><span class="sxs-lookup"><span data-stu-id="ce1a5-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="ce1a5-103">Als de beheerder kunt u **berichten intrekken voor gebruikers met PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="ce1a5-104">U kunt berichten van de admin center kan niet intrekken.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="ce1a5-105">U kunt **alleen berichten intrekken die zijn verzonden naar personen in uw organisatie**.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="ce1a5-106">Als het bericht is verzonden naar een Gmail-adres, bijvoorbeeld, kan niet u deze intrekken.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="ce1a5-107">U kunt **alleen berichten intrekken verzonden vanuit Outlook 2016 op de PC**.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="ce1a5-108">Als een gebruiker een bericht met behulp van Outlook voor Mac of Outlook op het web verzendt, kunt u deze niet meer intrekken.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="ce1a5-109">Intrekken of vervangen van een e-mailbericht:</span><span class="sxs-lookup"><span data-stu-id="ce1a5-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="ce1a5-110">In het deelvenster mappen aan de linkerzijde van het Outlook-venster, selecteert u de map Verzonden Items.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="ce1a5-111">Dubbelklik op het bericht dat u wilt intrekken om deze te openen.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="ce1a5-112">Klik op het tabblad **bericht** en selecteer vervolgens **Acties** > **Dit bericht intrekken**.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="ce1a5-113">Selecteer **Ongelezen kopieën van dit bericht verwijderen** of **Ongelezen kopieën verwijderen en vervangen door een nieuw bericht**en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="ce1a5-114">Als u een vervangend bericht verzendt het bericht opstelt, en selecteer vervolgens **verzenden**.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="ce1a5-115">Het slagen of mislukken van een bericht intrekken is afhankelijk van de instellingen van de ontvanger in Outlook.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="ce1a5-116">Raadpleeg [dit artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)om te controleren op het intrekken.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="ce1a5-117">Zoeken en verwijderen van e-mailberichten in uw organisatie</span><span class="sxs-lookup"><span data-stu-id="ce1a5-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="ce1a5-118">Als u niet een globale beheerder bent, moet uw account worden toegevoegd aan de eDiscovery managerrol of de rol van conformiteit zoeken om te zoeken naar berichten.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="ce1a5-119">Om berichten te verwijderen, moet u deel te nemen aan de rolgroep Management van de organisatie of de rol zoeken en verwijderen.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="ce1a5-120">Machtigingen voor deze rollen zijn toegewezen in het [midden van beveiliging en naleving](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="ce1a5-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="ce1a5-121">[Maken een inhoud zoeken](https://docs.microsoft.com/office365/securitycompliance/content-search) om te zoeken naar het bericht te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="ce1a5-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="ce1a5-122">[Verbinding maken met de veiligheid en conformiteit PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ce1a5-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="ce1a5-123">Als u een meerledige verificatie gebruikt, Zie [verbinding maken met Office 365-beveiliging en naleving Center PowerShell meerledige verificatie](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="ce1a5-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>