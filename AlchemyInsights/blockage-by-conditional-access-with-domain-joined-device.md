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
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Ik word geblokkeerd door Voorwaardelijke toegang met een apparaat dat is verbonden met een domein

**Sterk aanbevolen hulpprogramma's**

[Hulpprogramma voor probleemoplosser](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) voor apparaatregistratie: het hulpprogramma waarmee u de meest voorkomende problemen met apparaatregistratie kunt oplossen.

[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : het script waarmee u ervoor kunt zorgen dat een apparaat toegang heeft tot eindpunten voor apparaatregistratie onder het systeemaccount.

[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) : het script waarmee u verouderde apparaten in uw omgeving kunt zoeken en beheren.

Hier zijn enkele veelvoorkomende redenen waarom voorwaardelijke toegang kan mislukken bij een apparaat dat deel heeft uit gemaakt van een domein (Hybride Azure AD).

1. **Er is geen Azure AD PRT** op het apparaat: u moet ervoor zorgen dat het apparaat Azure AD Primary Refresh Token (PRT) heeft. Zie dit document voor meer [informatie](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)over PRT.

Als u wilt controleren of u Azure AD PRT hebt, kunt u de opdracht uitvoeren op het apparaat en controleren of `dsregcmd/status` 'AzureAdPrt' gelijk is aan 'JA'.

Als 'AzureAdPrt' 'NEE' is, gaat u als volgt te werk:

- Of u nu een federatief omgeving met **AD FS** hebt en dat deze niet bereikbaar is vanuit de thuisnetwerken van uw gebruikers: In dit geval moet u ervoor zorgen dat uw 'gebruikersnaammixed' eindpunten toegankelijk zijn via het extranet. Als uw AD FS achter een VPN zit, zorgt u ervoor dat de gebruikers verbinding maken met de VPN en zich opnieuw aanmelden bij het apparaat. Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Of de TPM van** het apparaat defect is en dus het apparaat niet kan verifiëren: Controleer 'tpm.msc' om te zien of de status van TPM 'Ready' is. Zo niet, voer `dsregcmd/leave` het apparaat uit en laat het opnieuw deelnemen aan Azure AD. Probeer het vervolgens opnieuw. Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- U gebruikt een externe identiteitsprovider, die geen ondersteuning biedt **voor WS-Trust protocol.** Zoals wordt beschreven in onze documenten, kunnen hybride apparaten met Azure AD-apparaten in dit geval niet werken. Werk samen met uw identiteitsprovider voor ondersteuning.

2. Gebruikers gebruiken de Chrome-browser zonder de **Windows 10-accounts** of Office-extensie Chrome gebruikt de PRT niet automatisch op **AAD-apparaten** of hybride AAD-apparaten: Dit leidt tot het mislukken van elk beleid op basis van voorwaardelijke toegang op apparaten, met het foutbericht 'Niet-geregistreerd apparaat' weergegeven. Als u de Chrome-browser correct wilt gebruiken, moet u de 'Windows 10-accounts' of 'Office-extensie voor de Chrome-browser van de gebruikers' installeren via SCCM of Intune. Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Als het niet mogelijk is om de extensie op afstand te pushen, stelt u gebruikers op de hoogte om een van de bovenstaande extensies handmatig te installeren voor toegang tot toepassingen achter apparaatgebaseerde voorwaardelijke toegang. Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Het apparaat is correct hybride Azure AD samengevoegd, maar is per ongeluk verwijderd of uitgeschakeld, hetzij vanwege synchronisatiewijzigingen in Azure AD Connect of vanuit de **Azure-portal:** Als dit gebeurt, wordt het apparaatobject niet meer herkend als een volledig verbonden apparaat, ook al wordt de status 'AzureAdJoined' en 'PRT' als geldig op het apparaat weergeven.

Als u dit probleem wilt oplossen, wordt dit uitgevoerd op de betreffende apparaten en kunnen ze opnieuw aan `dsregcmd/leave` Azure AD gaan werken. Zie dit document voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Als uw apparaten windows 10, 1809 bijwerken met VPN/Cloudproxy en problemen zien met de status AzureAdPrt of een app met een SSO-probleem (outlook die geen verbinding maakt met postvak, zelfs als u PRT had), zorgt u ervoor dat u deze patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) of april cumulatieve update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) hebt om PRT-fouten op deze machines te voorkomen.

















