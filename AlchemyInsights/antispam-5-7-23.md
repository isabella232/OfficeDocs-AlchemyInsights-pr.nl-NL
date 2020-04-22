---
title: Antispam - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676492"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="f8f75-102">Problemen met e-mailbezorging oplossen voor foutcode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="f8f75-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="f8f75-103">Controleer de SPF DNS-record voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op internet.</span><span class="sxs-lookup"><span data-stu-id="f8f75-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="f8f75-104">Controleer of het uitgaande bericht niet door Microsoft als spam is geïdentificeerd en door de [groep levering met een hoog risico](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)is doorgestuurd.</span><span class="sxs-lookup"><span data-stu-id="f8f75-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="f8f75-105">Berichten in de groep Levering met een hoog risico worden niet door de SPF-controles gehaald en worden daarom niet geaccepteerd door de e-mailorganisatie van de bestemming.</span><span class="sxs-lookup"><span data-stu-id="f8f75-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="f8f75-106">Als het probleem blijft bestaan, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u e-mail probeert te verzenden.</span><span class="sxs-lookup"><span data-stu-id="f8f75-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="f8f75-107">Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht.</span><span class="sxs-lookup"><span data-stu-id="f8f75-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="f8f75-108">Microsoft-ondersteuning kan mogelijk niet verder helpen.</span><span class="sxs-lookup"><span data-stu-id="f8f75-108">Microsoft support may not be able to assist further.</span></span>
