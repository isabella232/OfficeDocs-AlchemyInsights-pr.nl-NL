---
title: Office installeren op een Terminal Server-zonder licentie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663112"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="b4b16-102">Office installeren op een Terminal Server</span><span class="sxs-lookup"><span data-stu-id="b4b16-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="b4b16-103">Voor het implementeren van Microsoft 365-apps voor Enterprise op een Windows Server met extern bureaublad-services (RDS), eerder met de naam Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="b4b16-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="b4b16-104">U moet een Microsoft 365-abonnement hebben dat Microsoft 365-apps voor Enterprise bevat, zoals Office 365 Enterprise E3 of Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="b4b16-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="b4b16-105">De Microsoft 365 apps for Business and Microsoft 365 apps for Business Premium-abonnementen bevatten geen Microsoft 365-apps voor Enterprise.</span><span class="sxs-lookup"><span data-stu-id="b4b16-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="b4b16-106">U dient de activering van de [gedeelde computer](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)in te schakelen.</span><span class="sxs-lookup"><span data-stu-id="b4b16-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="b4b16-107">Voer de volgende stappen uit als u Microsoft 365-apps voor Enterprise op RDS wilt installeren via het Microsoft 365-Beheercentrum, met de ***Standaardinstellingen voor installeren***.</span><span class="sxs-lookup"><span data-stu-id="b4b16-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="b4b16-108">U kunt ook [Microsoft ondersteuning en herstel ondersteuning](https://aka.ms/SaRA_OfficeSCA_M365Portal) voor het installeren van microsoft 365-apps voor Enterprise downloaden en uitvoeren in de modus voor activering van de gedeelde computer.</span><span class="sxs-lookup"><span data-stu-id="b4b16-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="b4b16-109">Controleer wat Microsoft 365-abonnement u hebt.</span><span class="sxs-lookup"><span data-stu-id="b4b16-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="b4b16-110">Meer informatie</span><span class="sxs-lookup"><span data-stu-id="b4b16-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="b4b16-111">Overschakelen naar een ander abonnement van Microsoft 365, indien nodig.</span><span class="sxs-lookup"><span data-stu-id="b4b16-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="b4b16-112">Meer informatie</span><span class="sxs-lookup"><span data-stu-id="b4b16-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="b4b16-113">Als Office al op de RDS-server is geïnstalleerd met andere Microsoft 365-abonnementen, verwijdert u de app.</span><span class="sxs-lookup"><span data-stu-id="b4b16-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="b4b16-114">U kunt bijvoorbeeld een programma verwijderen via het Configuratiescherm \> .</span><span class="sxs-lookup"><span data-stu-id="b4b16-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="b4b16-115">Verwijder met de [Microsoft-ondersteunings-en herstel assistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.</span><span class="sxs-lookup"><span data-stu-id="b4b16-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="b4b16-116">Meld u op de RDS-server aan bij het Microsoft 365-Beheercentrum met uw beheerdersaccount en [Installeer Microsoft 365-apps voor Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="b4b16-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="b4b16-117">Wanneer Office is geïnstalleerd, kunt u geen Office-toepassingen ***openen of u aanmelden*** .</span><span class="sxs-lookup"><span data-stu-id="b4b16-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="b4b16-118">Schakel op de RDS-server het activeren van activerings computers in door het register als volgt te bewerken:</span><span class="sxs-lookup"><span data-stu-id="b4b16-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="b4b16-119">Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="b4b16-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="b4b16-120">Typ in het vak Openen de opdracht **regedit**en klik vervolgens op OK.</span><span class="sxs-lookup"><span data-stu-id="b4b16-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="b4b16-121">Selecteer Ja wanneer u wordt gevraagd of u de Register-editor wilt toestaan om wijzigingen op uw apparaat aan te brengen.</span><span class="sxs-lookup"><span data-stu-id="b4b16-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="b4b16-122">In de Register-editor voegt u een tekenreekswaarde van **SharedComputerLicensing** met de instelling 1 onder HKEY_LOCAL_MACHINE \Software\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="b4b16-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="b4b16-123">Meld u op de RDS-server aan ***als een eindgebruiker*** en [Controleer of de activering voor gedeelde computers is ingeschakeld voor Microsoft 365-apps voor ondernemingen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="b4b16-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="b4b16-124">Zie voor meer informatie over de installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office-implementatieprogramma [Microsoft 365-Apps implementeren voor Enterprise met behulp van extern bureaublad services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="b4b16-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="b4b16-125">Zie problemen met de activering van een [gedeelde computer voor Microsoft 365-apps voor bedrijven oplossen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)voor meer informatie over het oplossen van problemen met de activering van een gedeelde computer.</span><span class="sxs-lookup"><span data-stu-id="b4b16-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  