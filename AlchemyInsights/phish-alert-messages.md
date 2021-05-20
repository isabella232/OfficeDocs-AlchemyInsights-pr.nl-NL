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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544573"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mailberichten waarschuwen vanuit het beleid 'Phish Delivered due to tenant or user override'

Er is een standaardwaarschuwingsbeleid met de naam 'Phish Delivered due to tenant or user override' uitgerold naar tenants met Microsoft Defender voor Office 365 P1- en P2-licenties. Als u deze waarschuwing hebt ontvangen, volgen de volgende stappen om dit te onderzoeken:

1. Klik in het waarschuwingsbericht op **Waarschuwing weergeven om** naar de pagina **Waarschuwingen** te gaan in & Compliancecentrum.

2. Selecteer de waarschuwing om de optie Berichtenlijst weergeven **of** **Berichten weergeven in Verkenner te zien.** Beide opties brengen u naar de details van het bericht, inclusief de bericht-id. Houd er rekening mee dat de koppeling Threat Explorer automatisch de berichten filtert die voldoen aan de waarschuwingscriteria. Mogelijk moet u het datumfilter in Threat Explorer aanpassen.

Het phishingbericht is bezorgd vanwege een handmatig geconfigureerde override:

- Een toegestane afzender of domein die door de gebruiker is ingesteld.

- Een toegestane afzender of domein die door de beheerder is ingesteld in een antispambeleid.

- Een toegestaan IP-adres in een verbindingsfilterbeleid.

- Een regel voor de e-mailstroom (ook wel een transportregel genoemd) die is geconfigureerd om berichten toe te staan.

Als u denkt dat het bericht ten onrechte is gemarkeerd als phish, gebruikt u de invoeg Outlook [Rapportbericht](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) om berichtvoorbeelden in te dienen bij Microsoft.
