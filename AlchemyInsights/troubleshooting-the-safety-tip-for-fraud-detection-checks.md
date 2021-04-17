---
title: Problemen oplossen met de veiligheidstip voor fraudedetectiecontroles
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834726"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problemen oplossen met de veiligheidstip voor fraudedetectiecontroles

Als u een veiligheidstip krijgt met de opmerking 'De afzender heeft onze fraudedetectiecontroles niet uitgevoerd en is mogelijk niet de persoon die ze lijken te zijn', dan is de afzender niet geslaagd voor DKIM- of SPF-verificatiecontroles. De beste methode om dit op te lossen is voor de afzender om zichzelf te machtigen. Als de afzender namens u verstuurt, moet u deze machtigen door het IP-adres van de afzender toe te voegen aan uw SPF-record.
  
Zie [Het oplossen van de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.
  
Hier vindt u enkele andere koppelingen die u kunnen helpen:
  
- [Hoe Microsoft sender policy framework (SPF) gebruikt om spoofing te voorkomen](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF instellen om adresvervalsing te helpen voorkomen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
