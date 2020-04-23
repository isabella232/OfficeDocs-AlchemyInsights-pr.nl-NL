---
title: 932 AadConnect upgraden
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766488"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect upgraden

Standaard is automatische upgrade ingeschakeld voor Azure AD Connect, waarmee u ervoor zorgen dat u de nieuwste versie uitvoert. Als u de automatische upgrade-instellingen wilt verifiëren, gebruikt u de cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell. De cmdlet geeft een van de volgende waarden terug:

- **Ingeschakeld**: Automatische upgrade is ingeschakeld.

- **Uitgeschakeld**: Automatische upgrade is uitgeschakeld.

- **Opgeschort**: Het systeem komt niet langer in aanmerking voor automatische upgrades. U deze waarde niet configureren. Het is ingesteld door het systeem.

Zie [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)voor meer informatie.

Als u de nieuwste versie van [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Azure AD Connect wilt downloaden, gaat u naar .
