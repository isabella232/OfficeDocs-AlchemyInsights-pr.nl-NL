---
title: Ontbrekende voorwaarden in het SharePoint Online-Termenarchief
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750446"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-versleuteling inschakelen met intune

Het beleid voor het intune-endpoint voor beveiliging kan worden gebruikt voor het configureren van Boitlocker versleutelingsinstellingen voor Windows-apparaten, zoals beschreven in de Windows 10-(en latere) instellingen om apparaten te beschermen met intune.

U dient te beseffen dat veel nieuwere apparaten met Windows 10 automatische BitLocker-versleuteling ondersteunen die wordt geactiveerd zonder de toepassing van MDM-beleid. Dit kan van invloed zijn op de toepassing van het beleid als niet-standaardinstellingen zijn geconfigureerd. Zie Veelgestelde vragen voor meer informatie.


Veelgestelde vragen   : welke edities van Windows ondersteuning bieden voor apparaatversleuteling met het Endpoint Protection-beleid?
 A: de instellingen in intune-Endpoint Protection-beleid worden geïmplementeerd met de BitLocker CSP.Niet alle edities en versies van Windows ondersteunen de BitLocker CSP. 
      Op dit moment Windows-edities: Enterprise; Education, Mobile, Mobile Enterprise en Professional (vanaf build 1809 en later) worden ondersteund.




V: als een apparaat al is versleuteld met BitLocker met behulp van de standaardinstellingen van het besturingssysteem voor versleutelingsmethode en cipher vastheid (XTS-AES-128), wordt het toepassen van een beleid waarbij verschillende instellingen worden gebruikt, automatisch opnieuw versleutelen met de nieuwe instellingen?

A: Nee. Om de nieuwe instellingen voor Cipher toe te passen, moet het station eerst worden gedecodeerd.

Opmerking voor apparaten die worden geregistreerd met auto pilot de automatische versleuteling die zich in OOBE voordoet, wordt niet geactiveerd totdat het intune-beleid wordt geëvalueerd, zodat de beleidsinstellingen die kunnen worden gebruikt in plaats van de standaardinstellingen voor het besturingssysteem worden gebruikt.




V als een apparaat is versleuteld als gevolg van de toepassing van intune-beleid wordt deze gedecodeerd wanneer dat beleid wordt verwijderd?

A: het verwijderen van een beleids versleuteling heeft geen invloed op de decodering van de stations die zijn geconfigureerd.




V: Waarom wordt in het nalevingsbeleid van intune aangegeven dat mijn apparaat geen ' BitLocker ingeschakeld ' bevat, maar het is?

A: de instelling ' BitLocker ingeschakeld ' in het intune-nalevingsbeleid maakt gebruik van de client (DHA) voor Windows-apparaatstatusverklaring. Dit is alleen van toepassing op de status van het apparaat tijdens het opstarten. Als een apparaat niet opnieuw is opgestart sinds de BitLocker-versleuteling werd voltooid, wordt BitLocker niet door de DHA-client gerapporteerd als actief.