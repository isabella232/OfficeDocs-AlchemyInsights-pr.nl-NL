---
title: Probleemoplossing voor de veiligheidstip voor fraudedetectiecontroles
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
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504978"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Probleemoplossing voor de veiligheidstip voor fraudedetectiecontroles

Als u een veiligheidstip krijgt met de tekst "De afzender heeft onze fraudedetectiecontroles niet uitgevoerd en mogelijk niet wie ze lijken te zijn", dan is de afzender niet geslaagd voor DKIM- of SPF-verificatiecontroles. De beste methode om dit op te lossen is dat de afzender zichzelf kan autoriseren. Als de afzender namens u verzendt, moet u deze autoriseren door het IP-adres van de afzender toe te voegen aan uw SPF-record.
  
Zie [Probleemoplossing voor de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.
  
Hier zijn een aantal andere links die kunnen helpen:
  
- [Hoe Microsoft het SPF (Sender Policy Framework) gebruikt om spoofing te voorkomen](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF instellen om adresvervalsing te helpen voorkomen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
