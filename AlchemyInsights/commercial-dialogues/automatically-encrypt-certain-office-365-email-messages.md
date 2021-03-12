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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744583"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="d46fb-102">Bepaalde Office 365-e-mailberichten automatisch versleutelen</span><span class="sxs-lookup"><span data-stu-id="d46fb-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="d46fb-103">U kunt berichten die gebruikers naar bepaalde externe personen of organisaties verzenden, automatisch versleutelen.</span><span class="sxs-lookup"><span data-stu-id="d46fb-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="d46fb-104">Voer hiervoor de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="d46fb-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="d46fb-105">Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **de optie e-mailstroom > regels.**</span><span class="sxs-lookup"><span data-stu-id="d46fb-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="d46fb-106">Klik op **het pictogram Nieuw (+)** en klik vervolgens op **Office 365-berichtversleuteling en rechtenbescherming toepassen op berichten.**</span><span class="sxs-lookup"><span data-stu-id="d46fb-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="d46fb-107">Voer **in Naam** een naam in voor de regel, zoals Berichten *versleutelen die naar DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="d46fb-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="d46fb-108">Kies **in Deze regel toepassen als**, de > deze persoon **is.**</span><span class="sxs-lookup"><span data-stu-id="d46fb-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="d46fb-109">Selecteer in **het venster Leden** selecteren de naam van de persoon op wie u de versleutelingsregel wilt toepassen en klik op **Toevoegen.**</span><span class="sxs-lookup"><span data-stu-id="d46fb-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="d46fb-110">Wanneer u klaar bent met het toevoegen van gebruikers, klikt u op **OK.**</span><span class="sxs-lookup"><span data-stu-id="d46fb-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="d46fb-111">Klik naast **het veld Het volgende** doen op Selecteer **een**.</span><span class="sxs-lookup"><span data-stu-id="d46fb-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="d46fb-112">Selecteer in **de vervolgkeuzelijst RMS-sjabloon** de optie **Versleutelen** en klik vervolgens op **OK.**</span><span class="sxs-lookup"><span data-stu-id="d46fb-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="d46fb-113">(Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat.</span><span class="sxs-lookup"><span data-stu-id="d46fb-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="d46fb-114">Maar u kunt het toevoegen!)</span><span class="sxs-lookup"><span data-stu-id="d46fb-114">But you can add it!)</span></span>
9. <span data-ttu-id="d46fb-115">Kies een optionele selectie (in een lijst met optionele selecties die u op dit moment kunt maken, waarvan er veel kunnen worden overgelaten met de standaardinstelling voor eenvoud).</span><span class="sxs-lookup"><span data-stu-id="d46fb-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="d46fb-116">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="d46fb-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d46fb-117">U kunt deze regel later altijd weer bewerken.</span><span class="sxs-lookup"><span data-stu-id="d46fb-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="d46fb-118">Zie Regels voor e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)voor meer informatie over het maken van regels voor versleuteling.</span><span class="sxs-lookup"><span data-stu-id="d46fb-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

