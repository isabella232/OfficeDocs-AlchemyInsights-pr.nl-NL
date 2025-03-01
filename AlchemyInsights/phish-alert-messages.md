---
title: 2491 E-mailberichten van het beleid 'Phish Delivered due to tenant or user override'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316353"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mailberichten waarschuwen vanuit het beleid 'Phish Delivered due to tenant or user override'

Een standaardwaarschuwingsbeleid met de naam Phish Delivered vanwege tenant- of **gebruikers-overschrijven** is beschikbaar in organisaties met Microsoft Defender voor Office 365 P1- en P2-licenties. Als u deze waarschuwing hebt ontvangen, volgen de volgende stappen om dit te onderzoeken:

1. Klik in het waarschuwingsbericht op **Waarschuwing weergeven om** naar de pagina **Waarschuwingen** in de Microsoft 365 Defender gaan.

2. Selecteer de waarschuwing om de optie Berichtenlijst weergeven **of** **Berichten weergeven in Verkenner te zien.** Beide opties brengen u naar de details van het bericht, inclusief de bericht-id. Houd er rekening mee dat de koppeling Threat Explorer automatisch de berichten filtert die voldoen aan de waarschuwingscriteria. Mogelijk moet u het datumfilter in Threat Explorer aanpassen.

Het phishingbericht is bezorgd vanwege een handmatig geconfigureerde override:

- Een toegestane afzender of domein die door de gebruiker is ingesteld.
- Een toegestane afzender of domein die door de beheerder is ingesteld in een antispambeleid.
- Een toegestaan IP-adres in een verbindingsfilterbeleid.
- Een regel voor de e-mailstroom (ook wel een transportregel genoemd) die is geconfigureerd om berichten toe te staan.

Als u denkt dat het bericht onjuist is gemarkeerd als phishing, gebruikt [u](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) De inzending van beheerder om het bericht aan Microsoft te rapporteren.

Gebruikers kunnen de [invoeging Rapportbericht of](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) de invoeging Phishing melden in Outlook gebruiken om berichtvoorbeelden in te dienen bij Microsoft.
