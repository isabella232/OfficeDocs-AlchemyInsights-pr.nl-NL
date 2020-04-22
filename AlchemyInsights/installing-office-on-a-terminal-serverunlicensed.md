---
title: Kantoor installeren op een terminalserver - zonder licentie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763212"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="d1d99-102">Office installeren op een terminalserver</span><span class="sxs-lookup"><span data-stu-id="d1d99-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="d1d99-103">Voor het implementeren van Microsoft 365 Apps for enterprise op een Windows Server met Remote Desktop Services (RDS), voorheen Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="d1d99-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="d1d99-104">U moet een Microsoft 365-abonnement hebben dat Microsoft 365 Apps voor bedrijven bevat, zoals Office 365 Enterprise E3 of Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="d1d99-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="d1d99-105">De Microsoft 365 Apps for Business en Microsoft 365 Apps for business Premium-abonnementen bevatten geen Microsoft 365 Apps voor bedrijven.</span><span class="sxs-lookup"><span data-stu-id="d1d99-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="d1d99-106">U moet [de activering van gedeelde computers](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.</span><span class="sxs-lookup"><span data-stu-id="d1d99-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="d1d99-107">Als u Microsoft 365 Apps voor bedrijven op RDS wilt installeren vanuit het Microsoft 365-beheercentrum, ***dat standaardinstallatie-instellingen gebruikt,*** gebruikt u de volgende stappen.</span><span class="sxs-lookup"><span data-stu-id="d1d99-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="d1d99-108">U de [Microsoft Support- en Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) ook downloaden en uitvoeren om Microsoft 365 Apps voor bedrijven te installeren in de activeringsmodus voor gedeelde computers.</span><span class="sxs-lookup"><span data-stu-id="d1d99-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="d1d99-109">Controleer welk Microsoft 365-abonnement u hebt.</span><span class="sxs-lookup"><span data-stu-id="d1d99-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="d1d99-110">Meer informatie over hoe</span><span class="sxs-lookup"><span data-stu-id="d1d99-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="d1d99-111">Schakel indien nodig over naar een ander Microsoft 365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="d1d99-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="d1d99-112">Meer informatie over hoe</span><span class="sxs-lookup"><span data-stu-id="d1d99-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="d1d99-113">Als Office al is geïnstalleerd op de RDS-server met andere Microsoft 365-abonnementen, verwijdert u deze.</span><span class="sxs-lookup"><span data-stu-id="d1d99-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="d1d99-114">Bijvoorbeeld door naar Configuratiescherm \> te gaan Een programma verwijderen.</span><span class="sxs-lookup"><span data-stu-id="d1d99-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="d1d99-115">Verwijder met [Microsoft Support en Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.</span><span class="sxs-lookup"><span data-stu-id="d1d99-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="d1d99-116">Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="d1d99-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="d1d99-117">Nadat Office is geïnstalleerd, ***opent of meldt u zich niet*** aan bij Office-toepassingen.</span><span class="sxs-lookup"><span data-stu-id="d1d99-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="d1d99-118">Schakel op de RDS-server de activering van gedeelde computers in door het register te bewerken door de volgende stappen te volgen:</span><span class="sxs-lookup"><span data-stu-id="d1d99-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="d1d99-119">Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer Uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="d1d99-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="d1d99-120">Typ **regedit**in het vak Openen en selecteer OK.</span><span class="sxs-lookup"><span data-stu-id="d1d99-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="d1d99-121">Selecteer Ja wanneer u wordt gevraagd om de registereditor toe te staan wijzigingen aan te brengen in uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="d1d99-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="d1d99-122">Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d1d99-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="d1d99-123">Meld u op de ***RDS-server aan als eindgebruiker*** en [controleer of de activering van gedeelde computers is ingeschakeld voor Microsoft 365 Apps for Enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="d1d99-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="d1d99-124">Zie [Microsoft 365 Apps voor bedrijven implementeren met Remote Desktop Services voor](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office Deployment Tool.</span><span class="sxs-lookup"><span data-stu-id="d1d99-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="d1d99-125">Zie [Problemen met de activering van gedeelde computers oplossen voor microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)om fouten in verband met de activering van gedeelde computers op te lossen.</span><span class="sxs-lookup"><span data-stu-id="d1d99-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  