---
title: Problemen bij het samenvoegen van VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884978"
---
# <a name="issue-joining-vms"></a>Problemen bij het samenvoegen van VMs

Voer de volgende stappen uit als u problemen wilt oplossen die zich voordoen tijdens het bijwonen van Vm's.

1. Probeer u aan te melden met de **UPN** -indeling (bijvoorbeeld ' joeuser@contoso.com ') in plaats van de **SAMAccountName** -indeling (' CONTOSO\joeuser ').
2. Zorg ervoor dat u Wachtwoordsynchronisatie hebt ingeschakeld in overeenstemming met de stappen die worden beschreven in de handleiding *aan* de slag.
3. Zorg ervoor dat het desbetreffende gebruikersaccount geen extern account is in de Azure AD-Tenant. Externe gebruikers kunnen zich niet aanmelden bij het beheerde domein, aangezien Azure AD Domain Services geen referenties hebben voor dergelijke gebruikersaccounts.
4. Als het desbetreffende gebruikersaccount een gebruikersaccount van de Cloud is, moet u ervoor zorgen dat gebruikers hun wachtwoord wijzigen nadat u Azure AD Domain Services hebt ingeschakeld. Met deze stap worden de referenties voor de referenties van Azure AD Domain Services gegenereerd.
5. Als de desbetreffende gebruikersaccounts worden gesynchroniseerd vanuit een on-premises adreslijst, controleert u of de aanbevolen versie van Azure AD Connect is geconfigureerd om een volledige synchronisatie uit te voeren.
6. Als het probleem zich blijft voordoen nadat u stap 4 hebt bevestigd, voert u de volgende opdrachten uit op uw synchronisatie computer:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.