---
title: 932 AADConnect upgraden
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858955"
---
# <a name="upgrade-azure-ad-connect"></a>Upgrade Azure AD verbinding

Automatische upgrade is standaard ingeschakeld voor Azure AD Connect, die zorgt ervoor dat u werkt met de nieuwste versie. Als u wilt controleren of de instellingen voor automatisch bijwerken, gebruikt u de cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell. De cmdlet retourneert een van de volgende waarden: 

- **Ingeschakeld**: automatisch bijwerken is ingeschakeld.

- **Uitgeschakeld**: Automatische upgrade is uitgeschakeld.

- **Onderbroken**: het systeem is niet langer in aanmerking voor automatische upgrades. U kunt niet configureren dat deze waarde; door het systeem wordt ingesteld. 

Zie [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)voor meer informatie.

Downloaden van de nieuwste versie van Azure AD verbinding maken, gaat u naar [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
