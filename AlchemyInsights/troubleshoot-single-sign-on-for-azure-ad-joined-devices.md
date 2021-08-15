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
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039241"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Problemen met eenmalig aanmelden oplossen voor azure AD-apparaten die lid zijn van Azure AD

Als u een on-premises Ad-omgeving (Active Directory) hebt en u wilt deelnemen aan uw ad-domeincomputers met Azure AD, kunt u dit doen door hybride Azure AD-join te doen. [How To: Plan uw hybride Azure Active Directory join-implementatie](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) biedt u de bijbehorende stappen voor het implementeren van een hybride Azure AD-join in uw omgeving.

Zie Azure [AD-apparaten configureren voor on-premises Single-Sign On-premises](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)Windows Hello voor Bedrijven voor meer informatie.

**PrT-problemen (Primary Refresh Token)**

Een prt (Primary Refresh Token) is een belangrijk artefact van Azure AD-verificatie op Windows 10, Windows Server 2016 en latere versies, iOS- en Android-apparaten. Het is een JSON Web Token (JWT) die speciaal is uitgegeven aan microsoft first party token brokers om single sign-on (SSO) in te stellen voor de toepassingen die op deze apparaten worden gebruikt. Zie Wat is een primaire [vernieuwings-token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)voor meer informatie over hoe een PRT wordt uitgegeven, gebruikt en beveiligd op Windows 10 apparaten.

**WamDefaultSet: JA en AzureADPrt: JA**

Deze velden geven aan of de gebruiker zich bij het aanmelden bij het apparaat heeft geverifieerd bij Azure AD. Als de waarden **NEE zijn,** kan dit het gevolg zijn van:

- Slechte opslagsleutel in de TPM die bij registratie aan het apparaat is gekoppeld (controleer de KeySignTest tijdens het uitvoeren van verhoogde waarden)
- Alternatieve aanmeldings-id
- HTTP-proxy niet gevonden

Zie [SSO-status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)als u problemen wilt oplossen met de opdracht dsregcmd.
