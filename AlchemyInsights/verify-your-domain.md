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
# <a name="verify-your-domain"></a>Verify your domain

 **De record is waarschijnlijk niet bijgewerkt via internet.**
  
Het duurt meestal maar een paar minuten voordat de nieuwe record kan worden weergegeven, maar soms kan het even duren voordat het een paar uur duurt. 
  
- Als u de presentatie al lang hebt gewacht, controleert u of u de exacte waarde hebt gekopieerd en geplakt in de TXT-verificatie record bij de DNS-host. Een veelvoorkomende fout is dat het gedeelte 'MS=' van de record niet mee is gekopieerd. Maar dat hebben we ook nodig!

- Bij sommige DNS-hosts moet u een extra stap nemen om het zonebestand (waarin de DNS-record wordt opgeslagen) op te slaan zodat dit overal op internet wordt bijgewerkt. Zorg ervoor dat u de wijzigingen hebt opgeslagen, zodat Microsoft de record kan zien en verifiëren.
