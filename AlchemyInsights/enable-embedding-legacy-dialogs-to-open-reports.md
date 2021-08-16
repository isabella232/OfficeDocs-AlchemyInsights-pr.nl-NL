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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003384"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Schakel verouderde dialogen inbedden in op rapporten te openen

**Symptoom**

Gebruikers kunnen geen rapporten openen. "Er is iets misgegaan. Controleer technische details voor meer informatie."

**Oorzaak**

Rapporten kunnen niet uploaden in UCI met een fout. "Formulieromschrijving is null of niet omschreven." Rapporten in UCI vereisen nog steeds verouderde dialogen, dus moet het systeem van een klant nog steeds *allowlegacydialogsembedding* ingeschakeld hebben.

**Oplossing**

1. Ga naar **Instellingen >Administratie > Systeeminstellingen > Algemeen tabblad**.

2. Stel "Schakel inbeddeln van bepaalde verouderde dialogen in Unified Interface browser klant" in naar **Ja**.
