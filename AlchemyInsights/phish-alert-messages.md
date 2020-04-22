---
title: 2491 Waarschuwingse-mailberichten van het beleid 'Phish Delivered due to tenant or user override'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758903"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>E-mailberichten waarschuwen van het beleid 'Phish Delivered due to tenant or user override'

Er is een standaardwaarschuwingsbeleid met de naam 'Phish Delivered due to tenant or user override' uitgerold naar tenants met Office 365 ATP P1- en P2-licenties. Als u deze waarschuwing hebt ontvangen, zijn de stappen die u moet onderzoeken:

1. Klik in het waarschuwingsbericht op **Waarschuwing weergeven** om naar de pagina **Waarschuwingen** in het beveiligings- & Compliance Center te gaan.

2. Selecteer de waarschuwing om de optie te zien om **de berichtenlijst** weer te geven of **Berichten weer geven in Explorer**. Beide opties brengen u naar de details van het bericht, waaronder de Message ID. Houd er rekening mee dat de koppeling Threat Explorer automatisch de berichten filtert die overeenkomen met de waarschuwingscriteria. Mogelijk moet u het datumfilter in Threat Explorer aanpassen.

Het phishingbericht is bezorgd vanwege een handmatig geconfigureerde overschrijving:

- Een toegestane afzender of domein ingesteld door de gebruiker.

- Een toegestane afzender of domein die door de beheerder is ingesteld in een antispambeleid.

- Een toegestaan IP-adres in een verbindingsfilterbeleid.

- Een regel voor e-mailstroom (ook wel transportregel genoemd) die is geconfigureerd om berichten toe te laten.

Als u van mening bent dat het bericht onjuist is gemarkeerd als phish, gebruikt u de [invoegtoepassing Outlook-rapportbericht](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) om berichtvoorbeelden naar Microsoft in te dienen.
