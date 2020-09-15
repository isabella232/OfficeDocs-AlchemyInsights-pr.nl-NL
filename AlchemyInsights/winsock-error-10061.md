---
title: 1554 Winsock-fout 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698857"
---
# <a name="winsock-error-10061"></a>Winsock-fout 10061

Deze foutcode betekent dat Microsoft geen TCP-socket (verbinding) met de target-host kon maken. De meest waarschijnlijke oorzaak van deze fout is een probleem met de firewallconfiguratie. Ga als volgt te werk om het probleem op te lossen:

- De firewallconfiguratie controleren met de gegevens in [url's en IP-adresbereiken voor Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Als de fout specifiek is voor Exchange Online Protection (EOP), moet u eerder op de hoogte zijn van een wijziging in de [IP-adressen voor Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Controleer of uw internetprovider (ISP) de poort niet blokkeert.

- Controleer de instellingen voor de Smart host en de doelserver in de connectors.

Houd er rekening mee dat Microsoft 365 *binnenkomende* verbindingen op deze manier niet blokkeert.
