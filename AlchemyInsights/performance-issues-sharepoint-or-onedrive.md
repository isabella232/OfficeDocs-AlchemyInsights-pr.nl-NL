---
title: Prestatieproblemen-SharePoint of OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771896"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint of OneDrive traag, niet toegankelijk of niet beschikbaar voor meerdere gebruikers

Het is mogelijk dat SharePoint of OneDrive traag, niet toegankelijk of niet beschikbaar is, of dat de service niet beschikbaar is en de fouten in 503, om een aantal redenen:
  
- Als uw SharePoint-of OneDrive-site traag of vertraagd is voor meerdere gebruikers, is er mogelijk een tijdelijk serviceprobleem waarbij gebruikers een tijdelijke vertraging of navigatie fouten bij het openen van SharePoint-sites of OneDrive-inhoud kunnen vinden. Controleer het [Dashboard service status](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) om te zien of uw organisatie van invloed is.
  
- Gebruikers kunnen een fout bij een *503-Server* ontvangen bij het navigeren naar SharePoint-of OneDrive-sites. Deze fout kan worden veroorzaakt door de beperking binnen de SharePoint-service. SharePoint Online gebruikt beperking om optimale prestaties en betrouwbaarheid van de SharePoint Online-service te behouden. Dit beperkt het aantal gebruikersacties of gelijktijdige oproepen (via script of code) om overmatig gebruik van bronnen te voorkomen. Voor meer informatie over het beperken van beperking raadpleegt u [voorkomen dat u vertraagt of blokkeert in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Als u traag presteert met een **klassieke** of **moderne** SharePoint-site of-pagina, gebruikt u het [hulpprogramma](https://aka.ms/perftool) voor het maken van pagina's om de pagina's te analyseren.
  
- Als u nog steeds veel vertragingen onderneemt, raadpleegt u de bronnen onder aan dit artikel: [Inleiding tot het optimaliseren van de prestaties voor SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  