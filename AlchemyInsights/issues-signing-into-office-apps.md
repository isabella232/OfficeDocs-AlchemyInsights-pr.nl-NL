---
title: Problemen met aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709101"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="7d4cd-102">Fix the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span><span class="sxs-lookup"><span data-stu-id="7d4cd-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="7d4cd-103">Probeer het volgende om deze fout op te lossen:</span><span class="sxs-lookup"><span data-stu-id="7d4cd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="7d4cd-104">Installeer de meest recente updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="7d4cd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7d4cd-105">[Office-referenties leeg te maken](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) met Windows Referentiebeheer.</span><span class="sxs-lookup"><span data-stu-id="7d4cd-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7d4cd-106">**Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0.</span><span class="sxs-lookup"><span data-stu-id="7d4cd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7d4cd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7d4cd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="7d4cd-108">Probeer het [gebruikersherstelproces om](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) fouten in de TPM (Trusted Platform Module) op te lossen.</span><span class="sxs-lookup"><span data-stu-id="7d4cd-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="7d4cd-109">Stel enableADAL = 0 in door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="7d4cd-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="7d4cd-110">Klik met de rechtermuisknop op de startknop van Windows, kies **Uitvoeren,** typ **regedit** en kies **OK.**</span><span class="sxs-lookup"><span data-stu-id="7d4cd-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="7d4cd-111">Selecteer **Ja om** toe te staan dat de Register-editor wijzigingen aan uw apparaat aan kan brengen.</span><span class="sxs-lookup"><span data-stu-id="7d4cd-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="7d4cd-112">Voeg in de Register-editor de DWORD-waarde van **EnableADAL** toe met de instelling **0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="7d4cd-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="7d4cd-113">Zie Verbindingsproblemen bij het aanmelden na een update naar [Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="7d4cd-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>