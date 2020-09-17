---
title: 1065 afschaffing van het uitgaande IP-adres van EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806790"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="24ca3-102">Afschaffing van EOP uitgaande IP-adresbereiken</span><span class="sxs-lookup"><span data-stu-id="24ca3-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="24ca3-103">Er is een potentieel probleem met uw organisatie vastgesteld die (als dit niet is gecorrigeerd door 26 oktober 2018) kan de e-mail stroom naar uw on-premises of externe bestemmingen verbreken.</span><span class="sxs-lookup"><span data-stu-id="24ca3-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="24ca3-104">Ter vereenvoudiging van IP-adresbereiken voor een eenvoudiger beheer van IP-adresbereiken wordt de IP-adresbereiken van Exchange Online Protection (EOP) die worden gebruikt voor het verzenden en ontvangen van e-mail buiten Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="24ca3-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="24ca3-105">Onze analyse geeft aan dat een of meer externe e-mail bronnen of-bestemmingen die u hebt geconfigureerd in de e-mail stroom verbindingslijnen, geen verbindingen accepteren van de IP-adresbereiken die [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="24ca3-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="24ca3-106">Handel voor de 26 van oktober om ervoor te zorgen dat deze bronnen en bestemmingen verbindingen accepteren van en naar alle [gepubliceerde EOP IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="24ca3-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="24ca3-107">Zie berichtencentrum berichten [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)of [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)voor meer informatie over deze wijziging.</span><span class="sxs-lookup"><span data-stu-id="24ca3-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="24ca3-108">**Opmerking**: als u eerder een IP-of URL-publicatie via HTML, XML en RSS voor eindpunt updates hebt gebruikt, moet u ook migreren naar de nieuwe webservices om dit soort updates te automatiseren.</span><span class="sxs-lookup"><span data-stu-id="24ca3-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="24ca3-109">Zie [Microsoft 365-eindpunt categorieën en Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="24ca3-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
