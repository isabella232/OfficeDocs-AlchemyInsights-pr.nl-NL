---
title: 932 AadConnect upgraden
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766488"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="4a642-102">Azure AD Connect upgraden</span><span class="sxs-lookup"><span data-stu-id="4a642-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="4a642-103">Standaard is automatische upgrade ingeschakeld voor Azure AD Connect, waarmee u ervoor zorgen dat u de nieuwste versie uitvoert.</span><span class="sxs-lookup"><span data-stu-id="4a642-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="4a642-104">Als u de automatische upgrade-instellingen wilt verifiëren, gebruikt u de cmdlet **Get-ADSyncAutoUpgrade** in Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4a642-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="4a642-105">De cmdlet geeft een van de volgende waarden terug:</span><span class="sxs-lookup"><span data-stu-id="4a642-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="4a642-106">**Ingeschakeld**: Automatische upgrade is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="4a642-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="4a642-107">**Uitgeschakeld**: Automatische upgrade is uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="4a642-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="4a642-108">**Opgeschort**: Het systeem komt niet langer in aanmerking voor automatische upgrades.</span><span class="sxs-lookup"><span data-stu-id="4a642-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="4a642-109">U deze waarde niet configureren. Het is ingesteld door het systeem.</span><span class="sxs-lookup"><span data-stu-id="4a642-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="4a642-110">Zie [Automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4a642-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="4a642-111">Als u de nieuwste versie van [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)Azure AD Connect wilt downloaden, gaat u naar .</span><span class="sxs-lookup"><span data-stu-id="4a642-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
