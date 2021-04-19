---
title: 'AIP-scanner: installatie en configuratie'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821658"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="1ccf2-102">AIP-scanner: installatie en configuratie</span><span class="sxs-lookup"><span data-stu-id="1ccf2-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="1ccf2-103">**Als u de AIP-scanner wilt installeren, volgt u de aanbevolen richtlijnen:**</span><span class="sxs-lookup"><span data-stu-id="1ccf2-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="1ccf2-104">Als u een upgrade uitwerkt en geen schone installatie uitwerkt, controleert u of u de richtlijnen voor het upgraden van de [Azure Information Protection-scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) en voor geïntegreerde labelingclient hebt gevolgd, raadpleegt u het upgraden van de [Azure Information Protection-scanner.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="1ccf2-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="1ccf2-105">Controleer of u voldoet aan alle instellingen voor firewalls en [netwerkinfrastructuur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="1ccf2-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="1ccf2-106">Zorg ervoor dat [uw beleid is ingesteld](https://docs.microsoft.com/azure/information-protection/configure-policy) op automatische labeling of een standaardlabel in het beleid heeft.</span><span class="sxs-lookup"><span data-stu-id="1ccf2-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="1ccf2-107">Zorg ervoor dat het desbetreffende bestandstype is geconfigureerd voor label/beveiliging, zoals beschreven in bestandstypen die worden ondersteund [door de Azure Information Protection-client.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="1ccf2-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="1ccf2-108">Als u het standaardgedrag wilt wijzigen, volgt u de volgende richtlijnen: [Het standaardbeveiligingsniveau van bestanden wijzigen.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="1ccf2-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="1ccf2-109">Controleer of het gebruikersaccount dat is geconfigureerd om de scannerservice uit te voeren, machtigingen heeft voor toegang tot alle geconfigureerde opslagplaatsen.</span><span class="sxs-lookup"><span data-stu-id="1ccf2-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="1ccf2-110">Als er nog steeds problemen zijn, exporteert u de scannerlogboeken en voegt u deze toe aan uw ondersteuningsticket.</span><span class="sxs-lookup"><span data-stu-id="1ccf2-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="1ccf2-111">**Azure Information Protection Scanner-logboeken exporteren**</span><span class="sxs-lookup"><span data-stu-id="1ccf2-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="1ccf2-112">Ga naar %localappdata%\Microsoft\MSIP onder de gebruikerscontext met de scannerservice.</span><span class="sxs-lookup"><span data-stu-id="1ccf2-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="1ccf2-113">Zip alle inhoud onder de map MSIP.</span><span class="sxs-lookup"><span data-stu-id="1ccf2-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="1ccf2-114">Sla de logboeken op de door u gekozen locatie op en voeg ze toe aan uw serviceverzoek.</span><span class="sxs-lookup"><span data-stu-id="1ccf2-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="1ccf2-115">U kunt ook [Export-AIPLogs -OnBehalfOf gebruiken.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="1ccf2-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="1ccf2-116">**Zie voor meer informatie:**</span><span class="sxs-lookup"><span data-stu-id="1ccf2-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="1ccf2-117">De Azure Information Protection-scanner implementeren om bestanden automatisch te classificeren en te beveiligen</span><span class="sxs-lookup"><span data-stu-id="1ccf2-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="1ccf2-118">De parameter Token opgeven en gebruiken voor Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="1ccf2-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="1ccf2-119">Een detectiecyclus uitvoeren en rapporten voor de scanner weergeven</span><span class="sxs-lookup"><span data-stu-id="1ccf2-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="1ccf2-120">Azure Information Protection-documentatie bekijken</span><span class="sxs-lookup"><span data-stu-id="1ccf2-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="1ccf2-121">Vereisten voor Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="1ccf2-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="1ccf2-122">Azure Information Protection-client downloaden</span><span class="sxs-lookup"><span data-stu-id="1ccf2-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
