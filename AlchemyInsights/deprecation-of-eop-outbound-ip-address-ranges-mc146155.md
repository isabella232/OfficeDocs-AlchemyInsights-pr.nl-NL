---
title: 1065 afschrijving van EOP uitgaande IP-adres rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404816"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Afschrijving van EOP uitgaande IP-adresbereiken

We hebben een probleem met uw organisatie die (indien niet gecorrigeerd door te 26e oktober 2018) e-mailstroom naar uw in ruimten of externe bestemmingen breekt mogelijk vastgesteld. Als eerder meegedeeld, ter vereenvoudiging van het beheer van IP-adres bereik samenvoegt we de Exchange Online bescherming (EOP) IP-adresbereiken die worden gebruikt voor het verzenden en ontvangen van e-mailadres buiten Office 365. Onze analyse geeft aan dat een of meer van de e-mail van externe bronnen of bestemmingen die u hebt geconfigureerd in e-mail stroom connectors verbindingen met het IP-adres bereiken die [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden niet geaccepteerd.

Handelen voordat de 26e oktober om ervoor te zorgen dat deze bronnen en bestemmingen verbindingen van en naar alle [gepubliceerde EOP IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden geaccepteerd.

Zie dat Message Center boekt, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)of [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)voor meer informatie over deze wijziging.

**Opmerking**: als u eerder IP of URL publiceren via HTML, XML en RSS voor eindpunt updates gebruikt, ook moet u migreren naar het nieuwe webservices voor het automatiseren van deze typen updates. Zie voor meer informatie, [eindpunt categorieën van Office 365 en Office 365-IP-adres en URL-webservice](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
