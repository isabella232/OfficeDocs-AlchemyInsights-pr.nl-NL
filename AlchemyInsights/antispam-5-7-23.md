---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682096"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="e6275-102">Problemen met de bezorging van e-mail oplossen voor foutcode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="e6275-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="e6275-103">Controleer de SPF DNS-record voor uw domein op een openbaar beschikbare SPF of DNS record checker op het web.</span><span class="sxs-lookup"><span data-stu-id="e6275-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="e6275-104">Controleer of het uitgaande bericht niet is geïdentificeerd als spam door Office 365 en doorgestuurd via de [groep met hoog risico-levering](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="e6275-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="e6275-105">Berichten in de groep met hoog risico levering niet doorgeven SPF controles en daarom niet worden geaccepteerd door de organisatie van de bestemming e-mailadres.</span><span class="sxs-lookup"><span data-stu-id="e6275-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="e6275-106">Als het probleem zich blijft voordoen, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u probeert e-mail te verzenden.</span><span class="sxs-lookup"><span data-stu-id="e6275-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="e6275-107">Noteer de gedetailleerde externe fout die beschikbaar is in het Bounce-bericht.</span><span class="sxs-lookup"><span data-stu-id="e6275-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="e6275-108">Ondersteuning voor Office 365 kan mogelijk niet verder helpen.</span><span class="sxs-lookup"><span data-stu-id="e6275-108">Office 365 support may not be able to assist further.</span></span>