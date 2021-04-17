---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821406"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="ee29a-102">Problemen met e-mailbezorging oplossen voor foutcode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="ee29a-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="ee29a-103">Controleer de SPF DNS-record voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op het web.</span><span class="sxs-lookup"><span data-stu-id="ee29a-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="ee29a-104">Controleer of het uitgaande bericht niet is geïdentificeerd als spam door Microsoft en door de groep met hoge [risicobezorging is gerouteerd.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="ee29a-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="ee29a-105">Berichten in de groep Bezorging met hoog risico worden niet door SPF-controles uitgevoerd en worden daarom niet geaccepteerd door de doel-e-mailorganisatie.</span><span class="sxs-lookup"><span data-stu-id="ee29a-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="ee29a-106">Als het probleem zich blijft voordoen, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waaraan u e-mail wilt verzenden.</span><span class="sxs-lookup"><span data-stu-id="ee29a-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="ee29a-107">Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht.</span><span class="sxs-lookup"><span data-stu-id="ee29a-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="ee29a-108">Microsoft-ondersteuning kan mogelijk niet verder helpen.</span><span class="sxs-lookup"><span data-stu-id="ee29a-108">Microsoft support may not be able to assist further.</span></span>
