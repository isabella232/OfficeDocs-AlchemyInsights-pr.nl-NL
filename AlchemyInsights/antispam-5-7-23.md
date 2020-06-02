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
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506438"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="bf8a1-102">Problemen met e-mailbezorging oplossen voor foutcode 5.7.23</span><span class="sxs-lookup"><span data-stu-id="bf8a1-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="bf8a1-103">Controleer de DNS-record SPF voor uw domein bij een openbaar beschikbare SPF- of DNS-recordcontrole op het web.</span><span class="sxs-lookup"><span data-stu-id="bf8a1-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="bf8a1-104">Controleer of het uitgaande bericht niet door Microsoft als spam is geïdentificeerd en door de [pool met levering met een hoog risico is](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)doorgestuurd.</span><span class="sxs-lookup"><span data-stu-id="bf8a1-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="bf8a1-105">Berichten in de pool met levering met een hoog risico worden niet doorgegeven aan SPF-controles en worden daarom niet geaccepteerd door de e-mailorganisatie voor bestemmingen.</span><span class="sxs-lookup"><span data-stu-id="bf8a1-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="bf8a1-106">Als het probleem blijft bestaan, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u e-mail probeert te verzenden.</span><span class="sxs-lookup"><span data-stu-id="bf8a1-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="bf8a1-107">Noteer de gedetailleerde externe fout die beschikbaar is in het bouncebericht.</span><span class="sxs-lookup"><span data-stu-id="bf8a1-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="bf8a1-108">Microsoft-ondersteuning kan mogelijk niet verder helpen.</span><span class="sxs-lookup"><span data-stu-id="bf8a1-108">Microsoft support may not be able to assist further.</span></span>
