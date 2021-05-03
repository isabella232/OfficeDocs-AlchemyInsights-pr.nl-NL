---
title: Problemen met SharePoint op Windows 7 machines
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124924"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Problemen met SharePoint op Windows 7 machines

Als u fouten ontvangt op Windows 7-machines tijdens het werken aan SharePoint of OneDrive, kunnen deze zijn gerelateerd aan de intrekking van TLS 1.0/1.1. Zie voor meer informatie:

- [Voorbereiden op TLS 1.2 in Office 365 en Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 clients moet TLS1.2 zijn ingeschakeld. Zie Verificatiefouten optreden wanneer [client geen TLS 1.2-ondersteuning heeft](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support) voor meer informatie.

- Installeer KB3140245 en maak de registerwaarde. Zie Bijwerken om [TLS 1.1 en TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) in teschakelen als standaardveilige protocollen in WinHTTP in Windows

- Windows 7 SP1/Windows 8 clients moeten ervoor zorgen dat de nieuwste TLS-coderingssuites zijn geïnstalleerd. Zie [Microsoft Security Advisory 3042058 voor meer informatie.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


