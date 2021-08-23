---
title: Standaardinstelling Outlook label niet toegepast
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454567"
---
# <a name="default-outlook-label-setting-not-applied"></a>Standaardinstelling Outlook label niet toegepast

Als de standaardlabelinstellingen voor Outlook niet correct worden toegepast en er een ander label of geen label wordt toegepast, kan er een bekend probleem (MC277818) zijn en moet u een van de volgende 2 opties uitvoeren om het probleem op te lossen:

**Optie 1:**

1. Ga naar Microsoft 365 Compliance Center > **Solutions**  >  **Information Protection**.
1. Selecteer **Labelbeleid** en selecteer het labelbeleid dat u moet bewerken (**OutlookDefaultlabel-instelling** is niet correct ingesteld op het labelbeleid in kwestie. Voer **Get-labelpolicy uit om** deze instelling weer te geven en selecteer vervolgens Beleid **bewerken.**
1. Selecteer **Volgende** totdat u de instelling Dit standaardlabel toepassen op e-mailberichten **ziet,** die beschikbaar  is als u Gebruikers vereisen selecteert om een **label** toe te passen op e-mailberichten en documenten van de erfgenamen in het dialoogvenster Beleidsinstellingen.
1. Kies in **het dialoogvenster Een standaardlabel toepassen** op documenten de optie **Geen** in de vervolgkeuzelijst.
1. Selecteer **Volgende** en **Verzenden om** uw labelinstellingen op te slaan.

**Optie 2:**

Gebruik [in Powershell voor](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)beveiligings- en compliancecentrum de Set-LabelPolicy-opdracht om het **OutlookDefault-label** te wijzigen in **Geen** op de {OutlookDefaultLabel="None"}.

Uitvoeren: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

Zie Een ander standaardlabel instellen voor Outlook voor meer [informatie over standaardlabels voor Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)