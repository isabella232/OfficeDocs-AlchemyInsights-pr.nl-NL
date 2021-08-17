---
title: 401 Niet-geautoriseerde fout in SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 04f56dfc7ebe7de91bc64a5e6d2b480b07741c6e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314343"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Niet-geautoriseerde fout in SharePoint

Als u de fout '(401) Ongeautoriseerd' in SharePoint wordt weergegeven, kan dit verband houden met de intrekking van TLS 1.0/1.1. Zie voor meer informatie:

- [Voorbereiden op TLS 1.2 in Office 365 en Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Verificatiefouten treden op als client geen TLS 1.2-ondersteuning heeft](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Bijwerken om TLS 1.1 en TLS 1.2 in te stellen als standaardveilige protocollen in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Als gebruikers zich op Windows 7 bevinden, controleert u [of TLS Cipher Suites in](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .