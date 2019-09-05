---
title: Probleem oplossen-gebruiker niet gevonden in map
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754187"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probleem oplossen-gebruiker niet gevonden in map

Als gebruikers ontvangen foutbericht ' gebruiker kan niet worden gevonden ' in de map. Probeer het opnieuw waar het probleem type is gebruiker niet in de map.

De volgende stappen kunnen worden voltooid om het probleem op te lossen.

- Zorg ervoor dat het account dat de e-mail uitnodiging heeft geaccepteerd hetzelfde account is dat wordt gebruikt om later aan te melden. Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en zich aan te melden bij de site. 

Zie voor meer informatie, [over het beheren van aliassen voor uw micro</a> Soft-account voor het beheren van de aanmelding bij Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Blader naar elke site (s) waarin de gebruiker de fout ontvangt. 

Voeg '/_layouts/15/people.aspx/membershipgroupid = 0 ' (binnen de dubbele aanhalingstekens) toe aan het einde van de site-URL. 

Voorbeeld: https:/_Lt_ "contoso">. SharePoint. com/_layouts/15/people. aspx/membershipGroupId = 0.

- Selecteer de gebruiker in de lijst.

- Klik op **Gebruikersmachtigingen verwijderen** uit het lint. 
-  Voeg de gebruiker terug en verzend de uitnodiging opnieuw naar de gebruiker.

