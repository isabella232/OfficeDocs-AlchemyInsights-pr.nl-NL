---
title: UPN-synchronisatie uitgeschakeld
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726099"
---
# <a name="upn-sync-disabled"></a>UPN-synchronisatie uitgeschakeld

Als u voor 30 maart 2016 bent begonnen met synchroniseren met Azure AD, voert u de volgende Azure AD PowerShell-cmdlet uit om upn-softmatch alleen voor uw organisatie in te schakelen:
  
 **Set-MsolDirSyncFeature -Functie EnableSoftMatchOnUpn -Inschakelen $True**
  
UPN soft match is automatisch ingeschakeld voor organisaties die op of na 30 maart 2016 zijn begonnen met synchroniseren met Azure AD.
  
Zie [Azure AD Connect-synchronisatieservicefuncties](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)voor meer informatie over het inschakelen van soft match op UPN en andere synchronisatiefuncties.
  

