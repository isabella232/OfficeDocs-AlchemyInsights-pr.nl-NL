---
title: Probleem met PRT oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573493"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="09571-102">Probleem met PRT oplossen</span><span class="sxs-lookup"><span data-stu-id="09571-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="09571-103">Om te voorkomen dat een apparaat wordt geverifieerd, moet het volledig geregistreerd en in goede staat zijn en kan een primaire vernieuwings token (PRT) worden verkregen.</span><span class="sxs-lookup"><span data-stu-id="09571-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="09571-104">Voor het Hybrid Azure AD-registratieproces zijn apparaten in een bedrijfsnetwerk vereist.</span><span class="sxs-lookup"><span data-stu-id="09571-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="09571-105">Dit werkt ook via VPN, maar er is een aantal voorbehoud.</span><span class="sxs-lookup"><span data-stu-id="09571-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="09571-106">We willen klanten weten dat ze hulp nodig hebben bij het oplossen van problemen bij het registreren van het hybride Azure AD join-registratieproces onder externe werkomstandigheden.</span><span class="sxs-lookup"><span data-stu-id="09571-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="09571-107">Dit is een uitsplitsing van wat er gebeurt onder de oppervlakte tijdens het registratieproces.</span><span class="sxs-lookup"><span data-stu-id="09571-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="09571-108">**Cloud verificatie omgeving (via Azure AD Password Hash sync of Pass Through-verificatie)**</span><span class="sxs-lookup"><span data-stu-id="09571-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="09571-109">Deze registratie stroom wordt ook wel ' synchronisatie deelnemen ' genoemd.</span><span class="sxs-lookup"><span data-stu-id="09571-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="09571-110">Windows 10 detecteert een SCP-record bij gebruikers die zich bij het apparaat aanmelden.</span><span class="sxs-lookup"><span data-stu-id="09571-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="09571-111">Het apparaat probeert eerst Tenant informatie op te halen uit de clientzijde-SCP in het register [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="09571-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="09571-112">Zie dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="09571-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="09571-113">Als dit mislukt, communiceert het apparaat met on-premises Active Directory (AD) om Tenant informatie op te halen van het service verbindingspunt (SCP).</span><span class="sxs-lookup"><span data-stu-id="09571-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="09571-114">Als u SCP wilt controleren, raadpleegt u dit [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="09571-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="09571-115">U wordt aangeraden SCP in te schakelen in de advertentie en uitsluitend aan clientzijde-SCP te gebruiken voor initiële verificatie.</span><span class="sxs-lookup"><span data-stu-id="09571-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="09571-116">Windows 10 probeert met Azure AD te communiceren onder de systeemcontext om zichzelf te verifiëren tegen Azure AD.</span><span class="sxs-lookup"><span data-stu-id="09571-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="09571-117">U kunt controleren of het apparaat toegang heeft tot Microsoft-bronnen onder het systeemaccount met behulp van het script voor het registreren van apparaten.</span><span class="sxs-lookup"><span data-stu-id="09571-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="09571-118">In Windows 10 wordt een zelfondertekend certificaat gegenereerd en opgeslagen onder het computerobject in on-premises advertenties.</span><span class="sxs-lookup"><span data-stu-id="09571-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="09571-119">Dit vereist regel-van-gezichtsvermogen voor domein controller.</span><span class="sxs-lookup"><span data-stu-id="09571-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="09571-120">Een apparaatobject met een certificaat wordt gesynchroniseerd met Azure AD via Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="09571-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="09571-121">De synchronisatie cyclus is standaard elke 30 minuten, maar dit is afhankelijk van de configuratie van Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="09571-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="09571-122">Raadpleeg dit [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="09571-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="09571-123">In dit stadium ziet u mogelijk het onderwerp-apparaat in de status in behandeling onder apparaatprofielen van Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="09571-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="09571-124">Bij de volgende gebruikersaanmelding met Windows 10 wordt de registratie beëindigd.</span><span class="sxs-lookup"><span data-stu-id="09571-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="09571-125">Als u een VPN-verbinding hebt en een proces voor afmelden afmelden de domein verbinding beëindigt, kunt u de registratie handmatig activeren:</span><span class="sxs-lookup"><span data-stu-id="09571-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="09571-126">Meld u op een dsregcmd-/join lokale vragen of extern via PSExec op uw PC.</span><span class="sxs-lookup"><span data-stu-id="09571-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="09571-127">Bijvoorbeeld PsExec-s \\ win10client01 cmd, dsregcmd/join</span><span class="sxs-lookup"><span data-stu-id="09571-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="09571-128">Zie [problemen met apparaten oplossen](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)voor meer informatie over problemen met hybride verbindingen.</span><span class="sxs-lookup"><span data-stu-id="09571-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
