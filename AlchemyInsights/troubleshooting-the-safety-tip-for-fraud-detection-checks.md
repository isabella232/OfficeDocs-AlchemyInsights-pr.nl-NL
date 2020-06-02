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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="1dfcc-102">Probleemoplossing voor de veiligheidstip voor fraudedetectiecontroles</span><span class="sxs-lookup"><span data-stu-id="1dfcc-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="1dfcc-103">Als u een veiligheidstip krijgt met de tekst "De afzender heeft onze fraudedetectiecontroles niet uitgevoerd en mogelijk niet wie ze lijken te zijn", dan is de afzender niet geslaagd voor DKIM- of SPF-verificatiecontroles.</span><span class="sxs-lookup"><span data-stu-id="1dfcc-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="1dfcc-104">De beste methode om dit op te lossen is dat de afzender zichzelf kan autoriseren.</span><span class="sxs-lookup"><span data-stu-id="1dfcc-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="1dfcc-105">Als de afzender namens u verzendt, moet u deze autoriseren door het IP-adres van de afzender toe te voegen aan uw SPF-record.</span><span class="sxs-lookup"><span data-stu-id="1dfcc-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="1dfcc-106">Zie [Probleemoplossing voor de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="1dfcc-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="1dfcc-107">Hier zijn een aantal andere links die kunnen helpen:</span><span class="sxs-lookup"><span data-stu-id="1dfcc-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="1dfcc-108">Hoe Microsoft het SPF (Sender Policy Framework) gebruikt om spoofing te voorkomen</span><span class="sxs-lookup"><span data-stu-id="1dfcc-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="1dfcc-109">SPF instellen om adresvervalsing te helpen voorkomen</span><span class="sxs-lookup"><span data-stu-id="1dfcc-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
