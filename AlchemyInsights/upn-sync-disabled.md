---
title: UPN-synchronisatie uitgeschakeld
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749509"
---
# <a name="upn-sync-disabled"></a>UPN-synchronisatie uitgeschakeld

Als u bent begonnen met synchroniseren met Azure AD vóór 30 maart 2016, voert u de volgende Azure AD PowerShell-cmdlet uit om alleen UPN-overeenkomsten voor uw organisatie in te schakelen:
  
 **Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-$True inschakelen**
  
Voor organisaties die zijn gesynchroniseerd met Azure AD op of na 30 maart 2016 wordt automatisch een UPN-overeenkomst ingeschakeld.
  
Zie de functies van de [Azure AD Connect-synchronisatieservice](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)voor meer informatie over het inschakelen van vloeiend zoeken voor UPN en andere synchronisatiefuncties.
  

