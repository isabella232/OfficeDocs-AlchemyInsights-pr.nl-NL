---
title: Maak een e-mailvangst allemaal
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286105"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="4a4ad-102">Maak een e-mailvangst allemaal</span><span class="sxs-lookup"><span data-stu-id="4a4ad-102">Create an email catch all</span></span>

<span data-ttu-id="4a4ad-103">Het gebruik van een vangst wordt sterk afgeraden.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="4a4ad-104">Het is beter om een bounce terug te geven aan de afzender om afzenders te laten weten dat hun bericht niet kan worden bezorgd zoals geadresseerd, zodat ze actie kunnen ondernemen.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="4a4ad-105">U het bewaakte postvak ook beperken tot alleen voorheen geldige e-mailadressen.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="4a4ad-106">Elke vangst alle mailbox ontvangt een groot deel van spam en kan uiteindelijk vullen, indien niet nauwlettend gecontroleerd.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="4a4ad-107">(Er zijn ontvangstlimieten.)</span><span class="sxs-lookup"><span data-stu-id="4a4ad-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="4a4ad-108">Als u besluit door te gaan, voert u de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="4a4ad-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="4a4ad-109">Maak een dynamische distributiegroep & 'Alle typen geadresseerden' bevatten.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="4a4ad-110">Maak een speciaal postvak om bijvoorbeeld e-mails te vangen catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="4a4ad-111">Stel voor het specifieke domein het DomainType in op "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="4a4ad-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="4a4ad-112">Als u later de vangst allemaal verwijdert, moet u het domein terugzetten naar Authoritative.</span><span class="sxs-lookup"><span data-stu-id="4a4ad-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="4a4ad-113">Maak als volgt een mailflow-transportregel:</span><span class="sxs-lookup"><span data-stu-id="4a4ad-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="4a4ad-114">Als de afzender 'Buiten de organisatie' staat</span><span class="sxs-lookup"><span data-stu-id="4a4ad-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="4a4ad-115">Het bericht omleiden naar Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="4a4ad-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="4a4ad-116">Behalve als de ontvanger lid is van allusers@domain.com (Distributiegroep bevat alle leden)</span><span class="sxs-lookup"><span data-stu-id="4a4ad-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="4a4ad-117">Ervoor zorgen dat nieuwe postvakken worden toegevoegd aan de dynamische distributiegroep</span><span class="sxs-lookup"><span data-stu-id="4a4ad-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
