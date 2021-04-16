---
title: Schakel verouderde dialogen inbedden in op rapporten te openen
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814259"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Schakel verouderde dialogen inbedden in op rapporten te openen

**Symptoom**

Gebruikers kunnen geen rapporten openen. "Er is iets misgegaan. Controleer technische details voor meer informatie."

**Oorzaak**

Rapporten kunnen niet uploaden in UCI met een fout. "Formulieromschrijving is null of niet omschreven." Rapporten in UCI vereisen nog steeds verouderde dialogen, dus moet het systeem van een klant nog steeds *allowlegacydialogsembedding* ingeschakeld hebben.

**Oplossing**

1. Ga naar **Instellingen >Administratie > Systeeminstellingen > Algemeen tabblad**.

2. Stel "Schakel inbeddeln van bepaalde verouderde dialogen in Unified Interface browser klant" in naar **Ja**.
