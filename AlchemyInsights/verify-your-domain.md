---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
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
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365412"
---
# <a name="verify-your-domain"></a><span data-ttu-id="0b7c8-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="0b7c8-102">Verify your domain</span></span>

 <span data-ttu-id="0b7c8-103">**De waarschijnlijk nog niet bijgewerkt via het Internet.**</span><span class="sxs-lookup"><span data-stu-id="0b7c8-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="0b7c8-104">Meestal duurt het slechts een paar minuten om te zien de nieuwe record, maar af en toe kunt uitvoeren zolang een paar uur.</span><span class="sxs-lookup"><span data-stu-id="0b7c8-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="0b7c8-105">Als u die al lang hebt gewacht, Controleer dat u hebt gekopieerd en geplakt van de exacte waarde in de TXT-record voor verificatie op uw DNS-host.</span><span class="sxs-lookup"><span data-stu-id="0b7c8-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="0b7c8-106">Een veelvoorkomende fout is dat het gedeelte 'MS=' van de record niet mee is gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="0b7c8-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="0b7c8-107">Maar dat hebben we ook nodig!</span><span class="sxs-lookup"><span data-stu-id="0b7c8-107">We need that too!</span></span>

- <span data-ttu-id="0b7c8-108">Bij sommige DNS-hosts moet u een extra stap nemen om het zonebestand (waarin de DNS-record wordt opgeslagen) op te slaan zodat dit overal op internet wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="0b7c8-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="0b7c8-109">Controleer of u de wijzigingen hebt opgeslagen zodat Office 365 de record kan waarnemen en controleren.</span><span class="sxs-lookup"><span data-stu-id="0b7c8-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
