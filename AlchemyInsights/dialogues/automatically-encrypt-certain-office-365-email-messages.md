---
title: Bepaalde Office 365-e-mailberichten automatisch versleutelen
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524901"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="5ded3-102">Bepaalde Office 365-e-mailberichten automatisch versleutelen</span><span class="sxs-lookup"><span data-stu-id="5ded3-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="5ded3-103">U kunt berichten die gebruikers naar bepaalde externe personen of organisaties verzenden, automatisch versleutelen.</span><span class="sxs-lookup"><span data-stu-id="5ded3-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="5ded3-104">Voer hiervoor de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="5ded3-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="5ded3-105">Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **e-mailstroom > regels.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="5ded3-106">Klik op **het pictogram Nieuw (+)** en klik vervolgens op Office 365-berichtversleuteling toepassen en bescherming tegen rechten **op berichten.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="5ded3-107">Voer **in** Naam een naam in voor de regel, zoals Berichten versleutelen *die naar de* DrToniRamos@gmail.com.</span><span class="sxs-lookup"><span data-stu-id="5ded3-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="5ded3-108">Kies **bij Deze regel toepassen de** optie > deze persoon **is.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="5ded3-109">Selecteer in **het venster Leden** selecteren de naam van de persoon op wie u de versleutelingsregel wilt toepassen en klik op **Toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="5ded3-110">Klik op OK als u klaar bent met het toevoegen van **gebruikers.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="5ded3-111">Klik naast het **veld Ga als volgt** te werk op Selecteer een **optie.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="5ded3-112">Selecteer **versleutelen** in de vervolgkeuzelijst van de RMS-sjabloon **en** klik op **OK.**</span><span class="sxs-lookup"><span data-stu-id="5ded3-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="5ded3-113">(Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat.</span><span class="sxs-lookup"><span data-stu-id="5ded3-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="5ded3-114">Maar u kunt het toevoegen!)</span><span class="sxs-lookup"><span data-stu-id="5ded3-114">But you can add it!)</span></span>
9. <span data-ttu-id="5ded3-115">Kies desgewenst een selectie (in een lijst met optionele selecties die u op dit punt kunt maken, waarvan er een groot aantal kan worden overgelaten met de standaardinstelling voor eenvoud).</span><span class="sxs-lookup"><span data-stu-id="5ded3-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="5ded3-116">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="5ded3-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5ded3-117">U kunt altijd teruggaan en deze regel later bewerken.</span><span class="sxs-lookup"><span data-stu-id="5ded3-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="5ded3-118">Zie Regels voor de e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)voor meer informatie over het maken van regels voor versleuteling.</span><span class="sxs-lookup"><span data-stu-id="5ded3-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

