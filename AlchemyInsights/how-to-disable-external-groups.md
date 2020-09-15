---
title: Externe groepen uitschakelen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704123"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="4ab4e-102">Externe groepen uitschakelen</span><span class="sxs-lookup"><span data-stu-id="4ab4e-102">How to disable External Groups</span></span>

<span data-ttu-id="4ab4e-103">Yammer externe berichtuitwisseling toepast Exchange-Transport regels (Etr's), een set proactieve besturingselementen om te voorkomen dat bedrijfsgegevens worden gedeeld.</span><span class="sxs-lookup"><span data-stu-id="4ab4e-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="4ab4e-104">Om te voorkomen dat gebruikers externe groepen kunnen maken, moet u een Exchange-transportregel (ETR toe) configureren en Yammer configureren voor gebruik van de Exchange-transportregel om externe berichten te blokkeren.</span><span class="sxs-lookup"><span data-stu-id="4ab4e-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="4ab4e-105">Wanneer u een regel hebt gemaakt in het Exchange Online-Beheercentrum, voert u deze stappen uit om ETR toe in te stellen voor toepassing in Yammer:</span><span class="sxs-lookup"><span data-stu-id="4ab4e-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="4ab4e-106">Meld u aan bij Yammer als een gecontroleerde beheerder, en in het **Yammer-Beheercentrum**gaat u naar C \*\* \> Beveiligingsinstellingen voor inhoud en beveiliging.\*\*</span><span class="sxs-lookup"><span data-stu-id="4ab4e-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="4ab4e-107">Selecteer onder **externe bericht**uitwisseling **de optie uw Exchange Online Exchange-Transport regels (Etr's) afdwingen in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="4ab4e-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="4ab4e-108">Selecteer **Save**.</span><span class="sxs-lookup"><span data-stu-id="4ab4e-108">Choose **Save**.</span></span>

<span data-ttu-id="4ab4e-109">Zie voor meer informatie [externe berichten uitschakelen in een Yammer-netwerk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="4ab4e-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  