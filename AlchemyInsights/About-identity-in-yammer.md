---
title: Over identiteit in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148197"
---
# <a name="about-identity-in-yammer"></a>Over identiteit in Yammer

Het wordt aanbevolen dat alle netwerken de volgende stappen ondernemen om identiteitsgerelateerde problemen te voorkomen:

1. Afdwingen Office 365-identiteit na het inrichten van Microsoft 365-accounts voor gebruikers in Azure AD om ervoor te zorgen dat alle gebruikers zich aanmelden met hun primaire Microsoft 365-account. Zie [Office 365-identiteit afdwingen voor Yammer-gebruikers voor](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)meer informatie.
2. Meerdere Yammer-netwerken consolideren. Met verouderde Yammer-configuraties kunnen meerdere Yammer-netwerken worden verbonden met één tenant. Zie [Netwerkmigratie - Meerdere Yammer-netwerken consolideren](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)voor meer informatie .
3. Optioneel u licenties voor Yammer afdwingen om gebruikers van Yammer te blokkeren als ze geen licentie hebben. Zie [Yammer-gebruikerslicenties beheren in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)voor meer informatie.
4. Controleer ten slotte de gebruikerslijst voor oudere Yammer-netwerken en schort oudere gebruikers op. Het wordt aanbevolen om gebruikers op te schorten (te deactiveren) in plaats van ze te verwijderen, omdat verwijdering onomkeerbaar is. Zie [Yammer-gebruikers controleren in netwerken die zijn verbonden met Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) en [Gebruikers verwijderen](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)voor meer informatie.

Als u Yammer configureert met deze stappen, u ook uw Yammer-netwerk configureren voor native modus voor Microsoft 365. Zie [Uw Yammer-netwerk configureren voor native modus voor Microsoft 365 voor](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)meer informatie.