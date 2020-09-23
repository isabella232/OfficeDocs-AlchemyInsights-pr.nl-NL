---
title: 726 blokkeert het doorsturen van e-mail
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219850"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Doorsturen van e-mail blokkeren of de blokkering opheffen

Zie [doorsturen van E-mail configureren](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)om het doorsturen van e-mail voor een specifiek postvak in of uit te schakelen.

Op het tenantniveau wordt de besturing van extern doorsturen uitgevoerd met behulp van het uitgaande antispambeleid. Als de instelling op uit of automatisch is ingesteld, kan het doorsturen van e-mail blokkeren met de fout ' 550 5.7.520 toegang geweigerd ' wordt niet toegestaan dat uw organisatie de fout externe forwarding toestaat '. Als doorsturen is ingesteld op geblokkeerd, is dit de fout die uw gebruikers te zien krijgen.

Als het doorsturen wordt geblokkeerd, controleert u of het beleid is geconfigureerd voor het inschakelen van extern doorsturen. U kunt het uitgaande spam filter beleid controleren vanuit beveiligings-en compliance Center, of door opdracht Get-HostedOutboundSpamFilterPolicy | FL name, AutoForwardingMode. Als u de optie voor het doorsturen van e-mail wilt instellen, krijgt u de status van beleid nu te zien.

Opmerking: het wordt aanbevolen dat u de functie voor extern doorsturen uitgeschakeld laat voor het standaardbeleid voor uitgaande spam filters en dit alleen inschakelen voor de gebruikers die extern doorsturen willen maken door een aangepast beleid te maken voor deze gebruikers. Meer informatie vindt u in [externe e-mail forwarding configureren in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).