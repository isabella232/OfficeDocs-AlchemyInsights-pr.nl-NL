---
title: Problemen met aanmelden bij Microsoft 365 apps
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
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744631"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Problemen met het aanmelden bij Microsoft 365-apps

Opmerking: Als u een oudere versie van Windows gebruikt (bijvoorbeeld Windows 7 SP1, Windows Server 2008 R2), gebruikt u de eenvoudige oplossing om TLS 1.2 standaard in te stellen. [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Zie Bijwerken om [TLS 1.1 en TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)in te stellen als standaardveilige protocollen in WinHTTP in Windows.

Als u aanmeldingsproblemen met Microsoft 365-apps wilt oplossen, kunt u de volgende opties op de betreffende computer proberen:  

- Zie Windows voor meer [Aanbevelingen over het oplossen van veelvoorkomende aanmeldingsproblemen](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Zie Kan [u zich niet aanmelden bij een](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail) app Office 2016 voor Mac Mac

**Tip** op Windows-machines kunnen verschillende algemene problemen met aanmelden bij Office geconstateerd en automatisch opgelost worden. Download en voer de **[Microsoft Ondersteunings- en herstelassistent](https://aka.ms/SaRA-OfficeSignInScenario)** uit om het automatische hulpprogramma te gebruiken.

**Opmerking:** Het is niet raadzaam moderne verificatie (ADAL) of WAM (Web Account Management) uit te schakelen voor het oplossen van aanmeldings- of **activeringsproblemen.** Als de fouten optreden tijdens het maken van verbinding met Microsoft 365 met Office [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 2013, moet u ervoor zorgen dat u moderne verificatie inschakelen voor Office client.

Zie voor specifieke probleemoplossingsacties:

[Verbindingsproblemen bij de aanmelding na update voor Office 2016 build 16.0.7967 op Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[U kunt zich niet aanmelden bij uw organisatieaccount, zoals Office 365, Azure of Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Problemen met niet-browser-apps oplossen die zich niet kunnen aanmelden bij Office 365, Azure of Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Herhaaldelijk gevraagd om referenties in Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)