---
title: S/MIME in de webversie van Outlook
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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772257"
---
# <a name="encrypt-email-messages-in-outlook"></a>E-mailberichten in Outlook versleutelen

Microsoft 365-bericht versleuteling is gebaseerd op Microsoft Azure Rights Management (Azure RMS), dat deel uitmaakt van Azure Information Protection. Als uw abonnement Azure Rights Management of Azure Information Protection bevat, **hoeft u geen acties te ondernemen om de Rights Management-service handmatig in te schakelen of te activeren** .

Op basis van feedback van klanten hebben we geen Exchange-e-mail stroom regels meer voor het automatisch versleutelen van uitgaande e-mail met bepaalde typen gevoelige informatie in uw Tenant. In plaats daarvan bieden we uitgebreide instructies voor hoe u dit kunt doen met beoordelen. Zie [dit artikel](https://aka.ms/OmeEtr)voor meer informatie over het maken van een transportregel voor het versleutelen van gevoelige informatie.

- Als u de webversie van Outlook (voorheen **OWA**) gebruikt, hoeft u niets **te** doen om een e-mailbericht op te stellen in OWA. Dit is van toepassing op de machtiging niet doorsturen. Klik op **machtiging wijzigen** en kies **versleutelen** als u het bericht alleen wilt versleutelen.

- Als u de **Outlook-client**gebruikt: als u een versleuteld bericht wilt verzenden vanuit Outlook 2013 of 2016 of Outlook 2016 voor Mac, selecteert u **Opties**  >  **Permissions**en selecteert u de gewenste beschermings optie.

- Als u **alle e-mail** berichten die naar bepaalde geadresseerden of externe partnerorganisaties zijn verzonden automatisch wilt versleutelen, moet u een transportregel voor de e-mail stroom maken in het Exchange-Beheercentrum. In [Dit ondersteunings artikel](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)vindt u gedetailleerde instructies.

