---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806034"
---
# <a name="upgrade-azure-ad-connect"></a>Azure AD Connect upgraden

Automatisch upgraden is standaard ingeschakeld voor Azure AD Connect, zodat u kunt controleren of u de nieuwste versie gebruikt. Als u de instellingen voor automatische upgrade wilt controleren, gebruikt u de cmdlet **Get-ADSyncAutoUpgrade** in azure AD Powershell. Met de cmdlet wordt een van de volgende waarden geretourneerd:

- **Ingeschakeld**: automatische upgrade is ingeschakeld.

- **Uitgeschakeld**: automatische upgrade is uitgeschakeld.

- **Opgeschort**: het systeem is niet meer in aanmerking voor het ontvangen van automatische upgrades. U kunt deze waarde niet configureren. Dit is ingesteld door het systeem.

Zie voor meer informatie [automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Als u de meest recente versie van Azure AD Connect wilt downloaden, gaat u naar [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
