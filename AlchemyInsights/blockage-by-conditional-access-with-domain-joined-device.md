---
title: Ik word geblokkeerd door Voorwaardelijke toegang met een apparaat dat is verbonden met een domein
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035722"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="a5538-102">Ik word geblokkeerd door Voorwaardelijke toegang met een apparaat dat is verbonden met een domein</span><span class="sxs-lookup"><span data-stu-id="a5538-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="a5538-103">**Sterk aanbevolen hulpprogramma's**</span><span class="sxs-lookup"><span data-stu-id="a5538-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="a5538-104">[Hulpprogramma voor probleemoplosser](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) voor apparaatregistratie: het hulpprogramma waarmee u de meest voorkomende problemen met apparaatregistratie kunt oplossen.</span><span class="sxs-lookup"><span data-stu-id="a5538-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="a5538-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : het script waarmee u ervoor kunt zorgen dat een apparaat toegang heeft tot eindpunten voor apparaatregistratie onder het systeemaccount.</span><span class="sxs-lookup"><span data-stu-id="a5538-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="a5538-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) : het script waarmee u verouderde apparaten in uw omgeving kunt zoeken en beheren.</span><span class="sxs-lookup"><span data-stu-id="a5538-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="a5538-107">Hier zijn enkele veelvoorkomende redenen waarom voorwaardelijke toegang kan mislukken bij een apparaat dat deel heeft uit gemaakt van een domein (Hybride Azure AD).</span><span class="sxs-lookup"><span data-stu-id="a5538-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="a5538-108">**Er is geen Azure AD PRT** op het apparaat: u moet ervoor zorgen dat het apparaat Azure AD Primary Refresh Token (PRT) heeft.</span><span class="sxs-lookup"><span data-stu-id="a5538-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="a5538-109">Zie dit document voor meer [informatie](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)over PRT.</span><span class="sxs-lookup"><span data-stu-id="a5538-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="a5538-110">Als u wilt controleren of u Azure AD PRT hebt, kunt u de opdracht uitvoeren op het apparaat en controleren of `dsregcmd/status` 'AzureAdPrt' gelijk is aan 'JA'.</span><span class="sxs-lookup"><span data-stu-id="a5538-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="a5538-111">Als 'AzureAdPrt' 'NEE' is, gaat u als volgt te werk:</span><span class="sxs-lookup"><span data-stu-id="a5538-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="a5538-112">Of u nu een federatief omgeving met **AD FS** hebt en dat deze niet bereikbaar is vanuit de thuisnetwerken van uw gebruikers: In dit geval moet u ervoor zorgen dat uw 'gebruikersnaammixed' eindpunten toegankelijk zijn via het extranet.</span><span class="sxs-lookup"><span data-stu-id="a5538-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="a5538-113">Als uw AD FS achter een VPN zit, zorgt u ervoor dat de gebruikers verbinding maken met de VPN en zich opnieuw aanmelden bij het apparaat.</span><span class="sxs-lookup"><span data-stu-id="a5538-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="a5538-114">Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="a5538-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="a5538-115">**Of de TPM van** het apparaat defect is en dus het apparaat niet kan verifiëren: Controleer 'tpm.msc' om te zien of de status van TPM 'Ready' is.</span><span class="sxs-lookup"><span data-stu-id="a5538-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="a5538-116">Zo niet, voer `dsregcmd/leave` het apparaat uit en laat het opnieuw deelnemen aan Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a5538-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="a5538-117">Probeer het vervolgens opnieuw.</span><span class="sxs-lookup"><span data-stu-id="a5538-117">Then, try again.</span></span> <span data-ttu-id="a5538-118">Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="a5538-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="a5538-119">U gebruikt een externe identiteitsprovider, die geen ondersteuning biedt **voor WS-Trust protocol.**</span><span class="sxs-lookup"><span data-stu-id="a5538-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="a5538-120">Zoals wordt beschreven in onze documenten, kunnen hybride apparaten met Azure AD-apparaten in dit geval niet werken.</span><span class="sxs-lookup"><span data-stu-id="a5538-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="a5538-121">Werk samen met uw identiteitsprovider voor ondersteuning.</span><span class="sxs-lookup"><span data-stu-id="a5538-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="a5538-122">Gebruikers gebruiken de Chrome-browser zonder de **Windows 10-accounts** of Office-extensie Chrome gebruikt de PRT niet automatisch op **AAD-apparaten** of hybride AAD-apparaten: Dit leidt tot het mislukken van elk beleid op basis van voorwaardelijke toegang op apparaten, met het foutbericht 'Niet-geregistreerd apparaat' weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a5538-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="a5538-123">Als u de Chrome-browser correct wilt gebruiken, moet u de 'Windows 10-accounts' of 'Office-extensie voor de Chrome-browser van de gebruikers' installeren via SCCM of Intune.</span><span class="sxs-lookup"><span data-stu-id="a5538-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="a5538-124">Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="a5538-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="a5538-125">Als het niet mogelijk is om de extensie op afstand te pushen, stelt u gebruikers op de hoogte om een van de bovenstaande extensies handmatig te installeren voor toegang tot toepassingen achter apparaatgebaseerde voorwaardelijke toegang.</span><span class="sxs-lookup"><span data-stu-id="a5538-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="a5538-126">Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="a5538-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="a5538-127">Het apparaat is correct hybride Azure AD samengevoegd, maar is per ongeluk verwijderd of uitgeschakeld, hetzij vanwege synchronisatiewijzigingen in Azure AD Connect of vanuit de **Azure-portal:** Als dit gebeurt, wordt het apparaatobject niet meer herkend als een volledig verbonden apparaat, ook al wordt de status 'AzureAdJoined' en 'PRT' als geldig op het apparaat weergeven.</span><span class="sxs-lookup"><span data-stu-id="a5538-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="a5538-128">Als u dit probleem wilt oplossen, wordt dit uitgevoerd op de betreffende apparaten en kunnen ze opnieuw aan `dsregcmd/leave` Azure AD gaan werken.</span><span class="sxs-lookup"><span data-stu-id="a5538-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="a5538-129">Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="a5538-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="a5538-130">Als uw apparaten windows 10, 1809 bijwerken met VPN/Cloudproxy en problemen zien met de status AzureAdPrt of een app met een SSO-probleem (outlook die geen verbinding maakt met postvak, zelfs als u PRT had), zorgt u ervoor dat u deze patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) of april cumulatieve update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) hebt om PRT-fouten op deze machines te voorkomen.</span><span class="sxs-lookup"><span data-stu-id="a5538-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















