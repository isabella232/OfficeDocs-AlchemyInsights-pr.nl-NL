---
title: 1065 afschrijving van EOP uitgaande IP-adres rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284065"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="52cfb-102">Afschrijving van EOP uitgaande IP-adresbereiken</span><span class="sxs-lookup"><span data-stu-id="52cfb-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="52cfb-p101">We hebben een probleem met uw organisatie die (indien niet gecorrigeerd door te 26e oktober 2018) e-mailstroom naar uw in ruimten of externe bestemmingen breekt mogelijk vastgesteld. Als eerder meegedeeld, ter vereenvoudiging van het beheer van IP-adres bereik samenvoegt we de Exchange Online bescherming (EOP) IP-adresbereiken die worden gebruikt voor het verzenden en ontvangen van e-mailadres buiten Office 365. Onze analyse geeft aan dat een of meer van de e-mail van externe bronnen of bestemmingen die u hebt geconfigureerd in e-mail stroom connectors verbindingen met het IP-adres bereiken die [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden niet geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="52cfb-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="52cfb-106">Handelen voordat de 26e oktober om ervoor te zorgen dat deze bronnen en bestemmingen verbindingen van en naar alle [gepubliceerde EOP IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="52cfb-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="52cfb-107">Zie dat Message Center boekt, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)of [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)voor meer informatie over deze wijziging.</span><span class="sxs-lookup"><span data-stu-id="52cfb-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="52cfb-p102">**Opmerking**: als u eerder IP of URL publiceren via HTML, XML en RSS voor eindpunt updates gebruikt, ook moet u migreren naar het nieuwe webservices voor het automatiseren van deze typen updates. Zie voor meer informatie, [eindpunt categorieën van Office 365 en Office 365-IP-adres en URL-webservice](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="52cfb-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

