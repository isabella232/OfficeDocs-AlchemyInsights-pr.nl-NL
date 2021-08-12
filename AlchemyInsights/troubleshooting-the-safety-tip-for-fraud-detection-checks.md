---
title: Problemen met de veiligheidstip voor fraudedetectiecontroles oplossen
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
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955961"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Problemen met de veiligheidstip voor fraudedetectiecontroles oplossen

Als u een veiligheidstip met de naam 'De afzender heeft onze controles voor fraudedetectie mislukt en mogelijk niet de persoon is die ze lijken te zijn', kan de afzender DKIM- of SPF-verificatiecontroles niet uitvoeren. De beste methode om dit op te lossen is voor de afzender om zichzelf te machtigen. Als de afzender namens u verstuurt, moet u deze machtigen door het IP-adres van de afzender toe te voegen aan uw SPF-record.
  
Zie [Problemen oplossen met de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.
  
Hier vindt u enkele andere koppelingen die u kunnen helpen:
  
- [Hoe Microsoft sender policy framework (SPF) gebruikt om spoofing te voorkomen](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [SPF instellen om adresvervalsing te helpen voorkomen](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
