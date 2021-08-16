---
title: S/MIME in webversie van Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010719"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailberichten versleutelen in Outlook

Microsoft 365 Berichtversleuteling is gebaseerd Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection. Als uw abonnement een Azure Rights Management of Azure Information Protection **bevat,** hoeft u geen acties uit te voeren om de Rights Management Service handmatig in te stellen of te activeren.

Op basis van feedback van klanten kunnen de regels voor Exchange e-mailstroom niet meer automatisch uitgaande e-mail versleutelen die bepaalde typen gevoelige informatie in uw tenant bevat. In plaats daarvan geven we gedetailleerde instructies over hoe u dit zelf kunt doen. Zie dit artikel voor meer informatie over het maken van een transportregel voor het versleutelen van [gevoelige informatie.](https://aka.ms/OmeEtr)

- Als u Outlook op internet gebruikt (voorheen **OWA):** Klik bij het opstellen van een e-mailbericht op Beveiligen **in** OWA. Hiermee wordt de machtiging 'Niet doorsturen' toegepast. Klik **op Machtiging wijzigen** en kies **Versleutelen** om het bericht alleen te versleutelen.

- Als u **Outlook-client**: Als u een versleuteld bericht wilt verzenden vanaf Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u Optiesmachtigingen en selecteert u vervolgens de gewenste   >  beveiligingsoptie.

- Als **u alle e-mail** die naar bepaalde geadresseerden of externe partnerorganisaties wordt verzonden, automatisch wilt versleutelen, moet u een transportregel voor e-mailstroom maken in het Exchange Beheercentrum. Gedetailleerde instructies worden in dit [ondersteuningsartikel gegeven.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

