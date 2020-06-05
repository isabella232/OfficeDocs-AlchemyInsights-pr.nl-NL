---
title: Problemen met aanmelden bij Microsoft 365-apps
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579860"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="e1190-102">Het bericht microsoft 365-apps 'De trusted platformmodule van uw computer werkt niet goed' herstellen</span><span class="sxs-lookup"><span data-stu-id="e1190-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="e1190-103">Probeer het volgende om deze fout op te lossen:</span><span class="sxs-lookup"><span data-stu-id="e1190-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e1190-104">Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="e1190-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="e1190-105">[Office-referenties wissen](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="e1190-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e1190-106">**Let op:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0.</span><span class="sxs-lookup"><span data-stu-id="e1190-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e1190-107">(Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e1190-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e1190-108">Probeer het [herstelproces van](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) de gebruiker om TPM-fouten (Trusted Platform Module) op te lossen.</span><span class="sxs-lookup"><span data-stu-id="e1190-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="e1190-109">Stel de EnableADAL = 0 in met de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="e1190-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="e1190-110">Klik met de rechtermuisknop op de knop Start van Windows, kies **Uitvoeren**, typ **regedit**en kies **OK**.</span><span class="sxs-lookup"><span data-stu-id="e1190-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="e1190-111">Selecteer **Ja** om registereditor toe te staan wijzigingen aan te brengen in uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="e1190-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="e1190-112">Voeg in registereditor een DWORD-waarde van **EnableADAL** toe met een instelling van **0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="e1190-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="e1190-113">Zie [Verbindingsproblemen in aanmelding na update naar Office 2016 build 16.0.7967 voor](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)meer informatie in Windows 10 .</span><span class="sxs-lookup"><span data-stu-id="e1190-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>