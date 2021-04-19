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
# <a name="aip-scanner-installation-and-configuration"></a>AIP-scanner: installatie en configuratie

**Als u de AIP-scanner wilt installeren, volgt u de aanbevolen richtlijnen:**

1. Als u een upgrade uitwerkt en geen schone installatie uitwerkt, controleert u of u de richtlijnen voor het upgraden van de [Azure Information Protection-scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) en voor geïntegreerde labelingclient hebt gevolgd, raadpleegt u het upgraden van de [Azure Information Protection-scanner.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Controleer of u voldoet aan alle instellingen voor firewalls en [netwerkinfrastructuur.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Zorg ervoor dat [uw beleid is ingesteld](https://docs.microsoft.com/azure/information-protection/configure-policy) op automatische labeling of een standaardlabel in het beleid heeft.
4. Zorg ervoor dat het desbetreffende bestandstype is geconfigureerd voor label/beveiliging, zoals beschreven in bestandstypen die worden ondersteund [door de Azure Information Protection-client.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Als u het standaardgedrag wilt wijzigen, volgt u de volgende richtlijnen: [Het standaardbeveiligingsniveau van bestanden wijzigen.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Controleer of het gebruikersaccount dat is geconfigureerd om de scannerservice uit te voeren, machtigingen heeft voor toegang tot alle geconfigureerde opslagplaatsen.
6. Als er nog steeds problemen zijn, exporteert u de scannerlogboeken en voegt u deze toe aan uw ondersteuningsticket.

**Azure Information Protection Scanner-logboeken exporteren**

1. Ga naar %localappdata%\Microsoft\MSIP onder de gebruikerscontext met de scannerservice.
2. Zip alle inhoud onder de map MSIP.
3. Sla de logboeken op de door u gekozen locatie op en voeg ze toe aan uw serviceverzoek.
4. U kunt ook [Export-AIPLogs -OnBehalfOf gebruiken.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Zie voor meer informatie:**
- [De Azure Information Protection-scanner implementeren om bestanden automatisch te classificeren en te beveiligen](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [De parameter Token opgeven en gebruiken voor Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Een detectiecyclus uitvoeren en rapporten voor de scanner weergeven](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure Information Protection-documentatie bekijken](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Vereisten voor Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection-client downloaden](https://www.microsoft.com/download/details.aspx?id=53018)
