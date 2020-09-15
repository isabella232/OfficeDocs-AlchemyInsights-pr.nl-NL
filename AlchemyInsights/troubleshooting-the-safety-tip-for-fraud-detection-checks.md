---
title: Problemen oplossen met de veiligheids tip voor fraude detectie controles
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658405"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="5c7ae-102">Problemen oplossen met de veiligheids tip voor fraude detectie controles</span><span class="sxs-lookup"><span data-stu-id="5c7ae-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="5c7ae-103">Als u een veiligheids bericht ontvangt met de tekst "de afzender is mislukt onze fraude detectie en mogelijk niet de persoon die het lijkt te zijn, is het niet mogelijk om authenticatie van DKIM of SPF verificatie te volgen.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="5c7ae-104">De beste manier om dit op te lossen is dat de afzender zichzelf kan machtigen.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="5c7ae-105">Als de afzender namens u e-mail verzendt, moet u deze machtigen door het IP-adres van de afzender toe te voegen aan uw SPF-record.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="5c7ae-106">Zie [Probleemoplossing voor de rode (verdachte) beveiligings tip voor fraude detectie gecontroleerd](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="5c7ae-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="5c7ae-107">Hier volgen nog enkele andere koppelingen die u kunnen helpen:</span><span class="sxs-lookup"><span data-stu-id="5c7ae-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="5c7ae-108">Hoe Microsoft gebruikmaakt van het Microsoft-beleid (Sender Policy Framework) om spoofing te voorkomen</span><span class="sxs-lookup"><span data-stu-id="5c7ae-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="5c7ae-109">SPF instellen om adresvervalsing te helpen voorkomen</span><span class="sxs-lookup"><span data-stu-id="5c7ae-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
