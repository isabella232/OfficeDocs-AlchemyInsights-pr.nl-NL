---
title: UPN-synchronisatie is uitgeschakeld
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532326"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="46c4f-102">UPN-synchronisatie is uitgeschakeld</span><span class="sxs-lookup"><span data-stu-id="46c4f-102">UPN sync disabled</span></span>

<span data-ttu-id="46c4f-103">Voer de volgende Azure AD PowerShell-cmdlet UPN-zachte match voor uw organisatie alleen inschakelen als u wilt als u synchroniseren met Azure AD vóór 30 maart 2016 gestart:</span><span class="sxs-lookup"><span data-stu-id="46c4f-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="46c4f-104">**Set MsolDirSyncFeature-functie EnableSoftMatchOnUpn-$True inschakelen**</span><span class="sxs-lookup"><span data-stu-id="46c4f-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="46c4f-105">UPN-zachte match automatisch ingeschakeld voor organisaties die worden gesynchroniseerd met Azure AD op of na 30 maart 2016 is gestart.</span><span class="sxs-lookup"><span data-stu-id="46c4f-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="46c4f-106">Zie voor meer informatie over het inschakelen van zachte match op UPN en andere synchronisatiefuncties, [Azure AD verbinden sync servicefuncties](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="46c4f-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

