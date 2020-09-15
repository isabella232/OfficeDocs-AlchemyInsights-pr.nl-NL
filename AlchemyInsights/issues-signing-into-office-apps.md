---
title: Problemen bij het aanmelden bij Microsoft 365-apps
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
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695174"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d65a1-102">Het repareren van de Microsoft 365-apps "de vertrouwde platform module van uw computer functioneert niet goed"</span><span class="sxs-lookup"><span data-stu-id="d65a1-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d65a1-103">Probeer het volgende om deze fout op te lossen:</span><span class="sxs-lookup"><span data-stu-id="d65a1-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d65a1-104">Installeer de meest recente updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="d65a1-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d65a1-105">[Wis Office-referenties](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="d65a1-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d65a1-106">**Opmerking:** De registerpaden voor Office 2016 zijn gewijzigd in 16,0.</span><span class="sxs-lookup"><span data-stu-id="d65a1-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d65a1-107">(Bijvoorbeeld: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d65a1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d65a1-108">Probeer het [gebruikersherstel proces](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) voor het oplossen van TPM-fouten (Trusted Platform Module).</span><span class="sxs-lookup"><span data-stu-id="d65a1-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d65a1-109">Stel de EnableADAL = 0 in met de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="d65a1-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d65a1-110">Klik met de rechtermuisknop op de knop Start van Windows, kies **uitvoeren**, typ **regedit**en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="d65a1-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d65a1-111">Selecteer **Ja** als u wilt dat de Register-editor wijzigingen aan uw apparaat aanbrengt.</span><span class="sxs-lookup"><span data-stu-id="d65a1-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d65a1-112">In de Register-editor voegt u de DWORD-waarde **EnableADAL** met de instelling **0** onder HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="d65a1-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d65a1-113">Zie voor meer informatie [verbindingsproblemen tijdens het aanmelden na update naar Office 2016 build 16.0.7967 voor Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="d65a1-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>