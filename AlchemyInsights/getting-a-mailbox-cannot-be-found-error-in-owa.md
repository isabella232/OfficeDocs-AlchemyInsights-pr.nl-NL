---
title: 126 Het verkrijgen van een postvak kan niet worden gevonden fout in OWA?
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
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426657"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Krijgt u een foutbericht voor een postvak dat niet is gevonden in de webversie van Outlook?

Als u de webversie van Outlook  gebruikt en een postvak niet kan worden gevonden voor fout, heeft het account dat u hebt gebruikt om verbinding te maken met de webversie van Outlook geen Exchange Online-licentie en is er daarom geen postvak gekoppeld aan het account. Uw beheerder kan een licentie aan uw account toewijzen door de volgende stappen uit te voeren:

1. Open het [Microsoft 365-beheercentrum](https://portal.office.com/adminportal/home#/homepage) en  ga naar **Actieve** gebruikers onder de sectie Gebruikers en selecteer de gebruiker die de fout ziet.

2. Ga op de pagina van de gebruiker die wordt geopend  naar de sectie Licenties en apps, selecteer de juiste locatiewaarde en **wijs** een licentie toe die Exchange Online bevat (vouw de licentie uit om de details ervan te zien). Wanneer u gereed bent, klikt u op **Wijzigingen opslaan**.

Als de licentie al aan een gebruikersaccount is toegewezen, helpt het verwijderen en opnieuw toewijzen van de licentie in sommige gevallen om het probleem op te lossen en correct in te stellen in het systeem: 

- Controleer of uw M365 Exchange Online -abonnementen (en andere, als u er al bent) actueel zijn en nog niet onlangs zijn verlopen.

Nadat u ervoor hebt zorgen dat uw abonnement niet is verlopen en er een geldige licentie is toegewezen aan het gebruikersaccount, kan het tot 24 uur duren voordat de licentie is ingericht, zodat u mogelijk moet wachten totdat het probleem is opgelost. Zie Licenties toewijzen [en beheren voor meer informatie.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)