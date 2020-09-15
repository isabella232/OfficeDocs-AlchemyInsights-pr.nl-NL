---
title: Maak een e-mail-catch all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712981"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="f9fee-102">Maak een e-mail-catch all</span><span class="sxs-lookup"><span data-stu-id="f9fee-102">Create an email catch all</span></span>

<span data-ttu-id="f9fee-103">Het gebruik van een catch-all wordt sterk ontmoedigd.</span><span class="sxs-lookup"><span data-stu-id="f9fee-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="f9fee-104">Het is beter om de afzender te laten weten dat ze hun bericht niet kunnen afleveren als geadresseerd zodat ze een actie kunnen ondernemen.</span><span class="sxs-lookup"><span data-stu-id="f9fee-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="f9fee-105">U kunt ook het bewaakte postvak beperken, zodat alleen eerder geldige e-mailadressen worden onderschept.</span><span class="sxs-lookup"><span data-stu-id="f9fee-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="f9fee-106">Willekeurige vangst berichten ontvangen een goede aanbieding van spam en kunnen uiteindelijk opvullen, indien niet nauwkeurig wordt gecontroleerd.</span><span class="sxs-lookup"><span data-stu-id="f9fee-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="f9fee-107">(Er worden limieten ontvangen.)</span><span class="sxs-lookup"><span data-stu-id="f9fee-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="f9fee-108">Als u wilt doorgaan, gaat u als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="f9fee-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="f9fee-109">Maak een dynamische distributiegroep & Neem de ' alle typen geadresseerden '.</span><span class="sxs-lookup"><span data-stu-id="f9fee-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="f9fee-110">Maak een specifiek postvak voor het verwerken van e-mailberichten, bijvoorbeeld catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="f9fee-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="f9fee-111">Stel voor het specifieke domein de DomainType in op ' InternalRelay '.</span><span class="sxs-lookup"><span data-stu-id="f9fee-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="f9fee-112">Als u de optie catch later verwijdert, dient u het domein weer in te stellen op gezaghebbend.</span><span class="sxs-lookup"><span data-stu-id="f9fee-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="f9fee-113">Maak als volgt een transport-Transport regel:</span><span class="sxs-lookup"><span data-stu-id="f9fee-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="f9fee-114">Als de afzender zich buiten de organisatie bevindt</span><span class="sxs-lookup"><span data-stu-id="f9fee-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="f9fee-115">Het bericht omleiden naar Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="f9fee-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="f9fee-116">Behalve als de ontvanger lid is van allusers@domain.com (distributiegroep bevat alle leden)</span><span class="sxs-lookup"><span data-stu-id="f9fee-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="f9fee-117">Controleren of nieuwe postvakken worden toegevoegd aan de dynamische distributiegroep</span><span class="sxs-lookup"><span data-stu-id="f9fee-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
