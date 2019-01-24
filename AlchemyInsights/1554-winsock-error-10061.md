---
title: Winsock-fout 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/24/2019
ms.locfileid: "29465417"
---
# <a name="winsock-error-10061"></a>Winsock-fout 10061

Deze foutcode betekent dat Office 365 een TCP-socket (verbinding) met de doelhost niet kan vaststellen. De meest waarschijnlijke oorzaak van deze fout is een probleem met de configuratie van de firewall. Probleem wilt oplossen, moet u deze instellingen controleren:
  
- Controleer of de configuratie van de firewall met de gegevens in [Office 365-URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Als de fout specifiek naar Exchange Online bescherming (EOP), moet u zijn eerder aangemeld op een wijziging in de [Exchange Online bescherming IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Controleer of dat de poort is niet worden geblokkeerd door uw Internet Service Provider (ISP).
    
- Controleer of de smart host- en server-instellingen in uw verbindingslijnen.
    
Houd er rekening mee dat Office 365 *binnenkomende* verbindingen op deze manier niet blokkeren. 
  

