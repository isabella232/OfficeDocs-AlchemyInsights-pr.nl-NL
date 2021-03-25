---
title: Microsoft 365-apps voor ondernemingen implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200668"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="09bdd-102">Microsoft 365-apps voor ondernemingen implementeren voor gedeeld gebruik op RDS, Terminal Server of VDI</span><span class="sxs-lookup"><span data-stu-id="09bdd-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="09bdd-103">Microsoft 365-apps voor ondernemingen implementeren met RDS (Remote Desktop Services), voorheen Terminal Services genoemd:</span><span class="sxs-lookup"><span data-stu-id="09bdd-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="09bdd-104">U moet een Microsoft 365 Voor Bedrijven-abonnement of een Office 365-abonnement hebben met Microsoft 365 Apps voor ondernemingen, zoals Office 365 Enterprise E3 of Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="09bdd-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="09bdd-105">Microsoft 365 Apps voor Bedrijven en Microsoft 365 Business Standard-abonnementen bevatten geen Microsoft 365-apps voor ondernemingen.</span><span class="sxs-lookup"><span data-stu-id="09bdd-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="09bdd-106">U moet activering van [gedeelde computer inschakelen.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="09bdd-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="09bdd-107">U kunt ook de [Microsoft-ondersteunings-](https://aka.ms/SaRA_OfficeSCA_M365Portal) en herstelassistent downloaden en uitvoeren om Microsoft 365 Apps voor ondernemingen te installeren in de activeringsmodus voor gedeelde computer.</span><span class="sxs-lookup"><span data-stu-id="09bdd-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="09bdd-108">Zie [Microsoft 365-apps](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)voor bedrijven implementeren met behulp van Remote Desktop Services voor meer informatie over vereisten, installatie-instructies en richtlijnen voor aangepaste installaties met behulp van het Office-implementatieprogramma.</span><span class="sxs-lookup"><span data-stu-id="09bdd-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="09bdd-109">Fouten met betrekking tot activering van gedeelde computer oplossen:</span><span class="sxs-lookup"><span data-stu-id="09bdd-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="09bdd-110">Zie [Problemen oplossen met gedeelde computeractivering voor Microsoft 365 Apps voor bedrijven](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="09bdd-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="09bdd-111">Zie [Activeringsstatus van Microsoft 365-apps voor ondernemingen opnieuw instellen](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="09bdd-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="09bdd-112">Als u Microsoft 365 Apps voor ondernemingen wilt installeren op RDS vanuit het Microsoft 365-beheercentrum, dat standaardinstellingen voor installatie gebruikt, gebruikt u de volgende stappen:</span><span class="sxs-lookup"><span data-stu-id="09bdd-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="09bdd-113">Controleer welk abonnement u hebt.</span><span class="sxs-lookup"><span data-stu-id="09bdd-113">Check what subscription you have.</span></span> <span data-ttu-id="09bdd-114">[Meer informatie](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="09bdd-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="09bdd-115">Schakel indien nodig over naar een ander abonnement.</span><span class="sxs-lookup"><span data-stu-id="09bdd-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="09bdd-116">[Meer informatie](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="09bdd-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="09bdd-117">Als Office al is geïnstalleerd op de RDS-server met andere Microsoft-abonnementen, verwijdert u deze.</span><span class="sxs-lookup"><span data-stu-id="09bdd-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="09bdd-118">Ga bijvoorbeeld naar **Configuratiescherm**  >  **Een programma verwijderen.**</span><span class="sxs-lookup"><span data-stu-id="09bdd-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="09bdd-119">Verwijder de installatie [met microsoft-ondersteunings- en herstelassistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) als er problemen zijn.</span><span class="sxs-lookup"><span data-stu-id="09bdd-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="09bdd-120">Meld u op de RDS-server aan bij het Microsoft 365-beheercentrum met uw beheerdersaccount en [installeer Microsoft 365 Apps voor bedrijven.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="09bdd-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="09bdd-121">Nadat Office is geïnstalleerd, ***hoeft u zich niet te openen*** of aan te melden bij Office-toepassingen.</span><span class="sxs-lookup"><span data-stu-id="09bdd-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="09bdd-122">Schakel op de RDS-server de activering van gedeelde computer in door het register te bewerken door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="09bdd-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="09bdd-123">Klik met de rechtermuisknop op de Windows-knop in de linkerbenedenhoek van het scherm en selecteer **Uitvoeren.**</span><span class="sxs-lookup"><span data-stu-id="09bdd-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="09bdd-124">Typ in het vak Openen **regedit** en klik vervolgens op **OK**.</span><span class="sxs-lookup"><span data-stu-id="09bdd-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="09bdd-125">Selecteer **Ja** wanneer u wordt gevraagd om registereditor toe te staan wijzigingen aan te brengen op uw apparaat.</span><span class="sxs-lookup"><span data-stu-id="09bdd-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="09bdd-126">Voeg in de registereditor een tekenreekswaarde van **SharedComputerLicensing** toe met een instelling van 1 onder HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="09bdd-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="09bdd-127">Meld u op de  RDS-server aan als eindgebruiker en controleer of gedeelde computeractivering is ingeschakeld voor [Microsoft 365 Apps voor ondernemingen.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="09bdd-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
