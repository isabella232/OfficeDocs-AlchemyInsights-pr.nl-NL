---
title: Het uitschakelen van externe groepen
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540896"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="dee3b-102">Het uitschakelen van externe groepen</span><span class="sxs-lookup"><span data-stu-id="dee3b-102">How to disable External Groups</span></span>

<span data-ttu-id="dee3b-103">Yammer externe messaging toepassing Exchange transportregels (ETRs), een reeks proactieve besturingselementen om te voorkomen dat de gegevens van het bedrijf worden gedeeld.</span><span class="sxs-lookup"><span data-stu-id="dee3b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="dee3b-104">Om te voorkomen dat gebruikers kunnen maken van externe groepen, moet u een regel voor Exchange transport (ETR) configureren en vervolgens configureren Yammer de Exchange Transport als regel wilt gebruiken voor het blokkeren van externe berichten.</span><span class="sxs-lookup"><span data-stu-id="dee3b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="dee3b-105">Als u een regel hebt gemaakt in Exchange Online admin center, volgt ETR toe te passen in Yammer instellen:</span><span class="sxs-lookup"><span data-stu-id="dee3b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="dee3b-106">Aanmelden bij Yammer als een gecontroleerde admin en in de **Yammer admin center**, gaat u naar de C **inhoud en beveiliging van \> beveiligingsinstellingen.**</span><span class="sxs-lookup"><span data-stu-id="dee3b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="dee3b-107">Selecteer onder **Externe berichten** **uw Exchange Online Exchange transportregels handhaven (ETRs) in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="dee3b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="dee3b-108">Selecteer **Save**.</span><span class="sxs-lookup"><span data-stu-id="dee3b-108">Choose **Save**.</span></span>

<span data-ttu-id="dee3b-109">Voor meer informatie Zie [externe berichten in een netwerk Yammer met Exchange transportregels, besturingselement](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="dee3b-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  