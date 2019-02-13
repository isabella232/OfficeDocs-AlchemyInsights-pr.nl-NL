---
title: Winsock-fout 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903091"
---
# <a name="winsock-error-10061"></a>Winsock-fout 10061

Deze foutcode betekent dat Office 365 een TCP-socket (verbinding) met de doelhost niet kan vaststellen. De meest waarschijnlijke oorzaak van deze fout is een probleem met de configuratie van de firewall. Probleem wilt oplossen, moet u deze instellingen controleren:
  
- Controleer of de configuratie van de firewall met de gegevens in [Office 365-URL's en IP-adresbereiken](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Als de fout specifiek naar Exchange Online bescherming (EOP), moet u zijn eerder aangemeld op een wijziging in de [Exchange Online bescherming IP-adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Controleer of dat de poort is niet worden geblokkeerd door uw Internet Service Provider (ISP).
    
- Controleer of de smart host- en server-instellingen in uw verbindingslijnen.
    
Houd er rekening mee dat Office 365 *binnenkomende* verbindingen op deze manier niet blokkeren. 
  

