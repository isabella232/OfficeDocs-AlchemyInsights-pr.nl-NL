---
title: DLP heeft mogelijk een aangepast type nodig
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030789"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP heeft mogelijk een aangepast type nodig

**Belangrijk**: in deze ongekende tijden ondernemen we stappen om ervoor te zorgen dat SharePoint Online- en OneDrive-services optimaal beschikbaar blijven. Bezoek [Tijdelijke aanpassing van SharePoint Online-functies](https://aka.ms/ODSPAdjustments) voor meer informatie.

**Voor DLP is mogelijk een aangepast informatietype vereist**

Met een DLP-beleid (Data Loss Prevention) kunt u gevoelige gegevens in uw organisatie identificeren en beveiligen. In sommige scenario's moet u  mogelijk uw eigen aangepaste gevoelige informatietype maken om de gegevens van uw organisatie te beschermen.

Uw organisatie moet bijvoorbeeld werknemers-identiteiten of andere gegevens identificeren en beveiligen in een bepaalde indeling die specifiek is voor uw organisatie. In dat laatste artikel vindt u de volgende artikelen voor meer informatie.
  
 **Een ingebouwd type gevoelige informatie aanpassen**
  
Als een ingebouwd type gevoelige informatie met slechts enkele aanpassingen aan uw behoeften voldoet, kunt u een ingebouwde gevoelige [informatietype aanpassen.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) U kunt bijvoorbeeld trefwoorden toevoegen of verwijderen, of ondersteunend bewijs toevoegen of verwijderen, zoals een datum of adres.
  
 **Een aangepast type gevoelige informatie maken**
  
Maar als u een ander type gevoelige informatie moet identificeren en beveiligen, kunt u een aangepast type gevoelige informatie maken [in](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) de gebruikersinterface van het Beveiligings- & Compliancecentrum.
  
**Een aangepast type gevoelige informatie maken in het Beveiligings- en compliancecentrum PowerShell**

Als de gebruikersinterface niet alle opties biedt die u nodig hebt, kunt u [in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)een aangepast type gevoelige informatie maken. Door te beginnen met een XML-bestand, kunt u elke beschikbare optie gebruiken.
