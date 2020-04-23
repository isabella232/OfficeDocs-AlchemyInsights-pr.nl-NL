---
title: Externe groepen uitschakelen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720763"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="42f8b-102">Externe groepen uitschakelen</span><span class="sxs-lookup"><span data-stu-id="42f8b-102">How to disable External Groups</span></span>

<span data-ttu-id="42f8b-103">Yammer externe messaging past Exchange Transport Rules (ETRs), een set proactieve controles om te voorkomen dat bedrijfsinformatie wordt gedeeld.</span><span class="sxs-lookup"><span data-stu-id="42f8b-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="42f8b-104">Als u wilt voorkomen dat gebruikers externe groepen maken, moet u een Exchange-transportregel (ETR) configureren en Yammer configureren om de exchange-transportregel te gebruiken om externe berichten te blokkeren.</span><span class="sxs-lookup"><span data-stu-id="42f8b-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="42f8b-105">Nadat u een regel hebt gemaakt in het Exchange Online-beheercentrum, voert u de volgende stappen uit om etr toe te passen in Yammer:</span><span class="sxs-lookup"><span data-stu-id="42f8b-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="42f8b-106">Meld u aan bij Yammer als geverifieerde beheerder en ga in het **Yammer-beheercentrum**naar Inhoud **s- en \> beveiligingsinstellingen c.**</span><span class="sxs-lookup"><span data-stu-id="42f8b-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="42f8b-107">Selecteer **Onder Externe berichten**de optie Uw Exchange Online Exchange Transport Rules **(ETRs) afdwingen in Yammer.**</span><span class="sxs-lookup"><span data-stu-id="42f8b-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="42f8b-108">Selecteer **Save**.</span><span class="sxs-lookup"><span data-stu-id="42f8b-108">Choose **Save**.</span></span>

<span data-ttu-id="42f8b-109">Zie [Externe berichten uitschakelen in een Yammer-netwerk](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="42f8b-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  