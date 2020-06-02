---
title: S/MIME in de webversie van Outlook
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511503"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailberichten versleutelen in Outlook

Microsoft 365 Message Encryption is gebouwd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection. Als uw abonnement Azure Rights Management of Azure Information Protection bevat, hoeft u geen acties te ondernemen om de Rights Management Service **handmatig in te schakelen of te activeren.**

Op basis van feedback van klanten kunnen we exchange-e-mailstroomregels niet langer in staat stellen om uitgaande e-mail met bepaalde soorten gevoelige informatie in uw tenant standaard automatisch te versleutelen. In plaats daarvan geven we gedetailleerde instructies over hoe jullie dit zelf kunnen doen. Zie [dit artikel voor](https://aka.ms/OmeEtr)meer informatie over het maken van een transportregel om gevoelige informatie te versleutelen.

- Als u Outlook on the Web gebruikt (voorheen **OWA):** Wanneer u een e-mailbericht opstelt, klikt u op **Beveiligen** in OWA. Dit is van toepassing "Niet doorsturen" toestemming. Klik **op Machtiging wijzigen** en kies **Versleutelen** om alleen het bericht te versleutelen.

- Als u Outlook-client gebruikt: Als u **Outlook-client**gebruikt: Als u outlook 2013 of 2016 of Outlook 2016 voor Mac wilt verzenden: selecteert u **Options**  >  **Optiesmachtigingen**en selecteert u de beveiligingsoptie die u nodig hebt.

- Als u **alle e-mail die** naar bepaalde ontvangers of externe partnerorganisaties wordt verzonden, automatisch wilt versleutelen, moet u een regel voor e-mailstroomtransport maken in het Exchange-beheercentrum. Gedetailleerde instructies worden gegeven in [dit ondersteuningsartikel.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

