---
title: Probleem oplossen - Gebruiker niet gevonden in directory
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702733"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Probleem oplossen - Gebruiker niet gevonden in directory

Als gebruikers een foutbericht 'gebruiker kan niet niet worden gevonden' in de map ontvangen, probeert u het opnieuw waar het type probleem gebruiker niet in de map is.

De volgende stappen kunnen worden voltooid om het probleem op te lossen.

- Zorg ervoor dat het account dat de e-mailuitnodiging heeft geaccepteerd, hetzelfde account is dat wordt gebruikt om later in te loggen. Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en u aan te melden bij de site. 

Zie [Aliassen beheren voor</a> uw Microsoft-account om de Microsoft 365-aanmelding te beheren voor](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)meer informatie. 

- Blader naar elke site(s) waarin de gebruiker de fout ontvangt. 

Voeg "/_layouts/15/people.aspx/membershipgroupid=0" (binnen de dubbele aanhalingstekens) toe aan het einde van de SITE-URL. 

Voorbeeld: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Selecteer de gebruiker in de lijst.

- Klik **op Gebruikersmachtigingen verwijderen** van het lint. 
-  Voeg de gebruiker terug en stuur de uitnodiging opnieuw naar de gebruiker.

