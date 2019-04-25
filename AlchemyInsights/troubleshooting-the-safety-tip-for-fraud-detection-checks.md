---
title: Problemen met de veiligheid tip voor fraude-opsporing wordt gecontroleerd
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 98627edcd2b685673dda8a8a18821eddf9b64bc1
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391204"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="9de91-102">Problemen met de veiligheid tip voor fraude-opsporing wordt gecontroleerd</span><span class="sxs-lookup"><span data-stu-id="9de91-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="9de91-103">Als u veiligheid tip die aldus "de afzender is onze fraude detectie controles mislukt en mogelijk niet wie ze lijken te zijn", dan kan de afzender niet DKIM of SPF verificatiecontroles doorgeven.</span><span class="sxs-lookup"><span data-stu-id="9de91-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="9de91-104">De beste methode om dit probleem oplossen is voor de afzender zelf toe te staan.</span><span class="sxs-lookup"><span data-stu-id="9de91-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="9de91-105">Als de afzender namens u verzendt, moet u toestaan dat ze door het IP-adres van de afzender toe te voegen aan de SPF-record.</span><span class="sxs-lookup"><span data-stu-id="9de91-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="9de91-106">Zie [problemen met de veiligheid van rood (verdachte) tip voor fraude-opsporing gecontroleerd](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer info.</span><span class="sxs-lookup"><span data-stu-id="9de91-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="9de91-107">Hier volgen enkele koppelingen die kunnen helpen:</span><span class="sxs-lookup"><span data-stu-id="9de91-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="9de91-108">Hoe Office 365 afzender policy framework (SPF) gebruikt om te voorkomen dat spoofing</span><span class="sxs-lookup"><span data-stu-id="9de91-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- <span data-ttu-id="9de91-109">[Set up SPF in Office 365 to help prevent spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing) (SPF in Office 365 instellen om spoofing te helpen voorkomen)</span><span class="sxs-lookup"><span data-stu-id="9de91-109">[Set up SPF in Office 365 to help prevent spoofing](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)</span></span>
    

