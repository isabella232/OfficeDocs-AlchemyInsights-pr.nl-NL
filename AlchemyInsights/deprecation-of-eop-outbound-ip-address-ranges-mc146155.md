---
title: 1065 Deprecation van EOP uitgaande IP-adresbereikenMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704592"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="c3731-102">Afschaffing van uitgaande IP-adresbereiken van EOP</span><span class="sxs-lookup"><span data-stu-id="c3731-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="c3731-103">We hebben een mogelijk probleem met uw organisatie ontdekt dat (als deze niet is gecorrigeerd voor 26 oktober 2018) de e-mailstroom naar uw on-premises of externe bestemmingen kan breken.</span><span class="sxs-lookup"><span data-stu-id="c3731-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="c3731-104">Zoals eerder gecommuniceerd, om het beheer van ip-adresbereik te vereenvoudigen, consolideren we de IP-adresbereiken (Exchange Online Protection) die worden gebruikt om e-mail buiten Microsoft 365 te verzenden en te ontvangen.</span><span class="sxs-lookup"><span data-stu-id="c3731-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="c3731-105">Uit onze analyse blijkt dat een of meer van de externe e-mailbronnen of -bestemmingen die u hebt geconfigureerd in e-mailstroomconnectors geen verbindingen accepteren vanuit de ip-adresbereiken die [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden weergegeven.</span><span class="sxs-lookup"><span data-stu-id="c3731-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c3731-106">Besluit vóór 26 oktober om ervoor te zorgen dat deze bronnen en bestemmingen verbindingen van en naar alle [gepubliceerde EOP IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)accepteren.</span><span class="sxs-lookup"><span data-stu-id="c3731-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c3731-107">Zie BerichtenCENTRUM-berichten [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)of [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)voor meer informatie over deze wijziging.</span><span class="sxs-lookup"><span data-stu-id="c3731-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="c3731-108">**Opmerking:** Als u eerder IP- of URL-publicatie via HTML, XML en RSS hebt gebruikt voor endpoint-updates, moet u ook migreren naar de nieuwe webservices voor het automatiseren van dit soort updates.</span><span class="sxs-lookup"><span data-stu-id="c3731-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="c3731-109">Zie [Microsoft 365-eindpuntcategorieën en Microsoft 365-webservice VOOR](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)meer informatie .</span><span class="sxs-lookup"><span data-stu-id="c3731-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
