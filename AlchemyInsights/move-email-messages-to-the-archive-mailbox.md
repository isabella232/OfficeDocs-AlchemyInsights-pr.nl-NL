---
title: E-mailberichten naar de archiefmap Postvak verplaatsen
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941699"
---
Problemen bij het archiveren van items in de postbus archiveren. Zorg ervoor dat u de volgende stappen hebt uitgevoerd:
  
1. Bevestigen dat een **postbus archiveren** is ingeschakeld. Als dit niet het geval is, stappen in [dit artikel](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) gebruiken om te schakelen van de archiefmap Postvak. 
    
2. In het beheercentrum van Exchange **Tags bewaren** onder **Beheer van de conformiteit**selecteert, een **inhouding code** maken met de actie **verplaatsen naar het archief** met de gewenste **Leeftijd vasthouden**.
    
3. Selecteer **Bewaarbeleid**in het beheercentrum van Exchange, **Bewaarbeleid** maken en uw behoud **verplaatsen naar archief** tag toevoegen aan dat beleid. 
    
4. [Het bewaarbeleid toewijzen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) aan de specifieke postbus van gebruiker. Hetzelfde beleid zullen worden toegepast op zowel de **primaire** als de **archiefmap** postvak. 
    
De postbus van gebruiker hebt nu een archiveringsbeleid items te verplaatsen naar de archiefmap Postvak. Deze zijn nodig om de beheerde map-assistent (MVR gesloten) uit te voeren en de nieuwe instellingen toepassen op het postvak van de gebruiker. Voer de volgende opdracht [verbonden met EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tijdens het starten van de beheerde map-assistent van een bepaalde postbus: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Wilt u meer informatie over het instellen van een archiveringsbeleid, kunt u [een beleid voor archiveren en verwijderen van postbussen instellen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

