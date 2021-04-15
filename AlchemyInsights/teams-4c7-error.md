---
title: Fout in Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786664"
---
# <a name="4c7-error-in-microsoft-teams"></a>4c7-fout in Microsoft Teams

Deze fout treedt op omdat Voor Microsoft Teams Forms-verificatie is vereist. Wanneer u Active Directory Federation Services (AD FS) implementeert, is Forms Authentication standaard niet ingeschakeld voor het intranet. Als Windows Integrated Authentication mislukt, wordt u gevraagd u aan te melden met Forms Authentication.

Als u dit probleem wilt oplossen, schakelt u Forms Authentication in met behulp van de MMC-module (AD FS Microsoft Management Console) op de computer met de lokale kopie van Active Directory. Ga hiervoor als volgt te werk: 

1. Blader in het navigatiedeelvenster naar **Verificatiebeleid.**
2. Selecteer **onder Acties** in het detailvenster de optie Globale primaire verificatie **bewerken.**
3. Selecteer op **het tabblad Intranet** de optie **Formulierenverificatie**.
4. Selecteer **OK** (of **Toepassen).**