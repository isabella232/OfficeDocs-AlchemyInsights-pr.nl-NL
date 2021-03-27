---
title: Handmatig aanmelden bij Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398652"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Handmatig aanmelden bij Microsoft Edge

Als een gebruiker niet automatisch is aangemeld tijdens een eerste gebruikservaring, kan de gebruiker zich handmatig aanmelden via de instellingen van de browser of de flyout voor identiteiten. Als u aanmelding wilt beheren, gebruikt u het volgende beleid:

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - Om ervoor te zorgen dat een gebruiker altijd een werkprofiel heeft in Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - Om aanmelding te beperken tot een set vertrouwde accounts.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) : aanmelding uitschakelen of gebruikers dwingen zich aan te melden.

