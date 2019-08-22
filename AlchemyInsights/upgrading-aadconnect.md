---
title: 932 AADConnect upgraden
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506078"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="bb181-102">Upgrade Azure AD verbinding</span><span class="sxs-lookup"><span data-stu-id="bb181-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="bb181-103">Automatische upgrade is standaard ingeschakeld voor Azure AD Connect, die zorgt ervoor dat u werkt met de nieuwste versie.</span><span class="sxs-lookup"><span data-stu-id="bb181-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="bb181-104">Als u wilt controleren of de instellingen voor automatisch bijwerken, gebruikt u de cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bb181-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="bb181-105">De cmdlet retourneert een van de volgende waarden:</span><span class="sxs-lookup"><span data-stu-id="bb181-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="bb181-106">**Ingeschakeld**: automatisch bijwerken is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="bb181-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="bb181-107">**Uitgeschakeld**: Automatische upgrade is uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="bb181-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="bb181-108">**Onderbroken**: het systeem is niet langer in aanmerking voor automatische upgrades.</span><span class="sxs-lookup"><span data-stu-id="bb181-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="bb181-109">U kunt niet configureren dat deze waarde; door het systeem wordt ingesteld.</span><span class="sxs-lookup"><span data-stu-id="bb181-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="bb181-110">Zie [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="bb181-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="bb181-111">Downloaden van de nieuwste versie van Azure AD verbinding maken, gaat u naar [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="bb181-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
