---
title: 'AIP-scanner: installatie en configuratie'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357662"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="c83cb-102">AIP-scanner: installatie en configuratie</span><span class="sxs-lookup"><span data-stu-id="c83cb-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="c83cb-103">**Als u de AIP-scanner wilt installeren, volgt u de aanbevolen richtlijnen:**</span><span class="sxs-lookup"><span data-stu-id="c83cb-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="c83cb-104">Als u een upgrade uitvoert en geen schone installatie uitvoert, moet u ervoor zorgen dat u de richtlijnen voor [het upgraden van de Azure Information Protection-scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) en voor uniforme etiketteringsclient hebt gevolgd, zie upgraden van de Azure Information [Protection-scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="c83cb-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="c83cb-105">Controleer of u voldoet aan alle [vereisten voor firewalls en netwerkinfrastructuur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="c83cb-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="c83cb-106">Zorg ervoor dat uw [beleid is ingesteld op](https://docs.microsoft.com/azure/information-protection/configure-policy) automatische etikettering of een standaardlabel in het beleid heeft.</span><span class="sxs-lookup"><span data-stu-id="c83cb-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="c83cb-107">Controleer of het relevante bestandstype is geconfigureerd voor label/beveiliging zoals beschreven in [bestandstypen die worden ondersteund door de Azure Information Protection-client.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="c83cb-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="c83cb-108">Als u het standaardgedrag wilt wijzigen, volgt u bovendien de volgende richtlijnen: [Het standaardbeveiligingsniveau van bestanden wijzigen.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="c83cb-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="c83cb-109">Controleer of het gebruikersaccount dat is geconfigureerd om de scannerservice uit te voeren, machtigingen heeft om toegang te krijgen tot alle geconfigureerde opslagplaatsen.</span><span class="sxs-lookup"><span data-stu-id="c83cb-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="c83cb-110">Als u nog steeds problemen ondervindt, exporteert u de scannerlogboeken en voegt u deze toe aan uw ondersteuningsticket.</span><span class="sxs-lookup"><span data-stu-id="c83cb-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="c83cb-111">**Azure Information Protection Scanner-logboeken exporteren**</span><span class="sxs-lookup"><span data-stu-id="c83cb-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="c83cb-112">Navigeer naar %localappdata%\Microsoft\MSIP onder de gebruikerscontext waarop de scannerservice wordt uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="c83cb-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="c83cb-113">Rits alle inhoud onder de MSIP-map.</span><span class="sxs-lookup"><span data-stu-id="c83cb-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="c83cb-114">Sla de logboeken op bij uw locatiekeuze en voeg ze toe aan uw serviceaanvraag.</span><span class="sxs-lookup"><span data-stu-id="c83cb-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="c83cb-115">U ook [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)gebruiken.</span><span class="sxs-lookup"><span data-stu-id="c83cb-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="c83cb-116">**Zie voor meer informatie**:</span><span class="sxs-lookup"><span data-stu-id="c83cb-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="c83cb-117">De Azure Information Protection-scanner implementeren om bestanden automatisch te classificeren en te beveiligen</span><span class="sxs-lookup"><span data-stu-id="c83cb-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="c83cb-118">De parameter Token opgeven en gebruiken voor Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="c83cb-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="c83cb-119">Een detectiecyclus uitvoeren en rapporten voor de scanner weergeven</span><span class="sxs-lookup"><span data-stu-id="c83cb-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="c83cb-120">Documentatie over Azure Information Protection controleren</span><span class="sxs-lookup"><span data-stu-id="c83cb-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c83cb-121">Vereisten voor Azure-informatiebeveiliging</span><span class="sxs-lookup"><span data-stu-id="c83cb-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="c83cb-122">Azure Information Protection-client downloaden</span><span class="sxs-lookup"><span data-stu-id="c83cb-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
