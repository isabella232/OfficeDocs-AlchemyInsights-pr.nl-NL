---
title: UPN-synchronisatie uitgeschakeld
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782146"
---
# <a name="upn-sync-disabled"></a>UPN-synchronisatie uitgeschakeld

Als u vóór 30 maart 2016 bent begonnen met synchroniseren met Azure AD, moet u de volgende Azure AD PowerShell-cmdlet uitvoeren om alleen UPN-softmatch voor uw organisatie in te stellen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN soft match wordt automatisch ingeschakeld voor organisaties die zijn begonnen met synchroniseren met Azure AD op of na 30 maart 2016.
  
Zie Synchronisatiefuncties voor Azure AD Connect voor meer informatie over het inschakelen van soft match op UPN en andere [synchronisatiefuncties.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

