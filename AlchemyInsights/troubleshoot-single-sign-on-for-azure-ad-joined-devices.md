---
title: Problemen met eenmalig aanmelden oplossen voor azure AD-apparaten die lid zijn van Azure AD
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035466"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Problemen met eenmalig aanmelden oplossen voor azure AD-apparaten die lid zijn van Azure AD

Als u een on-premises Ad-omgeving (Active Directory) hebt en u wilt deelnemen aan uw ad-domeincomputers met Azure AD, kunt u dit doen door hybride Azure AD-join te doen. [How To: Plan your hybrid Azure Active Directory join implementation provides](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) you with the related steps to implement a hybrid Azure AD join in your environment.

Zie Azure [AD-apparaten configureren voor on-premises](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)apparaten Single-Sign Windows Hello voor Bedrijven gebruiken voor meer informatie.

**PrT-problemen (Primary Refresh Token)**

Een prt (Primary Refresh Token) is een belangrijk artefact van Azure AD-verificatie op Windows 10-, Windows Server 2016- en latere versies, iOS- en Android-apparaten. Het is een JSON Web Token (JWT) die speciaal is uitgegeven aan microsoft first party token brokers om single sign-on (SSO) in te stellen voor de toepassingen die op deze apparaten worden gebruikt. Zie Wat is een primaire [vernieuwings-token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)voor meer informatie over hoe een PRT wordt uitgegeven, gebruikt en beveiligd op Windows 10-apparaten.

**WamDefaultSet: JA en AzureADPrt: JA**

Deze velden geven aan of de gebruiker zich bij het aanmelden bij het apparaat heeft geverifieerd bij Azure AD. Als de waarden **NEE zijn,** kan dit het gevolg zijn van:

- Slechte opslagsleutel in de TPM die bij registratie aan het apparaat is gekoppeld (controleer de KeySignTest tijdens het uitvoeren van verhoogde waarden)
- Alternatieve aanmeldings-id
- HTTP-proxy niet gevonden

Zie [SSO-status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)als u problemen wilt oplossen met de opdracht dsregcmd.
