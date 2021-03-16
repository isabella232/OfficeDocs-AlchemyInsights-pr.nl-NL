---
title: De achtergrondservice voor Microsoft Search in Bing verwijderen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816125"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>De achtergrondservice voor Microsoft Search in Bing verwijderen

Als u de achtergrondservice voor Microsoft Search in Bing wilt verwijderen, kunt u de volgende oplossingen proberen:

1. Ga als volgt te werk om terug te keren naar de oorspronkelijke instellingen van de zoekmachine:

    a. Schakel de **wisselknop Bing gebruiken als standaardzoekmachine [uit.](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**

    b. [Ga naar het Microsoft 365-beheercentrum](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) en leeg de instelling die van invloed is op alle gebruikers in uw organisatie.

2. Als u de achtergrondservice van een afzonderlijk apparaat wilt verwijderen, moet u de volgende taken uitvoeren:

    a. Kies **Configuratiescherm > Programma's > programma's en functies**.

    b. Klik met de rechtermuisknop **op Microsoft Search in Bing** onder de lijst met geïnstalleerde programma's en klik vervolgens op **Verwijderen.**

3. Als u de achtergrondservice van meerdere apparaten in uw organisatie wilt verwijderen, meld u zich aan als beheerder en voer u de volgende opdracht uit in een script: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
