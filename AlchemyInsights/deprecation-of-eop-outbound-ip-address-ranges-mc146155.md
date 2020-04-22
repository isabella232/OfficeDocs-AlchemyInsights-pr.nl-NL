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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Afschaffing van uitgaande IP-adresbereiken van EOP

We hebben een mogelijk probleem met uw organisatie ontdekt dat (als deze niet is gecorrigeerd voor 26 oktober 2018) de e-mailstroom naar uw on-premises of externe bestemmingen kan breken. Zoals eerder gecommuniceerd, om het beheer van ip-adresbereik te vereenvoudigen, consolideren we de IP-adresbereiken (Exchange Online Protection) die worden gebruikt om e-mail buiten Microsoft 365 te verzenden en te ontvangen. Uit onze analyse blijkt dat een of meer van de externe e-mailbronnen of -bestemmingen die u hebt geconfigureerd in e-mailstroomconnectors geen verbindingen accepteren vanuit de ip-adresbereiken die [hier](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)worden weergegeven.

Besluit vóór 26 oktober om ervoor te zorgen dat deze bronnen en bestemmingen verbindingen van en naar alle [gepubliceerde EOP IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)accepteren.

Zie BerichtenCENTRUM-berichten [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)of [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)voor meer informatie over deze wijziging.

**Opmerking:** Als u eerder IP- of URL-publicatie via HTML, XML en RSS hebt gebruikt voor endpoint-updates, moet u ook migreren naar de nieuwe webservices voor het automatiseren van dit soort updates. Zie [Microsoft 365-eindpuntcategorieën en Microsoft 365-webservice VOOR](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)meer informatie .
