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
# <a name="upn-sync-disabled"></a><span data-ttu-id="aab14-102">UPN-synchronisatie uitgeschakeld</span><span class="sxs-lookup"><span data-stu-id="aab14-102">UPN sync disabled</span></span>

<span data-ttu-id="aab14-103">Als u bent begonnen met synchroniseren met Azure AD vóór 30 maart 2016, voert u de volgende Azure AD PowerShell-cmdlet uit om alleen UPN-overeenkomsten voor uw organisatie in te schakelen:</span><span class="sxs-lookup"><span data-stu-id="aab14-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="aab14-104">**Set-MsolDirSyncFeature-feature EnableSoftMatchOnUpn-$True inschakelen**</span><span class="sxs-lookup"><span data-stu-id="aab14-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="aab14-105">Voor organisaties die zijn gesynchroniseerd met Azure AD op of na 30 maart 2016 wordt automatisch een UPN-overeenkomst ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="aab14-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="aab14-106">Zie de functies van de [Azure AD Connect-synchronisatieservice](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)voor meer informatie over het inschakelen van vloeiend zoeken voor UPN en andere synchronisatiefuncties.</span><span class="sxs-lookup"><span data-stu-id="aab14-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

