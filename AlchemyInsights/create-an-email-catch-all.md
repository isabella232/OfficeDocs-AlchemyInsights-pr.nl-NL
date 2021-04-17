---
title: Een e-mail catch all maken
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816195"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="234e3-102">Een e-mail catch all maken</span><span class="sxs-lookup"><span data-stu-id="234e3-102">Create an email catch all</span></span>

<span data-ttu-id="234e3-103">Het gebruik van een catch all wordt sterk afgeraden.</span><span class="sxs-lookup"><span data-stu-id="234e3-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="234e3-104">Het is beter om een bounce terug te geven aan de afzender om afzenders te laten weten dat hun bericht niet kan worden bezorgd als geadresseerd, zodat ze actie kunnen ondernemen.</span><span class="sxs-lookup"><span data-stu-id="234e3-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="234e3-105">U kunt het bewaakte postvak ook beperken tot alleen voorheen geldige e-mailadressen.</span><span class="sxs-lookup"><span data-stu-id="234e3-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="234e3-106">Elke catch all mailbox ontvangt een groot deel van de spam en kan uiteindelijk worden gevuld als het niet goed wordt gecontroleerd.</span><span class="sxs-lookup"><span data-stu-id="234e3-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="234e3-107">(Er zijn ontvangstlimieten.)</span><span class="sxs-lookup"><span data-stu-id="234e3-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="234e3-108">Als u besluit verder te gaan, volgt u de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="234e3-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="234e3-109">Maak een dynamische distributiegroep & 'Alle typen geadresseerden'.</span><span class="sxs-lookup"><span data-stu-id="234e3-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="234e3-110">Maak een speciaal postvak om e-mailberichten te ontvangen, bijvoorbeeld catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="234e3-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="234e3-111">Stel voor het specifieke domein het DomainType in op 'InternalRelay'.</span><span class="sxs-lookup"><span data-stu-id="234e3-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="234e3-112">Als u de catch all later verwijdert, moet u het domein opnieuw instellen op Gezaghebbend.</span><span class="sxs-lookup"><span data-stu-id="234e3-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="234e3-113">Maak als volgt een Mailflow-transportregel:</span><span class="sxs-lookup"><span data-stu-id="234e3-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="234e3-114">Als de afzender 'Buiten de organisatie' is</span><span class="sxs-lookup"><span data-stu-id="234e3-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="234e3-115">Het bericht omleiden naar Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="234e3-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="234e3-116">Behalve als de geadresseerde lid is van allusers@domain.com (Distributiegroep bevat alle leden)</span><span class="sxs-lookup"><span data-stu-id="234e3-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="234e3-117">Controleer of nieuwe postvakken worden toegevoegd aan de dynamische distributiegroep</span><span class="sxs-lookup"><span data-stu-id="234e3-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
