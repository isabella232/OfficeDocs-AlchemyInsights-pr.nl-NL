---
title: Google Chrome-uitbreidingen voor poorten van Microsoft Edge (chroom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677287"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="4971e-102">Google Chrome-uitbreidingen voor poorten van Microsoft Edge (chroom)</span><span class="sxs-lookup"><span data-stu-id="4971e-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="4971e-103">[Google Chrome-extensies kunt u eenvoudig overbrengen naar Microsoft Edge (chroom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="4971e-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="4971e-104">In de meeste gevallen zijn er alleen minimale wijzigingen nodig om deze extensies op Microsoft Edge uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="4971e-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="4971e-105">De Api's met extensies en de manifest Keys die worden ondersteund door Google Chrome zijn code compatibel met Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4971e-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="4971e-106">Microsoft Edge biedt echter geen ondersteuning voor de extensie Api's Chrome. GCM, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken en Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="4971e-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>