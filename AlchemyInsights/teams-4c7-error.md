---
title: Fout teams 4c 7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796056"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c 7 fout in Microsoft teams

Deze fout treedt op omdat Microsoft teams Forms-verificatie vereist. Wanneer u Active Directory Federation Services (AD FS) implementeert, is Forms-verificatie niet standaard ingeschakeld voor het intranet. Als geïntegreerde Windows-verificatie mislukt, wordt u gevraagd u aan te melden met behulp van Forms-verificatie.

Dit probleem oplossen door Forms-verificatie inschakelen met behulp van de AD FS-module van Microsoft Management Console (MMC) op de computer met de lokale kopie van Active Directory. Volg deze stappen om dit te doen: 

1. Blader in het navigatiedeelvenster naar **verificatiebeleid**.
2. Onder **acties** in het detailvenster, selecteer **globale primaire verificatie bewerken**.
3. Selecteer op het tabblad **intranet** **Forms-verificatie**.
4. Selecteer **OK** (of **toepassen**).