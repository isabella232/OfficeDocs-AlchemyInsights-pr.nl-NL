---
title: 2491-waarschuwingen voor e-mailberichten van het beleid ' phishing verzonden vanwege Tenant of gebruiker override '
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728606"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Waarschuwen voor e-mailberichten van het beleid ' phishing is bezorgd vanwege Tenant of gebruiker override '

Een standaard waarschuwings beleid met de naam ' phishing bezorgd vanwege Tenant of gebruiker override ' is uitgerold naar tenants met Office 365 ATP P1 en P2-licenties. Als u deze melding ontvangt, volgt u deze stappen:

1. Klik in het waarschuwingsbericht op **melding weergeven** om naar de pagina **waarschuwingen** in het beveiligings & nalevings centrum te gaan.

2. Selecteer de melding om de optie voor het **weergeven** van berichten **in Verkenner**weer te geven. Met deze opties kunt u de details van het bericht, inclusief de bericht-ID, volgen. Houd er rekening mee dat de koppeling bedreigings Verkenner automatisch de berichten filtert die voldoen aan de waarschuwingscriteria. Mogelijk moet u het datumfilter in de bedreigings Verkenner aanpassen.

Het malafide bericht is bezorgd vanwege een handmatig geconfigureerde Override:

- Een toegestane afzender of domein dat is opgegeven door de gebruiker.

- Een toegestane afzender of domein dat door de beheerder is ingesteld op een antispambeleid.

- Een toegestaan IP-adres in een beleid voor verbindings filters.

- Een e-mail stroom regel (ook wel een transportregel genoemd) die is geconfigureerd voor het toestaan van berichten in.

Als u van mening bent dat het bericht onjuist is gemarkeerd als phishing, gebruikt u de [invoegtoepassing rapportbericht](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) in Outlook om bericht voorbeelden bij Microsoft in te dienen.
