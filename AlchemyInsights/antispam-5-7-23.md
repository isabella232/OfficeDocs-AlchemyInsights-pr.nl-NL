---
title: Spam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717320"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Problemen met e-mail bezorging voor foutcode 5.7.23

Controleer de SPF DNS-record voor uw domein bij een openbaar beschikbare SPF-of DNS-record controle op het web.

Controleer of het uitgaande bericht niet als spam door Microsoft is aangemerkt en gerouteerd via de [groep hoog risico voor levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Berichten in de groep hoog risico voor bezorgings berichten worden niet doorzocht, en worden daarom niet door de doel-e-mail organisatie geaccepteerd.

Als het probleem zich blijft voordoen, moet u mogelijk contact opnemen met de beheerder van de e-mailhost waarnaar u probeert e-mail te verzenden. Let op de gedetailleerde externe fout in het e-mailbericht. Microsoft ondersteuning kan mogelijk niet verder worden geholpen.
