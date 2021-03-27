---
title: Meld u automatisch aan bij Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398724"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Meld u automatisch aan bij Microsoft Edge

Microsoft Edge gebruikt het standaardaccount van het besturingssysteem om automatisch een gebruiker aan te melden op basis van de configuratie van het apparaat van de gebruiker. 

De scenario's van elk type apparaatconfiguratie en het afhankelijke aanmeldingsproces van de gebruiker worden hieronder beschreven:

- **Het apparaat is hybride/AAD-J:** Deze optie is beschikbaar in Windows 10, windows op lager niveau en bijbehorende serverversies. Gebruikers worden automatisch aangemeld met hun Ad-accounts (Azure Active Directory).
- **Het apparaat is domeingevoegd:** deze optie is beschikbaar in Windows 10, windows op lager niveau en bijbehorende serverversies. Gebruikers met domeinaccounts worden standaard niet automatisch aangemeld. Gebruik het beleid **ConfigureOnPremisesAccountAutoSignIn** om automatische aanmelding voor hen in te stellen. Als u automatische aanmelding wilt inschakelen voor gebruikers met Azure AD-accounts, kunt u overwegen om hybride deel te nemen aan hun apparaten.
- Het standaardaccount van het besturingssysteem is een **Microsoft-account:** deze optie is beschikbaar in Windows 10 RS3 (versie 1709, build 10.0.16299) en latere versies. Het is onwaarschijnlijk dat het scenario zich op ondernemingsapparaten voordoet. Als het standaardaccount van het besturingssysteem echter een Microsoft-account is, wordt de gebruiker automatisch door Microsoft Edge met het Microsoft-account aanmelden.
 
 
