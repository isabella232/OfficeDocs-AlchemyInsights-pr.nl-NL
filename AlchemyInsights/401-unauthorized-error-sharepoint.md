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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539927"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="637c7-102">401 Niet-geautoriseerde fout in SharePoint</span><span class="sxs-lookup"><span data-stu-id="637c7-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="637c7-103">Als u de fout '(401) Ongeautoriseerd' in SharePoint wordt weergegeven, kan dit verband houden met de intrekking van TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="637c7-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="637c7-104">Zie voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="637c7-104">For more info, see:</span></span>

- [<span data-ttu-id="637c7-105">Voorbereiden op TLS 1.2 in Office 365 en Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="637c7-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="637c7-106">Verificatiefouten treden op als client geen TLS 1.2-ondersteuning heeft</span><span class="sxs-lookup"><span data-stu-id="637c7-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="637c7-107">Bijwerken om TLS 1.1 en TLS 1.2 in te stellen als standaardveilige protocollen in WinHTTP in Windows</span><span class="sxs-lookup"><span data-stu-id="637c7-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="637c7-108">Als gebruikers zich op Windows 7 bevinden, controleert u [of ze TLS Cipher Suites in](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .</span><span class="sxs-lookup"><span data-stu-id="637c7-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>