---
title: Office installeren op een Terminal Server-zonder licentie
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205404"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="fff83-102">Office installeren op een Terminal Server</span><span class="sxs-lookup"><span data-stu-id="fff83-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="fff83-103">Voor het implementeren van Office 365 ProPlus op een Windows-Server met behulp van extern bureaublad-services (RDS), voorheen genaamd Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="fff83-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="fff83-104">U moet beschikken over een Office 365-abonnement met Office 365 ProPlus, zoals Office 365 Enterprise E3 of Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="fff83-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="fff83-105">De Office 365 Business en Office 365 Business Premium-abonnementen bevatten geen Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="fff83-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="fff83-106">U moet de [Activering van gedeelde computers](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)inschakelen.</span><span class="sxs-lookup"><span data-stu-id="fff83-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="fff83-107">Als u wilt installeren van Office 365 ProPlus op RDS van de Microsoft 365 Admin Center, ***die gebruikmaakt van standaardinstallatie-instellingen***, gebruikt u de volgende stappen uit.</span><span class="sxs-lookup"><span data-stu-id="fff83-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="fff83-108">U ook de [Microsoft-ondersteunings-en Herstelassistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) downloaden en uitvoeren om Office 365 ProPlus te installeren in de activerings modus voor gedeelde computers.</span><span class="sxs-lookup"><span data-stu-id="fff83-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="fff83-109">Controleer welk Office 365-abonnement u hebt.</span><span class="sxs-lookup"><span data-stu-id="fff83-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="fff83-110">Leer hoe</span><span class="sxs-lookup"><span data-stu-id="fff83-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="fff83-111">Schakel indien nodig naar een ander Office 365-abonnement.</span><span class="sxs-lookup"><span data-stu-id="fff83-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="fff83-112">Leer hoe</span><span class="sxs-lookup"><span data-stu-id="fff83-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="fff83-113">Als Office al is geïnstalleerd op de RDS-server met behulp van een andere Office 365-abonnementen, verwijdert u deze.</span><span class="sxs-lookup"><span data-stu-id="fff83-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="fff83-114">Bijvoorbeeld, door te gaan naar het configuratie \> scherm een programma verwijderen.</span><span class="sxs-lookup"><span data-stu-id="fff83-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="fff83-115">Verwijder met [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) als u problemen ondervindt.</span><span class="sxs-lookup"><span data-stu-id="fff83-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="fff83-116">Meld u op de RDS-server aan bij het Microsoft 365 Admin Center met uw beheerdersaccount en [Installeer Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="fff83-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="fff83-117">Nadat Office is geïnstalleerd, ***niet openen of aanmelden*** bij een Office-toepassingen.</span><span class="sxs-lookup"><span data-stu-id="fff83-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="fff83-118">Schakel op de RDS-server de activering van gedeelde computers in door het register te bewerken door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="fff83-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="fff83-119">Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van uw scherm en selecteer uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="fff83-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="fff83-120">Typ **regedit**in het vak openen en selecteer vervolgens OK.</span><span class="sxs-lookup"><span data-stu-id="fff83-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="fff83-121">Selecteer Ja wanneer u wordt gevraagd de Register-editor toe te staan wijzigingen aan te brengen in uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="fff83-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="fff83-122">In de Register-editor, voeg een tekenreekswaarde van **Sharedcomputerlicensing** met een instelling van 1 onder HKEY_LOCAL_MACHINE \Software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="fff83-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="fff83-123">Meld u op de RDS-server aan ***als eindgebruiker*** en [Controleer of de activering van gedeelde computers is ingeschakeld voor Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="fff83-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="fff83-124">Zie voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van de Office Deployment Tool, [office 365 ProPlus implementeren met behulp van extern bureaublad-services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="fff83-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="fff83-125">Als u fouten met betrekking tot de activering van gedeelde computers wilt oplossen, raadpleegt u [problemen met gedeelde computer activering voor Office 365 ProPlus oplossen](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="fff83-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  