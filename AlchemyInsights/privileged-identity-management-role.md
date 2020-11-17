---
title: Rollen van geprivilegieerde identiteitsbeheer
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
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088678"
---
# <a name="privileged-identity-managementpim-role"></a>De rol van bevoorrechte identiteitsbeheer (PIM)

**Machtigingen worden niet toegekend na het activeren van een rol**

Wanneer u een rol activeert in azure AD geprivilegieerde identiteitsbeheer (PIM), wordt de activering mogelijk niet onmiddellijk doorgegeven aan alle portals die de rol met bevoegdheden vereisen. Soms kan het gebeuren dat de wijziging niet onmiddellijk van invloed is op webcaches in een portal, zelfs als de wijziging wordt doorgevoerd.

Voer de volgende stappen uit als uw activering is vertraagd:

1. Meld u af bij de Azure-Portal en meld u vervolgens weer aan. Wanneer u een functie van Azure AD of een Azure-resource activeert, ziet u de fasen van de activering. Wanneer alle fasen zijn voltooid, wordt de link Afmelden weergegeven. U kunt deze koppeling gebruiken om u af te melden. Hiermee kunt u de meeste aanvragen voor activerings vertraging oplossen.
2. Zorg er in PIM voor dat u wordt vermeld als lid van de rol.
3. Zorg dat u zich afmeldt en opnieuw aanmeldt als u de rol van Exchange-beheerder activeert. Als het probleem zich blijft voordoen, opent u een ondersteuningsticket en verhoogt u dit als probleem. Als u de rol van Exchange-beheerder gebruikt om toegang te krijgen tot het beveiligings-en compliance-centrum, raadpleegt u de volgende stap.
4. Als u een rol activeert om toegang te krijgen tot het beleid voor beveiliging en compliance, of als u de SharePoint-beheerdersrol activeert, kunt u de activerings vertraging van enkele minuten tot enkele minuten tot een paar uur weer krijgen. Dit is een bekend probleem en we werken actief met deze teams om dit probleem zo snel mogelijk op te lossen.

Zie voor meer informatie:

- [Mijn Azure AD-rollen in PIM activeren](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Mijn Azure-resourcerollen in PIM activeren](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Machtigingen worden niet verwijderd na het deactiveren van een rol of de activering van rollen is verloopt**

Wanneer u een rol deactiveert op een Azure AD-identiteitsbeheer of wanneer een activeringsperiode voor rollen verloopt, is er mogelijk een vertraging waarbij u nog steeds toegang hebt.

Voer de volgende stappen uit als uw deactivering vertraagd is:

1. Als u de rol van Exchange-beheerder of de activeringsperiode voor rollen deactiveert en u merkt dat de machtigingen niet worden verwijderd, opent u een ondersteuningsticket en laat u uw ondersteuningsmedewerker weten dat u een ticket met het DRM-team (geprivilegieerde toegangsbeheer) in Office kunt vinden over dit probleem.
2. Als de activeringsperiode is verlopen, maar de browsersessie nog steeds is geopend, sluit u de browser. U kunt de rol blijven gebruiken totdat u deze sessie sluit. Dit is een bekend probleem en we bekijken een mogelijke oplossing voor het actief intrekken van elke sessie wanneer de activering is verlopen.

Als uw vertraging afwijkt van deze twee scenario's, kunt u een ondersteuningsticket openen.
