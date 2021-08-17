---
title: De onderliggende verbinding is in de SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883314"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Fout 'De onderliggende verbinding is gesloten' in SharePoint

Als u de fout 'De onderliggende verbinding is gesloten' ontvangt in SharePoint is deze mogelijk gerelateerd aan de intrekking van TLS 1.0/1.1. Zie deze artikelen voor meer informatie:

- [Voorbereiden op TLS 1.2 in Office 365 en Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Verificatiefouten treden op als client geen TLS 1.2-ondersteuning heeft](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Bijwerken om TLS 1.1 en TLS 1.2 in te stellen als standaardveilige protocollen in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Als gebruikers zich op Windows 7 bevinden, controleert u [of ze TLS Cipher Suites in](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .