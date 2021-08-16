---
title: 1065 Deprecation of EOP outbound IP address rangesMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031257"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Intrekking van uitgaande IP-adresbereiken van EOP

Er is een mogelijk probleem met uw organisatie aangetroffen dat (indien niet gecorrigeerd op 26 oktober 2018) de e-mailstroom naar uw on-premises of externe bestemmingen kan breken. Zoals eerder is gemeld, consolideren we de IP-adresbereiken van Exchange Online Protection (EOP) die worden gebruikt om e-mail te verzenden en te ontvangen buiten Microsoft 365. Onze analyse geeft aan dat een of meer externe e-mailbronnen of bestemmingen die u hebt geconfigureerd in verbindingslijnen voor e-mailstroom, geen verbindingen accepteren vanuit de IP-adresbereiken die hier worden [weergegeven.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Ga vóór 26 oktober te werk om ervoor te zorgen dat deze bronnen en bestemmingen verbindingen accepteren van en naar alle [gepubliceerde EOP-IP-adressen.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Zie Berichten in het Berichtencentrum [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)of [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)voor meer informatie over deze wijziging.

**Opmerking:** Als u eerder IP- of URL-publicatie hebt gebruikt via HTML, XML en RSS voor eindpuntupdates, moet u ook migreren naar de nieuwe webservices voor het automatiseren van dit soort updates. Zie voor meer informatie Microsoft 365 eindpuntcategorieën en [Microsoft 365 IP-adres- en URL-webservice.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
