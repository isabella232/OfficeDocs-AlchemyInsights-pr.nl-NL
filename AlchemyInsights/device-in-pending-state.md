---
title: Apparaat met status in behandeling
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/11/2020
ms.locfileid: "49677570"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="ecf53-102">Apparaat met status in behandeling</span><span class="sxs-lookup"><span data-stu-id="ecf53-102">Device in pending state</span></span>

<span data-ttu-id="ecf53-103">**Vereisten**</span><span class="sxs-lookup"><span data-stu-id="ecf53-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="ecf53-104">Als u apparaatregistratie voor het eerst instelt, moet u ervoor zorgen dat u de [Inleiding bij Apparaatbeheer hebt bekeken in azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) voor meer informatie over het krijgen van apparaten onder het beheer van Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ecf53-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="ecf53-105">Als u apparaten rechtstreeks registreert in azure AD en ze registreert in intune, moet u ervoor zorgen dat u [intune hebt geconfigureerd](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) en de [licenties](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) eerst moet invoeren.</span><span class="sxs-lookup"><span data-stu-id="ecf53-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="ecf53-106">Zorg ervoor dat u gemachtigd bent om bewerkingen uit te voeren in azure AD en on-premises AD.</span><span class="sxs-lookup"><span data-stu-id="ecf53-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="ecf53-107">U kunt in azure AD alleen een globale beheerder in azure AD instellingen beheren voor apparaatregistratie.</span><span class="sxs-lookup"><span data-stu-id="ecf53-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="ecf53-108">Als u automatische registraties in uw on-premises Active Directory wilt instellen, moet u ook een beheerder van Active Directory en AD FS (indien van toepassing) zijn.</span><span class="sxs-lookup"><span data-stu-id="ecf53-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="ecf53-109">Voor het Hybrid Azure AD join-registratieproces zijn apparaten in het bedrijfsnetwerk vereist.</span><span class="sxs-lookup"><span data-stu-id="ecf53-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="ecf53-110">Dit werkt ook via VPN, maar er is een aantal voorbehoud.</span><span class="sxs-lookup"><span data-stu-id="ecf53-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="ecf53-111">We hebben klanten die u willen assistentie bij het oplossen van problemen met het oplossen van het hybride Azure AD-registratieproces onder externe werkomstandigheden.</span><span class="sxs-lookup"><span data-stu-id="ecf53-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="ecf53-112">**Cloud verificatie omgeving (via Azure AD Password Hash sync of Pass Through-verificatie)**</span><span class="sxs-lookup"><span data-stu-id="ecf53-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="ecf53-113">Deze registratie stroom wordt ook wel ' synchronisatie deelnemen ' genoemd.</span><span class="sxs-lookup"><span data-stu-id="ecf53-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="ecf53-114">Hier ziet u een overzicht van wat er gebeurt tijdens het registratieproces:</span><span class="sxs-lookup"><span data-stu-id="ecf53-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="ecf53-115">Windows 10-record service verbindingspunt (SCP) wordt gedetecteerd wanneer de gebruiker zich aanmeldt bij het apparaat.</span><span class="sxs-lookup"><span data-stu-id="ecf53-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="ecf53-116">Het apparaat probeert eerst Tenant informatie op te halen uit de clientzijde-SCP in het register [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="ecf53-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="ecf53-117">Zie voor meer informatie [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="ecf53-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="ecf53-118">Als dit mislukt, communiceert het apparaat met on-premises Active Directory om Tenant informatie op te halen van SCP.</span><span class="sxs-lookup"><span data-stu-id="ecf53-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="ecf53-119">Als u SCP wilt controleren, raadpleegt u dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="ecf53-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="ecf53-120">U wordt aangeraden SCP in te schakelen in Active Directory en alleen aan clientzijde-SCP te gebruiken voor de eerste validatie.</span><span class="sxs-lookup"><span data-stu-id="ecf53-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="ecf53-121">Windows 10 probeert met Azure AD te communiceren onder de systeemcontext om zichzelf te verifiëren tegen Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ecf53-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="ecf53-122">U kunt controleren of het apparaat toegang heeft tot Microsoft-bronnen onder het systeemaccount met behulp van het script voor het [registreren van apparaten](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="ecf53-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="ecf53-123">In Windows 10 wordt zelfondertekend certificaat gegenereerd en opgeslagen onder het computerobject in on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ecf53-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="ecf53-124">Dit vereist regel-van-gezichtsvermogen voor domein controller.</span><span class="sxs-lookup"><span data-stu-id="ecf53-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="ecf53-125">Apparaatobject met certificaat dat via Azure AD Connect via Azure AD Connect wordt gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ecf53-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="ecf53-126">De synchronisatie cyclus is standaard elke 30 minuten, maar dit is afhankelijk van de configuratie van Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ecf53-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="ecf53-127">Zie dit [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ecf53-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="ecf53-128">In dit stadium ziet u mogelijk het onderwerp-apparaat in de status **in behandeling** onder apparaatprofielen van Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ecf53-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="ecf53-129">Bij de volgende gebruikersaanmelding met Windows 10 wordt de registratie beëindigd.</span><span class="sxs-lookup"><span data-stu-id="ecf53-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="ecf53-130">Als u gebruikmaakt van VPN en afmelden of als u de domein verbinding beëindigt, kunt u de registratie handmatig activeren.</span><span class="sxs-lookup"><span data-stu-id="ecf53-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="ecf53-131">U doet dit als volgt:</span><span class="sxs-lookup"><span data-stu-id="ecf53-131">To do that:</span></span>
    >
    > <span data-ttu-id="ecf53-132">Meld u aan bij een `dsregcmd /join` lokale beheerder of extern via PSExec op uw PC.</span><span class="sxs-lookup"><span data-stu-id="ecf53-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="ecf53-133">Voorbeeld: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="ecf53-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="ecf53-134">Zie [Veelgestelde vragen over apparaten](https://docs.microsoft.com/azure/active-directory/devices/faq)voor algemene problemen met de registratie van Azure Active Directory-apparaten.</span><span class="sxs-lookup"><span data-stu-id="ecf53-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
