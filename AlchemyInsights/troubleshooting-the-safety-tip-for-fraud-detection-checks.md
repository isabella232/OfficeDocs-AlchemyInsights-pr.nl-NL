---
title: Problemen oplossen met de veiligheidstip voor fraudedetectiecontroles
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759507"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problemen oplossen met de veiligheidstip voor fraudedetectiecontroles

Als u een veiligheidstip krijgt met de tekst "De afzender heeft onze fraudedetectiecontroles niet uitgevoerd en mogelijk niet zijn wie ze lijken te zijn", dan is de afzender niet geslaagd voor dkim- of SPF-verificatiecontroles. De beste methode om dit op te lossen is voor de afzender om zichzelf te autoriseren. Als de afzender namens u verzendt, moet u deze autoriseren door het IP-adres van de afzender toe te voegen aan uw SPF-record.
  
Zie [Het oplossen van de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.
  
Hier zijn een aantal andere links die kunnen helpen:
  
- [Hoe Microsoft het beleidframework (Sender Policy Framework) gebruikt om spoofing te voorkomen](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF instellen om spoofing te voorkomen](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
