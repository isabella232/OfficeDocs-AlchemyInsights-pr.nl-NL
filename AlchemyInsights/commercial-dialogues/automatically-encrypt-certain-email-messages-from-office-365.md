---
title: Bepaalde e-mailberichten automatisch versleutelen vanuit Office 365
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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744586"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="10521-102">Bepaalde e-mailberichten automatisch versleutelen vanuit Office 365</span><span class="sxs-lookup"><span data-stu-id="10521-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="10521-103">Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **de optie e-mailstroom > regels.**</span><span class="sxs-lookup"><span data-stu-id="10521-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="10521-104">Klik op **het pictogram Nieuw (+)** en klik vervolgens op **Office 365-berichtversleuteling en rechtenbescherming toepassen op berichten.**</span><span class="sxs-lookup"><span data-stu-id="10521-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="10521-105">Voer **in Naam** een naam in voor de regel, zoals Alle berichten *versleutelen.*</span><span class="sxs-lookup"><span data-stu-id="10521-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="10521-106">Kies **in Deze regel toepassen als**, **[Toepassen op alle berichten]**.</span><span class="sxs-lookup"><span data-stu-id="10521-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="10521-107">Klik naast **het veld Het volgende** doen op Selecteer **een**.</span><span class="sxs-lookup"><span data-stu-id="10521-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="10521-108">Selecteer in **de vervolgkeuzelijst RMS-sjabloon** de optie **Versleutelen** en klik vervolgens op **OK.**</span><span class="sxs-lookup"><span data-stu-id="10521-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="10521-109">(Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat.</span><span class="sxs-lookup"><span data-stu-id="10521-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="10521-110">Maar u kunt het toevoegen!)</span><span class="sxs-lookup"><span data-stu-id="10521-110">But you can add it!)</span></span>
7. <span data-ttu-id="10521-111">Schakel het **selectievakje Deze regel controleren met ernstniveau** in en selecteer vervolgens het gewenste niveau.</span><span class="sxs-lookup"><span data-stu-id="10521-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="10521-112">Als uw bedrijf contractuele verplichtingen heeft om alle e-mailberichten versleuteld te verzenden, raad ik u aan het niveau in te stellen op **Hoog.**</span><span class="sxs-lookup"><span data-stu-id="10521-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="10521-113">Klik **onder Een model voor deze regel kiezen** op **Afdwingen.**</span><span class="sxs-lookup"><span data-stu-id="10521-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="10521-114">Kies een optionele selectie (in een lijst met optionele selecties die u op dit moment kunt maken, waarvan er veel kunnen worden overgelaten met de standaardinstelling voor eenvoud).</span><span class="sxs-lookup"><span data-stu-id="10521-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="10521-115">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="10521-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="10521-116">U kunt deze regel later altijd weer bewerken.</span><span class="sxs-lookup"><span data-stu-id="10521-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="10521-117">Zie Regels voor e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) voor meer informatie over het maken van regels voor versleuteling.</span><span class="sxs-lookup"><span data-stu-id="10521-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

