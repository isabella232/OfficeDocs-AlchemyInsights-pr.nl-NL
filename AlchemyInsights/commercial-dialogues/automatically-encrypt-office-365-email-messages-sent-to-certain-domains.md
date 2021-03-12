---
title: Office 365-e-mailberichten die naar bepaalde domeinen worden verzonden, automatisch versleutelen
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744550"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="61959-102">Office 365-e-mailberichten die naar bepaalde domeinen worden verzonden, automatisch versleutelen</span><span class="sxs-lookup"><span data-stu-id="61959-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="61959-103">Kies in [het Exchange-beheercentrum](https://outlook.office365.com/ecp/) **de optie e-mailstroom > regels.**</span><span class="sxs-lookup"><span data-stu-id="61959-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="61959-104">Klik op **het pictogram Nieuw (+)** en klik vervolgens op **Office 365-berichtversleuteling en rechtenbescherming toepassen op berichten.**</span><span class="sxs-lookup"><span data-stu-id="61959-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="61959-105">Voer **in Naam** een naam in voor de regel, zoals Berichten versleutelen die naar *contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="61959-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="61959-106">Kies **in Deze regel toepassen als**, de optie De ontvanger > domein **is**.</span><span class="sxs-lookup"><span data-stu-id="61959-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="61959-107">Voer de naam van het domein in, zoals **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="61959-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="61959-108">Klik op **het pictogram Toevoegen (+)** en klik vervolgens op **OK.**</span><span class="sxs-lookup"><span data-stu-id="61959-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="61959-109">Klik naast **het veld Het volgende** doen op Selecteer **een**.</span><span class="sxs-lookup"><span data-stu-id="61959-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="61959-110">Selecteer in **de vervolgkeuzelijst RMS-sjabloon** de optie **Versleutelen** en klik vervolgens op **OK.**</span><span class="sxs-lookup"><span data-stu-id="61959-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="61959-111">(Als u deze optie niet ziet, betekent dit dat uw abonnement geen automatische versleuteling bevat.</span><span class="sxs-lookup"><span data-stu-id="61959-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="61959-112">Maar u kunt het toevoegen!)</span><span class="sxs-lookup"><span data-stu-id="61959-112">But you can add it!)</span></span>
9. <span data-ttu-id="61959-113">Kies een optionele selectie (in een lijst met optionele selecties die u op dit moment kunt maken, waarvan er veel kunnen worden overgelaten met de standaardinstelling voor eenvoud).</span><span class="sxs-lookup"><span data-stu-id="61959-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="61959-114">Klik op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="61959-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="61959-115">U kunt deze regel later altijd weer bewerken.</span><span class="sxs-lookup"><span data-stu-id="61959-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="61959-116">Zie Regels voor e-mailstroom definiëren om e-mailberichten te versleutelen [in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) voor meer informatie over het maken van regels voor versleuteling.</span><span class="sxs-lookup"><span data-stu-id="61959-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>