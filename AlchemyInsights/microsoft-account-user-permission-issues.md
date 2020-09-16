---
title: Problemen oplossen-gebruiker is niet gevonden in de adreslijst
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725402"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Problemen oplossen-gebruiker is niet gevonden in de adreslijst

Als gebruikers in de adreslijst foutbericht ' gebruiker kan niet vinden ' wordt weergegeven, probeer het dan opnieuw.

U kunt de volgende stappen uitvoeren om het probleem op te lossen.

- Zorg ervoor dat de account die de uitnodiging voor e-mail heeft geaccepteerd, gelijk is aan het account waarmee u zich later aanmeldt. Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en u aan te melden bij de site. 

Zie [aliassen voor uw Microsoft-account beheren voor meer informatie over </a> het beheren van de microsoft 365-aanmelding](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)voor meer informatie. 

- Blader naar een of meer sites waarbij de gebruiker de fout ontvangt. 

U kunt "/_layouts/15/people.aspx/membershipgroupid = 0" (binnen de dubbele aanhalingstekens) toevoegen aan het einde van de URL van de site. 

Voorbeeld: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecteer de gebruiker in de lijst.

- Klik op **Gebruikersmachtigingen verwijderen** op het lint. 
-  De gebruiker opnieuw toevoegen en de uitnodiging opnieuw verzenden aan de gebruiker.

