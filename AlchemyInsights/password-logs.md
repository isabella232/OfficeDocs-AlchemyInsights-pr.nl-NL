---
title: Wachtwoordlogboeken
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525141"
---
# <a name="password-logs"></a>Wachtwoordlogboeken

**Ik heb problemen met het openen van auditlogboeken voor het opnieuw instellen van wachtwoorden**

Voer de volgende stap uit om problemen met betrekking tot toegang tot auditlogboeken voor wachtwoord opnieuw instellen op te lossen:

Controleer of u bevoegd bent om auditlogboeken weer te geven. 

Alleen de volgende rollen zijn geautoriseerd:
 - Globale beheerder
 - Beveiligingsbeheerder
 - Beveiligingslezer

**Ik wil alle auditgebeurtenissen voor het opnieuw instellen van wachtwoorden zien vanaf het moment dat ik ze in eerste instantie heb geïmplementeerd**

Er worden maximaal 120.000 gebeurtenissen voor wachtwoord opnieuw instellen/registratie opgeslagen in de rapporten van de afgelopen 30 dagen. Deze maximumlimiet is van toepassing op de gebruikersinterface bij het downloaden van de CSV. Er zijn 1 miljoen gebeurtenissen beschikbaar via PowerShell.
Zie de onderstaande koppelingen voor meer informatie:

- [Selfservice voor wachtwoordresetgebeurtenissen vanuit de Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Registratiegebeurtenissen voor wachtwoord opnieuw instellen snel downloaden met PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Ik wil meer weten over de rapportagemogelijkheden voor wachtwoord opnieuw instellen**

Controleer wie zich registreert voor wachtwoorden of stel deze opnieuw in met auditlogboeken voor het opnieuw instellen van wachtwoorden voor Azure AD in de Azure Portal onder **Gebruikers en groepen.**
Zie de volgende koppelingen voor meer informatie:

- [Overzicht van rapporten voor wachtwoord opnieuw instellen](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Rapporten over het opnieuw instellen van wachtwoorden weergeven in de Azure Portal](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Selfservice voor wachtwoordresetgebeurtenissen vanuit de Azure AD Reports and Events API](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Registratiegebeurtenissen voor wachtwoord opnieuw instellen snel downloaden met PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


