---
title: E-mailberichten automatisch verplaatsen naar het archiefpostvak
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744547"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="788d3-102">E-mailberichten automatisch verplaatsen naar het archiefpostvak</span><span class="sxs-lookup"><span data-stu-id="788d3-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="788d3-103">U kunt als volgende een beleid instellen om het oude e-mailbericht van een gebruiker automatisch naar het archiefpostvak te verplaatsen:</span><span class="sxs-lookup"><span data-stu-id="788d3-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="788d3-104">Ga naar [**Beveiligingsbeheer &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **compliancegegevensbeheerarchief** om te controleren of een  >   archiefpostvak is ingeschakeld voor de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="788d3-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="788d3-105">Als dat niet het beste  is, klikt u **in het** waarschuwingsvak op Inschakelen en ja.</span><span class="sxs-lookup"><span data-stu-id="788d3-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="788d3-106">Ga naar [**Exchange-beheercentrum > compliancebeheer > bewaarlabels.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="788d3-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="788d3-107">Kies het pictogram + en kies **vervolgens automatisch toepassen op het hele postvak.**</span><span class="sxs-lookup"><span data-stu-id="788d3-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="788d3-108">Wijs een naam toe aan de bewaarlabel en kies **Verplaatsen naar archief.**</span><span class="sxs-lookup"><span data-stu-id="788d3-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="788d3-109">Voer voor de bewaarperiode de beste tijd in, bijvoorbeeld 90 dagen.</span><span class="sxs-lookup"><span data-stu-id="788d3-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="788d3-110">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="788d3-110">Click **Save**.</span></span>
5. <span data-ttu-id="788d3-111">Maak nu een bewaarbeleid: kies **bewaarbeleid** en kies het pictogram om een nieuw beleid toe te voegen.</span><span class="sxs-lookup"><span data-stu-id="788d3-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="788d3-112">Wijs een naam toe aan het bewaarbeleid en klik en schuif om de bewaartag te zoeken en toe te voegen die u zojuist hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="788d3-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="788d3-113">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="788d3-113">Click **Save**.</span></span>
7. <span data-ttu-id="788d3-114">Pas ten slotte het bewaarbeleid toe op het postvak van de gebruiker: ga nog steeds in het Exchange-beheercentrum naar postvakken **van**  >  **geadresseerden.**</span><span class="sxs-lookup"><span data-stu-id="788d3-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="788d3-115">Kies alle gebruikers op wie u het beleid wilt toepassen en kies vervolgens **Bewerken** (het potloodpictogram).</span><span class="sxs-lookup"><span data-stu-id="788d3-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="788d3-116">Klik in het dialoogvenster op **postvakfuncties.**</span><span class="sxs-lookup"><span data-stu-id="788d3-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="788d3-117">Pas **onder Bewaarbeleid** het beleid toe dat u zojuist hebt gemaakt > **Opslaan.**</span><span class="sxs-lookup"><span data-stu-id="788d3-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="788d3-118">Zie Een bewaarbeleid toepassen op postvakken voor instructies voor het toepassen van het beleid [op alle gebruikers.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="788d3-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
