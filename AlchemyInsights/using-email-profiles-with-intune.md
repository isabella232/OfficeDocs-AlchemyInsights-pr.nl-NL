---
title: E-mailprofielen gebruiken met Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554979"
---
# <a name="using-email-profiles-with-intune"></a>E-mailprofielen gebruiken met Intune

Intune kan worden gebruikt voor het maken en implementeren van e-mailprofielen voor de native (ingebouwde) e-mailclient op meerdere apparaatplatforms.

[Zie E-mailinstellingen toevoegen aan apparaten met Intune voor](https://docs.microsoft.com/intune/email-settings-configure)informatie over enkele beperkingen die zijn gekoppeld aan e-mailprofielen, waaronder de manier waarop de aanwezigheid van bestaande profielen wordt behandeld en hoe u e-mailprofielen verwijdert.

Zie voor meer informatie over het maken van e-mailprofielen voor elk apparaatplatform:

[Instellingen voor Android-apparaten voor het configureren van e-mail, verificatie en synchronisatie in Intune](https://docs.microsoft.com/intune/email-settings-android)  
[E-mailinstellingen voor iOS- en iPadOS-apparaten toevoegen in Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Instellingen voor e-mailprofiel in Microsoft Intune voor apparaten met Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Instellingen voor e-mailprofiel voor apparaten met Windows 10 in Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Veelvoorkomend synchronisatieprobleem**

**Een KNOX-e-mailprofiel op Android voorkomt dat gebruikerscontacten, agenda en taken worden gesynchroniseerd met gebruikersapparaten.**

Het KNOX-e-mailprofiel op Android KNOX biedt de beheerder de mogelijkheid om te bepalen welke inhoudstypen worden gesynchroniseerd met het apparaat door elk op ingeschakeld in te stellen.

Als de instelling voor een van de inhoudstypen is ingesteld op **Niet geconfigureerd** (het standaard), wordt dat inhoudstype niet automatisch gesynchroniseerd. Een gebruiker kan het gewenste inhoudstype rechtstreeks op het apparaat inschakelen, maar die configuratie wordt overschreven door de instelling Intune-beleid en de synchronisatie stopt voor dat inhoudstype.

