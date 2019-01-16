---
title: Winsock-fout 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28283923"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="cdf9b-102">Winsock-fout 10061</span><span class="sxs-lookup"><span data-stu-id="cdf9b-102">Winsock error 10061</span></span>

<span data-ttu-id="cdf9b-p101">Deze foutcode betekent dat Office 365 een TCP-socket (verbinding) met de doelhost niet kan vaststellen. De meest waarschijnlijke oorzaak van deze fout is een probleem met de configuratie van de firewall. Probleem wilt oplossen, moet u deze instellingen controleren:</span><span class="sxs-lookup"><span data-stu-id="cdf9b-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="cdf9b-106">Controleer of de configuratie van de firewall met de gegevens in [Office 365-URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="cdf9b-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="cdf9b-107">Als de fout specifiek naar Exchange Online bescherming (EOP), moet u zijn eerder aangemeld op een wijziging in de [Exchange Online bescherming IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="cdf9b-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="cdf9b-108">Controleer of dat de poort is niet worden geblokkeerd door uw Internet Service Provider (ISP).</span><span class="sxs-lookup"><span data-stu-id="cdf9b-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="cdf9b-109">Controleer of de smart host- en server-instellingen in uw verbindingslijnen.</span><span class="sxs-lookup"><span data-stu-id="cdf9b-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="cdf9b-110">Houd er rekening mee dat Office 365 *binnenkomende* verbindingen op deze manier niet blokkeren.</span><span class="sxs-lookup"><span data-stu-id="cdf9b-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

