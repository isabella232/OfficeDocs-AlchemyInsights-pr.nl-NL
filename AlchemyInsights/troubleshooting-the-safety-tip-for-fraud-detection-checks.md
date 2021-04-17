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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="2e766-102">Problemen oplossen met de veiligheidstip voor fraudedetectiecontroles</span><span class="sxs-lookup"><span data-stu-id="2e766-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="2e766-103">Als u een veiligheidstip krijgt met de opmerking 'De afzender heeft onze fraudedetectiecontroles niet uitgevoerd en is mogelijk niet de persoon die ze lijken te zijn', dan is de afzender niet geslaagd voor DKIM- of SPF-verificatiecontroles.</span><span class="sxs-lookup"><span data-stu-id="2e766-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="2e766-104">De beste methode om dit op te lossen is voor de afzender om zichzelf te machtigen.</span><span class="sxs-lookup"><span data-stu-id="2e766-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="2e766-105">Als de afzender namens u verstuurt, moet u deze machtigen door het IP-adres van de afzender toe te voegen aan uw SPF-record.</span><span class="sxs-lookup"><span data-stu-id="2e766-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="2e766-106">Zie [Het oplossen van de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="2e766-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="2e766-107">Hier vindt u enkele andere koppelingen die u kunnen helpen:</span><span class="sxs-lookup"><span data-stu-id="2e766-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="2e766-108">Hoe Microsoft sender policy framework (SPF) gebruikt om spoofing te voorkomen</span><span class="sxs-lookup"><span data-stu-id="2e766-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="2e766-109">SPF instellen om adresvervalsing te helpen voorkomen</span><span class="sxs-lookup"><span data-stu-id="2e766-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
