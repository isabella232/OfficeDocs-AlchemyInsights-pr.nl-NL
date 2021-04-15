---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770986"
---
# <a name="verify-your-domain"></a><span data-ttu-id="996d3-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="996d3-102">Verify your domain</span></span>

 <span data-ttu-id="996d3-103">**De record is waarschijnlijk niet op internet bijgewerkt.**</span><span class="sxs-lookup"><span data-stu-id="996d3-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="996d3-104">Meestal duurt het slechts enkele minuten voordat we de nieuwe record kunnen zien, maar af en toe kan het enkele uren duren.</span><span class="sxs-lookup"><span data-stu-id="996d3-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="996d3-105">Als u al zo lang hebt gewacht, controleert u of u de exacte waarde hebt gekopieerd en in de TXT-verificatierecord bij uw DNS-host hebt gekopieerd en geklikt.</span><span class="sxs-lookup"><span data-stu-id="996d3-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="996d3-106">Een veelvoorkomende fout is dat het gedeelte 'MS=' van de record niet mee is gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="996d3-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="996d3-107">Maar dat hebben we ook nodig!</span><span class="sxs-lookup"><span data-stu-id="996d3-107">We need that too!</span></span>

- <span data-ttu-id="996d3-108">Bij sommige DNS-hosts moet u een extra stap nemen om het zonebestand (waarin de DNS-record wordt opgeslagen) op te slaan zodat dit overal op internet wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="996d3-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="996d3-109">Zorg ervoor dat u uw wijzigingen hebt opgeslagen, zodat Microsoft de record kan zien en controleren.</span><span class="sxs-lookup"><span data-stu-id="996d3-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
