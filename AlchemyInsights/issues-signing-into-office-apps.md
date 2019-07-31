---
title: Problemen met het aanmelden bij Office apps
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938184"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="839cd-102">Tot vaststelling van het bericht Office apps 'vertrouwde Platform-module van de computer niet goed werkt. "</span><span class="sxs-lookup"><span data-stu-id="839cd-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="839cd-103">U kunt deze fout oplossen door het volgende proberen:</span><span class="sxs-lookup"><span data-stu-id="839cd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="839cd-104">Installeer de nieuwste updates voor [Windows](https://support.microsoft.com/help/4027667/windows-10-update) en [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="839cd-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="839cd-105">[Duidelijke Office referenties](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met behulp van Windows Referentiebeheer.</span><span class="sxs-lookup"><span data-stu-id="839cd-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="839cd-106">**Opmerking:** De paden voor Office 2016 hebt 16,0 gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="839cd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="839cd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="839cd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="839cd-108">Voer het [herstelproces gebruiker](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) u Trusted Platform Module (TPM)-fouten kunt oplossen.</span><span class="sxs-lookup"><span data-stu-id="839cd-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="839cd-109">Stel de EnableADAL = 0, met behulp van de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="839cd-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="839cd-110">Klik met de rechtermuisknop op de knop Start, kies **uitvoeren**, typ **regedit**en klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="839cd-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="839cd-111">Selecteer **Ja** om de Register-Editor om uw apparaat te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="839cd-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="839cd-112">In de Register-Editor een DWORD-waarde van **EnableADAL** met een instelling van **0** onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity toevoegen</span><span class="sxs-lookup"><span data-stu-id="839cd-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="839cd-113">Voor meer informatie, Zie [problemen met verbinding bij aanmelden nadat deze is bijgewerkt naar Office 2016 build 16.0.7967 op Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="839cd-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>