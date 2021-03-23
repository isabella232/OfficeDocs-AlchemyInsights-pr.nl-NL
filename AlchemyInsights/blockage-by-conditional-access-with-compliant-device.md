---
title: Ik word geblokkeerd door Voorwaardelijke toegang met compatibel apparaat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035370"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Ik word geblokkeerd door Voorwaardelijke toegang met compatibel apparaat

**Sterk aanbevolen hulpprogramma's**

- [Hulpprogramma voor probleemoplosser](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) voor apparaatregistratie: een uitgebreid hulpprogramma waarmee u de meest voorkomende problemen met apparaatregistratie kunt oplossen.
- [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) : een hulpmiddel dat wordt gebruikt om ervoor te zorgen dat een apparaat toegang heeft tot eindpunten voor apparaatregistratie onder het systeemaccount.
- [Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) : een hulpprogramma dat wordt gebruikt voor het zoeken en beheren van verouderde apparaten in uw omgeving.

Hier zijn enkele veelvoorkomende redenen waarom Voorwaardelijke toegang mogelijk mislukt  voor een compatibel apparaat of waarom uw gebruikers mogelijk ontvangen U kunt hier geen bericht ontvangen tijdens een aanmeldingsaanvraag bij een organisatieresource.

1. **Apparaat heeft geen vereiste apparaattoestand met een MDM:**

Controleer of het apparaat is geregistreerd bij een goedgekeurde MDM-provider, zoals Intune en *gemarkeerd als compatibel.* Zie dit document voor meer [informatie](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)over Intune. Zie Compliancebeleid gebruiken om regels in te stellen voor apparaten die u beheert met Intune voor meer informatie over apparaat compliance [en Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Als u problemen hebt met het registreren van een apparaat met Intune, vindt u meer informatie over het oplossen van problemen bij Het registreren van apparaten [in Microsoft oplossen.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) Maak een ondersteuningsaanvraag voor verdere Intune-ondersteuning. Ga daarom naar de pagina Help en [ondersteuning van Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Apparaat is niet verbonden met het netwerk van organisaties:**

Voor toegang tot organisatieresources moet het apparaat zijn verbonden met het netwerk van de organisatie, hetzij via een directe verbinding of een virtueel privénetwerk (VPN), maar ook verbonden met on-premises of Azure Active Directory. Zie Deelnemen aan uw werkapparaat aan het netwerk van uw organisatie als u wilt deelnemen aan een werkapparaat [aan het organisatienetwerk.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Zie Uw persoonlijke apparaat registreren op het netwerk van uw organisatie als u een persoonlijk/BYOD-apparaat [wilt registreren.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Als u wilt controleren of het apparaat deel heeft genomen aan het netwerk, kunt u de stappen voor geregistreerde apparaten [hier](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) volgen of hier [werken.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Als u het probleem wilt uitbreiden naar netwerkconnectiviteit op org, volgt u de onderstaande richtlijnen:

    1. Meld u aan bij Windows met uw werk- of schoolaccount, bijvoorbeeld alain@contoso.com.
    2. Maak verbinding met het netwerk van uw organisatie via een VPN of DirectAccess.
    3. Nadat u verbinding hebt, drukt u op **de Windows-logotoets+L om** uw apparaat te vergrendelen.
    4. Ontgrendel uw apparaat met uw werk- of schoolaccount en probeer vervolgens opnieuw toegang te krijgen tot de problematische app of service.

Als u het **foutbericht U kunt er vanaf** hier niet meer komen ziet, is het probleem waarschijnlijk ergens anders.

3. **Besturingssysteem wordt niet ondersteund:**

Controleer of u een ondersteunde versie van het besturingssysteem gebruikt, waaronder:

- **Windows Client:** Windows 7 of hoger

- **Windows Server**: Windows Server 2008 R2 of hoger

- **macOS**: macOS X of hoger

- **Android en iOS:** Nieuwste versie van mobiele besturingssystemen voor Android en iOS

4. **Webbrowser wordt niet ondersteund:**

Zoek hieronder ondersteunde browsers. Voor Chrome-ondersteuning met Windows 1703- of nieuwere versies is een windows 10-accountextensie vereist. Voor Edge 85+ moet de gebruiker zijn aangemeld om de nalevingsgegevens van het apparaat correct door te geven. Zie hier voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Beheerde browser in Intune, Safari
- **Android:** **Microsoft Edge:** Beheerde browser in Intune, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Hier vindt u meer informatie **over** de stappen voor het vinden van berichten en het oplossen van [problemen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
