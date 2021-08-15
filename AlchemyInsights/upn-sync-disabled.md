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
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038107"
---
# <a name="upn-sync-disabled"></a>UPN-synchronisatie uitgeschakeld

Als u vóór 30 maart 2016 bent begonnen met synchroniseren met Azure AD, moet u de volgende Azure AD PowerShell-cmdlet uitvoeren om alleen UPN-softmatch voor uw organisatie in te stellen:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN soft match wordt automatisch ingeschakeld voor organisaties die zijn begonnen met synchroniseren met Azure AD op of na 30 maart 2016.
  
Zie Azure AD Verbinding maken sync servicefuncties voor meer informatie over het inschakelen van soft match op UPN en andere [synchronisatiefuncties.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

