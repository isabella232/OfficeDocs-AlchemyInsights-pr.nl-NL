---
title: 1554 Winsock fout 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766164"
---
# <a name="winsock-error-10061"></a>Winsock fout 10061

Deze foutcode betekent dat Microsoft geen TCP-socket (verbinding) met de doelhost kan maken. De meest waarschijnlijke oorzaak van deze fout is een probleem met uw firewallconfiguratie. Als u het probleem wilt oplossen, controleert u de volgende instellingen:

- Uw firewallconfiguratie verifiëren met de gegevens in [Microsoft 365-URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Als de fout specifiek is voor Exchange Online Protection (EOP), moet u eerder op de hoogte zijn gesteld van een wijziging van de [IP-adressen van Exchange Online Protection.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Controleer of uw internetserviceprovider (ISP) de poort niet blokkeert.

- Controleer de instellingen voor slimme host en doelserver in uw connectors.

Houd er rekening mee dat Microsoft 365 *inkomende* verbindingen op deze manier niet blokkeert.
