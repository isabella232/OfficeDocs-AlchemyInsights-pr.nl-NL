---
title: 932 upgrade AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806034"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="30a9b-102">Azure AD Connect upgraden</span><span class="sxs-lookup"><span data-stu-id="30a9b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="30a9b-103">Automatisch upgraden is standaard ingeschakeld voor Azure AD Connect, zodat u kunt controleren of u de nieuwste versie gebruikt.</span><span class="sxs-lookup"><span data-stu-id="30a9b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="30a9b-104">Als u de instellingen voor automatische upgrade wilt controleren, gebruikt u de cmdlet **Get-ADSyncAutoUpgrade** in azure AD Powershell.</span><span class="sxs-lookup"><span data-stu-id="30a9b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="30a9b-105">Met de cmdlet wordt een van de volgende waarden geretourneerd:</span><span class="sxs-lookup"><span data-stu-id="30a9b-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="30a9b-106">**Ingeschakeld**: automatische upgrade is ingeschakeld.</span><span class="sxs-lookup"><span data-stu-id="30a9b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="30a9b-107">**Uitgeschakeld**: automatische upgrade is uitgeschakeld.</span><span class="sxs-lookup"><span data-stu-id="30a9b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="30a9b-108">**Opgeschort**: het systeem is niet meer in aanmerking voor het ontvangen van automatische upgrades.</span><span class="sxs-lookup"><span data-stu-id="30a9b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="30a9b-109">U kunt deze waarde niet configureren. Dit is ingesteld door het systeem.</span><span class="sxs-lookup"><span data-stu-id="30a9b-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="30a9b-110">Zie voor meer informatie [automatische upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="30a9b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="30a9b-111">Als u de meest recente versie van Azure AD Connect wilt downloaden, gaat u naar [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="30a9b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
