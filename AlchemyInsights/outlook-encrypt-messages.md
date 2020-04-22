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
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764867"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailberichten versleutelen in Outlook

Microsoft 365-berichtversleuteling is gebouwd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection. Als uw abonnement Azure Rights Management of Azure Information Protection bevat, hoeft u geen acties uit te voeren om de Rights Management Service **handmatig in te schakelen of te activeren.**

Op basis van feedback van klanten kunnen de Exchange-mailstroomregels niet langer automatisch uitgaande e-mail versleutelen die standaard bepaalde soorten gevoelige informatie in uw tenant bevat. In plaats daarvan geven we gedetailleerde instructies over hoe jullie dat zelf kunnen doen. Zie [dit artikel](https://aka.ms/OmeEtr)voor meer informatie over het maken van een transportregel om gevoelige informatie te versleutelen.

- Als u Outlook on the Web gebruikt (voorheen **OWA):** Klik bij het opstellen van een e-mailbericht op **Beveiligen** in OWA. Dit geldt voor "Niet doorsturen" toestemming. Klik **op Machtigingen wijzigen** en kies **Versleutelen** om het bericht alleen te versleutelen.

- Als u **Outlook-client gebruikt:** Als u outlook-client wilt gebruiken: als u een versleuteld bericht wilt verzenden vanuit Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u **Optiesmachtigingen** > **Permissions**en selecteert u de gewenste beveiligingsoptie.

- Als u **alle e-mail die** naar bepaalde ontvangers of externe partnerorganisaties wordt verzonden, automatisch wilt versleutelen, moet u een regel voor het transport van e-mailstromen maken in het Exchange-beheercentrum. Gedetailleerde instructies zijn opgenomen in [dit ondersteuningsartikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).

