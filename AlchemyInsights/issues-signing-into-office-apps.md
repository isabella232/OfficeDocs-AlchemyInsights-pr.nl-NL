---
title: Problemen met aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832998"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="5058a-102">Het bericht 'De vertrouwde platformmodule van uw computer werkt niet goed' van de Microsoft 365-apps herstellen</span><span class="sxs-lookup"><span data-stu-id="5058a-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="5058a-103">Probeer het volgende om deze fout op te lossen:</span><span class="sxs-lookup"><span data-stu-id="5058a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="5058a-104">Installeer de meest recente updates [voor Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="5058a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="5058a-105">[Office-referenties met](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windows Credential Manager uit.</span><span class="sxs-lookup"><span data-stu-id="5058a-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5058a-106">**Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0.</span><span class="sxs-lookup"><span data-stu-id="5058a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5058a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5058a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="5058a-108">Probeer het [herstelproces voor gebruikers om](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) TPM-fouten (Trusted Platform Module) op te lossen.</span><span class="sxs-lookup"><span data-stu-id="5058a-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="5058a-109">Stel enableADAL = 0 in met de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="5058a-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="5058a-110">Klik met de rechtermuisknop op de knop Start van Windows, **kies Uitvoeren,** typ **regedit** en kies **OK.**</span><span class="sxs-lookup"><span data-stu-id="5058a-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="5058a-111">Selecteer **Ja** om registereditor toe te staan wijzigingen aan te brengen op uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="5058a-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="5058a-112">Voeg in registereditor een DWORD-waarde van **EnableADAL** toe met een instelling **van 0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="5058a-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="5058a-113">Zie Verbindingsproblemen in aanmelding na update naar [Office 2016 build 16.0.7967 in Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="5058a-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>