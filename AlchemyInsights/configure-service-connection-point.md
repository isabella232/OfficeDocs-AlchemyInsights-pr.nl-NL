---
title: Service Connection Point (SCP) configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035450"
---
# <a name="configure-service-connection-point-scp"></a>Service connection Point (SCP) configureren

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Reden:** Kan het SCP-object niet lezen en de Azure AD-tenantgegevens verkrijgen
- **Oplossing:** Raadpleeg de sectie [Een serviceverbindingspunt configureren](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Actieplan**

- Controleer of het apparaat het GPO voor de gecontroleerde validatie heeft ontvangen.
- Controleer of het GPO de registersleutels heeft gemaakt.
- Zorg ervoor dat u twee sleutels hebt gemaakt met uw Adreslijst-id en onmicrosoft-domein.

**Registerinstelling aan clientzijde configureren voor SCP**

Gebruik het volgende voorbeeld om een groepsbeleidsobject (GPO) te maken om een registerinstelling te implementeren die een SCP-item configureert in het register van uw apparaten.

1. Open een groepsbeleidsconsole en maak een nieuw GPO in uw domein.
     - Geef uw zojuist gemaakte GPO een naam (bijvoorbeeld ClientSideSCP)

2. Bewerk het GPO en zoek het volgende pad: **Computerconfiguratie > voorkeuren > Windows-instellingen > Register**.

3. Klik met de rechtermuisknop op **Register** en selecteer **Nieuw > registeritem**.

4. Configureer **op het** tabblad Algemeen het volgende:
  
- **Actie**: Bijwerken
    
- **Bijenkorf**: HKEY_LOCAL_MACHINE
    
- **Sleutelpad:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Waardenaam:** TenantId
    
- **Waardetype**: REG_SZ
    
- **Waardegegevens:** de GUID- of Adreslijst-id van uw Azure **AD-exemplaar**(Deze waarde vindt u in Azure Portal > Azure Active Directory > Properties > Directory ID )
 
- Klik op **OK**.
 
5. Klik met de rechtermuisknop op **Register** en selecteer **Nieuw > registeritem**.

6. Configureer **op het** tabblad Algemeen het volgende:
  
- **Actie**: Bijwerken
    
- **Bijenkorf**: HKEY_LOCAL_MACHINE
    
- **Sleutelpad:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Waardenaam:** TenantName
    
- **Waardetype**: REG_SZ
    
- **Waardegegevens:** uw geverifieerde domeinnaam als u federatief gebruik maakt van omgevingen zoals AD FS. Uw geverifieerde domeinnaam of uw onmicrosoft.com domeinnaam (bijvoorbeeld contoso.onmicrosoft).com als u een beheerde omgeving gebruikt

- Klik op **OK**.

7. Sluit de editor voor het nieuwe GPO.

8. Koppel het zojuist gemaakte GPO aan de gewenste BOU met domeincomputers die deel uitmaken van uw gecontroleerde implementatiepopulatie.

Zie Gecontroleerde validatie van hybride [Azure AD-join - Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









