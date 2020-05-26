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
# <a name="aip-scanner-installation-and-configuration"></a>AIP-scanner: installatie en configuratie

**Als u de AIP-scanner wilt installeren, volgt u de aanbevolen richtlijnen:**

1. Als u een upgrade uitvoert en geen schone installatie uitvoert, moet u ervoor zorgen dat u de richtlijnen voor [het upgraden van de Azure Information Protection-scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) en voor uniforme etiketteringsclient hebt gevolgd, zie upgraden van de Azure Information [Protection-scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Controleer of u voldoet aan alle [vereisten voor firewalls en netwerkinfrastructuur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Zorg ervoor dat uw [beleid is ingesteld op](https://docs.microsoft.com/azure/information-protection/configure-policy) automatische etikettering of een standaardlabel in het beleid heeft.
4. Controleer of het relevante bestandstype is geconfigureerd voor label/beveiliging zoals beschreven in [bestandstypen die worden ondersteund door de Azure Information Protection-client.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Als u het standaardgedrag wilt wijzigen, volgt u bovendien de volgende richtlijnen: [Het standaardbeveiligingsniveau van bestanden wijzigen.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Controleer of het gebruikersaccount dat is geconfigureerd om de scannerservice uit te voeren, machtigingen heeft om toegang te krijgen tot alle geconfigureerde opslagplaatsen.
6. Als u nog steeds problemen ondervindt, exporteert u de scannerlogboeken en voegt u deze toe aan uw ondersteuningsticket.

**Azure Information Protection Scanner-logboeken exporteren**

1. Navigeer naar %localappdata%\Microsoft\MSIP onder de gebruikerscontext waarop de scannerservice wordt uitgevoerd.
2. Rits alle inhoud onder de MSIP-map.
3. Sla de logboeken op bij uw locatiekeuze en voeg ze toe aan uw serviceaanvraag.
4. U ook [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)gebruiken.

**Zie voor meer informatie**:
- [De Azure Information Protection-scanner implementeren om bestanden automatisch te classificeren en te beveiligen](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [De parameter Token opgeven en gebruiken voor Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Een detectiecyclus uitvoeren en rapporten voor de scanner weergeven](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Documentatie over Azure Information Protection controleren](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Vereisten voor Azure-informatiebeveiliging](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection-client downloaden](https://www.microsoft.com/download/details.aspx?id=53018)
