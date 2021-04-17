---
title: Meldingen in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833574"
---
# <a name="notifications-in-yammer"></a>Meldingen in Yammer

Om u attent te maken op een nieuwe activiteit in relevante gesprekken, [stuurt Yammer meldingen](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) via e-mail of - als u Yammer op uw mobiele apparaat gebruikt - via pushmeldingen. Yammer verzendt standaardmeldingen voor allerlei typen activiteiten in uw netwerk. Gebruikers kunnen hun e-mailinstellingen bijwerken via de Yammer-website en pushmeldingen worden geconfigureerd in de mobiele app. 

Yammer heeft ondersteuning toegevoegd voor [interactieve e-mails in Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Sommige e-mailberichten (kopie van het bericht) worden interactief in de webversie van Outlook. Een toekomstige update brengt dit naar andere versies van Outlook.

**Soorten meldingen in Yammer**

- E-mailberichten (updates van een groep, iemand nodigt u uit voor een groep, u ontvangt een bericht in uw postvak, enzovoort.)
- Pushmeldingen (verzonden naar mobiele apparaten als u wordt genoemd, een bericht ontvangt in uw postvak, enzovoort.)
- Pop-up op bureaublad (wanneer u de Yammer-bureaubladapp hebt geïnstalleerd, krijgen gebruikers meldingen die 'toast'-meldingen worden genoemd.)
- Belmeldingen (binnen de Yammer-website krijgen gebruikers meldingen voor verschillende gebeurtenissen te zien. Het is mogelijk dat deze meldingen niet altijd een bijbehorende e-mail- of pushmelding hebben.)

Meer [gedetailleerde informatie over meldingen](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) is beschikbaar.

**Meldingen beheren**

Gebruikers moeten hun eigen meldingen beheren. Informatie is beschikbaar op [het in- en uitschakelen van e-mail- en mobiele meldingen van Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Het is niet mogelijk voor beheerders om alle meldingen of beheermeldingen namens gebruikers uit te schakelen. Beheerders kunnen [het logo in e-mailbericht beheren en of gebruikers berichten moeten bevestigen](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) die per e-mail worden verzonden.

**E-mailmeldingen die naar een groot aantal gebruikers in uw organisatie worden verzonden**

Soms wordt een melding per e-mail door Yammer verzonden en ontvangen door veel meer gebruikers in uw organisatie dan verwacht. Dit gebeurt als een distributielijst of een ander soort niet-individueel e-mailadres wordt toegevoegd aan Yammer. Yammer weet niet in alle gevallen of een e-mailadres tot één gebruiker behoort of een e-mailadres is dat ervoor zorgt dat één e-mailbericht naar een groot aantal geadresseerden wordt gestuurd. Als dit probleem zich voordoet, moet u actie ondernemen om [de ongeldige gebruiker met dat e-mailadres te schorsen (deactiveren)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) in Yammer. 

U kunt de kans op dit probleem verkleinen door het volgende te doen:

1. [Office 365-identiteit afdwingen](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) voor Yammer.
2. Blokkeer externe afzenders voor het verzenden van e-mail naar uw organisatie of beperk afzenders tot een goedgekeurde lijst.

Als dit probleem zich voordoet:

1. Identificeer de ontvanger van het e-mailbericht, die overeen moet komen met de gebruiker in Yammer. Zo is all-in-sales@fabrikam.com een DL voor alle verkopers. Deze DL zou u kunnen identificeren aan de hand van het e-mailbericht van Yammer dat gebruikers hebben ontvangen.
2. Gebruik de functie [deactiveren (onderbreken) in de Netwerkbeheerder](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) om de gebruiker met het e-mailadres all-in-sales@fabrikam.com te schorsen. De schorsing kan ongedaan gemaakt worden en is dus veiliger dan verwijdering. De gebruiker wordt na 90 dagen automatisch verwijderd.
3. U kunt ook de [Gebruiker exporteren](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) om andere e-mailadressen te identificeren die niet aan gebruikers zijn gekoppeld en dus moeten worden opgeschort.
