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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="eb411-102">Problemen oplossen met de veiligheidstip voor fraudedetectiecontroles</span><span class="sxs-lookup"><span data-stu-id="eb411-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="eb411-103">Als u een veiligheidstip krijgt met de tekst "De afzender heeft onze fraudedetectiecontroles niet uitgevoerd en mogelijk niet zijn wie ze lijken te zijn", dan is de afzender niet geslaagd voor dkim- of SPF-verificatiecontroles.</span><span class="sxs-lookup"><span data-stu-id="eb411-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="eb411-104">De beste methode om dit op te lossen is voor de afzender om zichzelf te autoriseren.</span><span class="sxs-lookup"><span data-stu-id="eb411-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="eb411-105">Als de afzender namens u verzendt, moet u deze autoriseren door het IP-adres van de afzender toe te voegen aan uw SPF-record.</span><span class="sxs-lookup"><span data-stu-id="eb411-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="eb411-106">Zie [Het oplossen van de rode (verdachte) veiligheidstip voor fraudedetectiecontroles](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="eb411-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="eb411-107">Hier zijn een aantal andere links die kunnen helpen:</span><span class="sxs-lookup"><span data-stu-id="eb411-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="eb411-108">Hoe Microsoft het beleidframework (Sender Policy Framework) gebruikt om spoofing te voorkomen</span><span class="sxs-lookup"><span data-stu-id="eb411-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="eb411-109">SPF instellen om spoofing te voorkomen</span><span class="sxs-lookup"><span data-stu-id="eb411-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
