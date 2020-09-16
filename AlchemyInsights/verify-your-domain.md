---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734301"
---
# <a name="verify-your-domain"></a><span data-ttu-id="3c0f9-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="3c0f9-102">Verify your domain</span></span>

 <span data-ttu-id="3c0f9-103">**De record is waarschijnlijk niet bijgewerkt via internet.**</span><span class="sxs-lookup"><span data-stu-id="3c0f9-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="3c0f9-104">Het duurt meestal maar een paar minuten voordat de nieuwe record kan worden weergegeven, maar soms kan het even duren voordat het een paar uur duurt.</span><span class="sxs-lookup"><span data-stu-id="3c0f9-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="3c0f9-105">Als u de presentatie al lang hebt gewacht, controleert u of u de exacte waarde hebt gekopieerd en geplakt in de TXT-verificatie record bij de DNS-host.</span><span class="sxs-lookup"><span data-stu-id="3c0f9-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="3c0f9-106">Een veelvoorkomende fout is dat het gedeelte 'MS=' van de record niet mee is gekopieerd.</span><span class="sxs-lookup"><span data-stu-id="3c0f9-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="3c0f9-107">Maar dat hebben we ook nodig!</span><span class="sxs-lookup"><span data-stu-id="3c0f9-107">We need that too!</span></span>

- <span data-ttu-id="3c0f9-108">Bij sommige DNS-hosts moet u een extra stap nemen om het zonebestand (waarin de DNS-record wordt opgeslagen) op te slaan zodat dit overal op internet wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="3c0f9-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="3c0f9-109">Zorg ervoor dat u de wijzigingen hebt opgeslagen, zodat Microsoft de record kan zien en verifiëren.</span><span class="sxs-lookup"><span data-stu-id="3c0f9-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
