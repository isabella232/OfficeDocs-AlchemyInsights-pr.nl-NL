---
title: Single-Sign voor apparaten met azure Active Directory-apparaten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404590"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Eén aanmelding voor azure Active Directory-apparaten

Als u een on-premises Ad-omgeving (Active Directory) hebt en u wilt deelnemen aan uw ad-domeincomputers met Azure AD, kunt u dit doen door hybride Azure AD-join te doen. [How To: Plan your hybrid Azure Active Directory join implementation provides](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) you with the related steps to implement a hybrid Azure AD join in your environment.

[Azure AD-apparaten configureren voor on-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**PrT-problemen (Primary Refresh Token)** Een prt (Primary Refresh Token) is een belangrijk artefact van Azure AD-verificatie op Windows 10-, Windows Server 2016- en latere versies, iOS- en Android-apparaten. Het is een JSON Web Token (JWT) die speciaal is uitgegeven aan microsoft first party token brokers om single sign-on (SSO) in te stellen voor de toepassingen die op deze apparaten worden gebruikt. [In Wat is een primaire vernieuwings-token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)geven we informatie over hoe een PRT wordt uitgegeven, gebruikt en beveiligd op Windows 10-apparaten.

**WamDefaultSet: JA en AzureADPrt: JA** Deze velden geven aan of de gebruiker zich bij het aanmelden bij het apparaat heeft geverifieerd bij Azure AD. Als de waarden **NEE zijn,** kan dit een gevolg zijn:

- Slechte opslagsleutel in de TPM die bij registratie aan het apparaat is gekoppeld (controleer de KeySignTest tijdens het uitvoeren van verhoogde waarden).
- Alternatieve aanmeldings-id
- HTTP-proxy niet gevonden

Problemen met apparaten oplossen met de opdracht dsregcmd - [status SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
