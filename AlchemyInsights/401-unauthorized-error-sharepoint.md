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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233493"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Niet-geautoriseerde fout in SharePoint

Als u de fout '(401) Ongeautoriseerd' in SharePoint wordt weergegeven, kan dit verband houden met de intrekking van TLS 1.0/1.1. Zie voor meer informatie:

[Voorbereiden op TLS 1.2 in Office 365 en Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Verificatiefouten treden op als client geen TLS 1.2-ondersteuning heeft](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Als gebruikers zich op Windows 7 bevinden, controleert u [of ze TLS Cipher Suites in](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .