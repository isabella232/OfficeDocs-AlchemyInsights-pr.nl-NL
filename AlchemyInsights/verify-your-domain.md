---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710438"
---
# <a name="verify-your-domain"></a><span data-ttu-id="da1c1-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="da1c1-102">Verify your domain</span></span>

 <span data-ttu-id="da1c1-103">**De plaat is waarschijnlijk niet bijgewerkt op het internet.**</span><span class="sxs-lookup"><span data-stu-id="da1c1-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="da1c1-104">Het duurt meestal slechts een paar minuten voor ons in staat zijn om de nieuwe record te zien, maar af en toe kan het zo lang duren als een paar uur.</span><span class="sxs-lookup"><span data-stu-id="da1c1-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="da1c1-105">Als u al zo lang hebt gewacht, controleert u of u de exacte waarde hebt gekopieerd en geplakt in de TXT-verificatierecord bij uw DNS-host.</span><span class="sxs-lookup"><span data-stu-id="da1c1-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="da1c1-106">Een veelvoorkomende fout is dat het gedeelte 'MS=' van de record niet mee is gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="da1c1-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="da1c1-107">Maar dat hebben we ook nodig!</span><span class="sxs-lookup"><span data-stu-id="da1c1-107">We need that too!</span></span>

- <span data-ttu-id="da1c1-108">Bij sommige DNS-hosts moet u een extra stap nemen om het zonebestand (waarin de DNS-record wordt opgeslagen) op te slaan zodat dit overal op internet wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="da1c1-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="da1c1-109">Zorg ervoor dat u de wijzigingen hebt opgeslagen, zodat Microsoft de record kan zien en verifiëren.</span><span class="sxs-lookup"><span data-stu-id="da1c1-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
