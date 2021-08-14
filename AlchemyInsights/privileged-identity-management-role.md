---
title: Privileged Identity Management rol
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
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973224"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) rol

**Machtigingen worden niet verleend na het activeren van een rol**

Wanneer u een rol activeert in Azure AD Privileged Identity Management (PIM), wordt de activering mogelijk niet direct doorgegeven aan alle portals waarvoor de bevoorrechte rol is vereist. Soms, zelfs als de wijziging wordt doorgevoerd, kan webcaching in een portal ertoe leiden dat de wijziging niet onmiddellijk van kracht wordt.

Als de activering is vertraagd, volgt u de volgende stappen:

1. Meld u af bij de Azure-portal en meld u weer aan. Wanneer u een Azure AD-rol of een Azure-resourcerol activeert, ziet u de stadia van de activering. Wanneer alle stadia zijn voltooid, ziet u een koppeling 'Uitloggen'. U kunt deze koppeling gebruiken om u af te melden. Hierdoor worden de meeste gevallen voor activeringsvertraging opgelost.
2. Controleer in PIM of u als lid van de rol wordt vermeld.
3. Als u de functie beheerder Exchange activeren, moet u zich aanmelden en zich opnieuw aanmelden. Als het probleem zich blijft voordoen, opent u een ondersteuningsticket en stelt u dit als een probleem aan de orde. Als u de rol Exchange beheerder gebruikt om toegang te krijgen tot het Beveiligings- en compliancecentrum, bekijkt u de volgende stap.
4. Als u een rol activeert om toegang te krijgen tot het Beveiligings- en compliancecentrum of als u de rol SharePoint Beheerder activeert, wordt er enige activeringsvertraging van enkele minuten tot enkele uren ervaren. Dit is een bekend probleem en we werken actief samen met deze teams om dit probleem zo snel mogelijk op te lossen.

Zie voor meer informatie:

- [Mijn Azure AD-rollen activeren in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Mijn Azure-resourcerollen activeren in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Machtigingen worden niet verwijderd nadat een rol is gedeactiveerd of de rolactivering verloopt**

Wanneer u een rol deactiveert in Azure AD Privileged Identity Management of wanneer een periode voor rollenactivering verloopt, kan er een vertraging zijn waarbij u nog steeds toegang hebt.

Als de deactivering is vertraagd, volgt u de volgende stappen:

1. Als u de rol van Exchange beheerder deactiveert of de periode voor rolactivering verloopt en u merkt dat er een aanzienlijke vertraging is voordat de machtigingen worden verwijderd, opent u een ondersteuningsticket en laat u uw ondersteuningsmedewerker weten dat u een ticket kunt indienen bij het PAM-team (Privileged Access Management) in Office over dit probleem.
2. Als de activeringsperiode is verlopen, maar de browsersessie nog steeds is geopend, sluit u de browser. U kunt de rol blijven gebruiken totdat u die sessie sluit. Dit is een bekend probleem en we kijken naar een mogelijke oplossing om elke sessie actief in te trekken zodra de activering is verlopen.

Als uw vertraging anders is dan deze twee scenario's, opent u een ondersteuningsticket.
