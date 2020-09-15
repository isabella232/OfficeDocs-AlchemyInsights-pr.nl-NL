---
title: 4c7 fout in teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700198"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fout in Microsoft teams

Deze fout treedt op omdat Microsoft teams formulierverificatie vereist. Wanneer u Active Directory Federation Services (AD FS) implementeert, wordt formulierverificatie niet standaard ingeschakeld voor het intranet. Als Windows Integrated Authentication mislukt, wordt u gevraagd u aan te melden met behulp van formulierverificatie.

U kunt dit probleem oplossen door formulierverificatie in te schakelen via de MMC (Microsoft Management Console) van de Microsoft Management Console op de computer met de lokale kopie van Active Directory. Ga hiervoor als volgt te werk: 

1. Blader in het navigatiedeelvenster naar **verificatiebeleid**.
2. Selecteer onder **acties** in het detailvenster de optie **globale primaire verificatie bewerken**.
3. Selecteer op het tabblad **intranet** de optie **formulierverificatie**.
4. Selecteer **OK** (of **toepassen**).