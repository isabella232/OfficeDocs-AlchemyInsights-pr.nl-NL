---
title: S/MIME in Outlook op het web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666835"
---
# <a name="encrypt-email-messages-in-outlook"></a>Codeer e-mail berichten in Outlook

Office 365-bericht versleuteling is gebaseerd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection. Als uw abonnement Azure Rights Management of Azure Information Protection bevat, **hoeft u geen acties uit te voeren om de Rights Management-service handmatig in te schakelen of te activeren** .

Op basis van feedback van klanten, zullen we niet langer inschakelen Exchange mail flow regels voor het automatisch coderen van uitgaande e-mail met een bepaald type gevoelige informatie in uw Tenant standaard. In plaats daarvan geven we gedetailleerde instructies over hoe je dat zelf doen. Zie [dit artikel](https://aka.ms/OmeEtr)voor meer informatie over het maken van een transportregel voor het versleutelen van gevoelige informatie.

- Als u Outlook op het web (voorheen **OWA**): wanneer u een e-mail bericht opstelt, klikt u op **beveiligen** in OWA. Dit is van toepassing op de machtiging ' niet doorsturen '. Klik op **machtiging wijzigen** en kies **coderen** om het bericht alleen te versleutelen.

- Als u **Outlook-client**gebruikt: als u een gecodeerd bericht wilt verzenden vanuit Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u **Opties** > **machtigingen**en selecteert u vervolgens de gewenste beveiligingsoptie.

- Als u **alle e-mail** die is verzonden naar bepaalde geadresseerden of externe partnerorganisaties automatisch wilt coderen, moet u een regel voor het transport van e-mail berichten in het Beheercentrum van Exchange maken. Gedetailleerde instructies zijn beschikbaar in [dit ondersteuningsartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

