---
title: Bepaalde e-mailberichten van Office 365 automatisch versleutelen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524913"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="c9a9e-102">Bepaalde e-mailberichten van Office 365 automatisch versleutelen</span><span class="sxs-lookup"><span data-stu-id="c9a9e-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="c9a9e-103">Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **e-mailstroom > regels.**</span><span class="sxs-lookup"><span data-stu-id="c9a9e-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c9a9e-104">Klik op **het pictogram Nieuw (+)** en klik vervolgens op Office 365-berichtversleuteling toepassen en bescherming tegen rechten **op berichten.**</span><span class="sxs-lookup"><span data-stu-id="c9a9e-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c9a9e-105">Voer **in** Naam een naam in voor de regel, zoals *Alle berichten versleutelen.*</span><span class="sxs-lookup"><span data-stu-id="c9a9e-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="c9a9e-106">Kies **bij Deze regel toepassen indien**, de optie **[Toepassen op alle berichten]**.</span><span class="sxs-lookup"><span data-stu-id="c9a9e-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="c9a9e-107">Klik naast het **veld Ga als volgt** te werk op Selecteer een **optie.**</span><span class="sxs-lookup"><span data-stu-id="c9a9e-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="c9a9e-108">Selecteer **versleutelen** in de vervolgkeuzelijst van de RMS-sjabloon **en** klik op **OK.**</span><span class="sxs-lookup"><span data-stu-id="c9a9e-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c9a9e-109">(Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat.</span><span class="sxs-lookup"><span data-stu-id="c9a9e-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c9a9e-110">Maar u kunt het toevoegen!)</span><span class="sxs-lookup"><span data-stu-id="c9a9e-110">But you can add it!)</span></span>
7. <span data-ttu-id="c9a9e-111">Schakel het **selectievakje Deze regel controleren met niveau van ernst** in en selecteer vervolgens het gewenste niveau.</span><span class="sxs-lookup"><span data-stu-id="c9a9e-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="c9a9e-112">Als uw bedrijf contractuele verplichtingen heeft om alle e-mailberichten versleuteld te verzenden, raden we u aan het niveau in te stellen op **Hoog.**</span><span class="sxs-lookup"><span data-stu-id="c9a9e-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="c9a9e-113">Klik **onder Een model kiezen voor deze regel** op **Afdwingen.**</span><span class="sxs-lookup"><span data-stu-id="c9a9e-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="c9a9e-114">Kies desgewenst een selectie (in een lijst met optionele selecties die u op dit punt kunt maken, waarvan er een groot aantal kan worden overgelaten met de standaardinstelling voor eenvoud).</span><span class="sxs-lookup"><span data-stu-id="c9a9e-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c9a9e-115">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="c9a9e-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c9a9e-116">U kunt altijd teruggaan en deze regel later bewerken.</span><span class="sxs-lookup"><span data-stu-id="c9a9e-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c9a9e-117">Zie Regels voor de e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) voor meer informatie over het maken van regels voor versleuteling.</span><span class="sxs-lookup"><span data-stu-id="c9a9e-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

