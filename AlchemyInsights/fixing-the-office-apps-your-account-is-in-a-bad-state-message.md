---
title: De Office-apps herstellen Uw account is in een slecht staatsbericht
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969363"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="f883c-102">De fout van Office-apps 'Uw account is in een slechte staat' herstellen</span><span class="sxs-lookup"><span data-stu-id="f883c-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="f883c-103">Als u deze fout wilt oplossen, probeert u de volgende opties op de betreffende computer:</span><span class="sxs-lookup"><span data-stu-id="f883c-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="f883c-104">Open een Office-app en selecteer **Account** > \*\*\*\* > **afmelden van alle accounts**.</span><span class="sxs-lookup"><span data-stu-id="f883c-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="f883c-105">Meld u opnieuw aan met een gebruikersaccount met een geldige licentie.</span><span class="sxs-lookup"><span data-stu-id="f883c-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="f883c-106">Zie [Accounts in Office voor](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f883c-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="f883c-107">[Office-referenties wissen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) met Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="f883c-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="f883c-108">**Let op:** De registerpaden voor Office 2016 zijn gewijzigd in 16.0.</span><span class="sxs-lookup"><span data-stu-id="f883c-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="f883c-109">\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="f883c-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="f883c-110">Stel op de betreffende computer de EnableADAL = 0 in met de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="f883c-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="f883c-111">Klik met de rechtermuisknop op de knop Windows en selecteer **Uitvoeren**.</span><span class="sxs-lookup"><span data-stu-id="f883c-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="f883c-112">Typ **regedit**in het vak **Openen** en selecteer **OK**.</span><span class="sxs-lookup"><span data-stu-id="f883c-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="f883c-113">Selecteer **Ja** wanneer u wordt gevraagd registereditor toe te staan wijzigingen aan te brengen in uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="f883c-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="f883c-114">Voeg in de registereditor een DWORD-waarde van EnableADAL toe met een instelling van 0 onder HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="f883c-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="f883c-115">Als de fout optreedt tijdens het verbinden met Office 365 met Office 2013, [schakelt u moderne verificatie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) in voor de Office-client.</span><span class="sxs-lookup"><span data-stu-id="f883c-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="f883c-116">Zie [Problemen met niet-browserapps die zich niet kunnen aanmelden bij Office 365, Azure of Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f883c-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

