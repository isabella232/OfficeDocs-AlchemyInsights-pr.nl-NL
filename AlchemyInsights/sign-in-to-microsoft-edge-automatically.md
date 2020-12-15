---
title: Automatisch aanmelden bij Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677234"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automatisch aanmelden bij Microsoft Edge

In Microsoft Edge wordt het standaardaccount van het besturingssysteem gebruikt om automatisch aan te melden bij een gebruiker op basis van het geconfigureerde apparaat van de gebruiker. 

Hieronder vindt u een beschrijving van de scenario's van elk type apparaatconfiguratie en van het afhankelijke gebruikersproces.

1. **Het apparaat is Hybrid/Aad-J**: deze optie is beschikbaar in Windows 10, downlevel Windows en bijbehorende server versies. Gebruikers zijn automatisch aangemeld met hun account van Azure Active Directory (AD).
2. **Het apparaat is verbonden met een domein**: deze optie is beschikbaar in Windows 10, op het niveau van Windows en de bijbehorende server versies. Standaard worden gebruikers met domeinaccounts niet automatisch aangemeld. Als u automatisch aanmelden wilt inschakelen, gebruikt u het **ConfigureOnPremisesAccountAutoSignIn** -beleid. Als u automatisch aanmelden wilt inschakelen voor gebruikers met een Azure AD-account, kunt u overwegen om hybride lid te worden van zijn of haar apparaten.
3. **Het standaardaccount van het besturingssysteem is een Microsoft-account**: deze optie is beschikbaar in Windows 10 RS3 (versie 1709, build 10.0.16299) en nieuwere versies. Het scenario doet zich waarschijnlijk niet voor op Enterprise-apparaten. Als het standaardaccount van het besturingssysteem een Microsoft-account is, wordt de gebruiker automatisch bij Microsoft Edge aangemeld met het Microsoft-account.
 
 
