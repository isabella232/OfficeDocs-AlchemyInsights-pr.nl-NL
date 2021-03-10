---
title: Verbindingsbeleid herstellen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/09/2021
ms.locfileid: "50693301"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="eb9c3-102">Verbindingsbeleid herstellen</span><span class="sxs-lookup"><span data-stu-id="eb9c3-102">Fix connection policy</span></span>

<span data-ttu-id="eb9c3-103">Het e-mailbericht is als veilig gemarkeerd en bezorgd in het Postvak IN van de gebruiker omdat het verzendende IP-adres als veilig is gemarkeerd in het verbindingsfilterbeleid.</span><span class="sxs-lookup"><span data-stu-id="eb9c3-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="eb9c3-104">Ga als volgt te werk om het beleid te controleren:</span><span class="sxs-lookup"><span data-stu-id="eb9c3-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="eb9c3-105">Ga naar het [Office 365-& compliancecentrum](https://go.microsoft.com/fwlink/p/?linkid=2077143)en ga naar Beleid voor bedreigingsbeheer  >    >  [antispam.](https://go.microsoft.com/fwlink/?linkid=2101518)</span><span class="sxs-lookup"><span data-stu-id="eb9c3-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="eb9c3-106">Selecteer op **het tabblad** Aangepast het **verbindingsfilterbeleid** en selecteer beleid **bewerken.**</span><span class="sxs-lookup"><span data-stu-id="eb9c3-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="eb9c3-107">Bekijk de lijst **met toegestane IP-adressen.**</span><span class="sxs-lookup"><span data-stu-id="eb9c3-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="eb9c3-108">Kijk of **De lijst** Veilig is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="eb9c3-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="eb9c3-109">Microsoft abonneert zich op bronnen van vertrouwde afzenders van derden.</span><span class="sxs-lookup"><span data-stu-id="eb9c3-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="eb9c3-110">Als **de lijst** Veilig is ingeschakeld, worden deze vertrouwde afzenders niet per ongeluk gemarkeerd als spam.</span><span class="sxs-lookup"><span data-stu-id="eb9c3-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="eb9c3-111">Het is raadzaam deze optie te selecteren, omdat hiermee het aantal fout-positieven (goede e-mail die als spam is geclassificeerd) wordt beperkt.</span><span class="sxs-lookup"><span data-stu-id="eb9c3-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
