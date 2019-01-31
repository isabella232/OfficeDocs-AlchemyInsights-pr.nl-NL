---
title: UPN-synchronisatie is uitgeschakeld
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657966"
---
# <a name="upn-sync-disabled"></a>UPN-synchronisatie is uitgeschakeld

Voer de volgende Azure AD PowerShell-cmdlet UPN-zachte match voor uw organisatie alleen inschakelen als u wilt als u synchroniseren met Azure AD vóór 30 maart 2016 gestart:
  
 **Set MsolDirSyncFeature-functie EnableSoftMatchOnUpn-$True inschakelen**
  
UPN-zachte match automatisch ingeschakeld voor organisaties die worden gesynchroniseerd met Azure AD op of na 30 maart 2016 is gestart.
  
Zie voor meer informatie over het inschakelen van zachte match op UPN en andere synchronisatiefuncties, [Azure AD verbinden sync servicefuncties](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

