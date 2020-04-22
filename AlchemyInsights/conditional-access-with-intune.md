---
title: Voorwaardelijke toegang met Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706016"
---
# <a name="conditional-access-with-intune"></a>Voorwaardelijke toegang met Intune

Het gebruik **van voorwaardelijke toegang** met Intune vereist 3 stappen: 
  
- Maak een **beleid voor voorwaardelijke toegang** waarin wordt gedefinieerd welke resources worden beschermd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze bronnen. Een apparaat moet bijvoorbeeld compatibel zijn voordat het bedrijfse-mail inziet. 
    
- Maak een **nalevingsbeleid** om instellingen te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pin van ten minste 6 cijfers hebben voordat het als compatibel wordt beschouwd. 
    
- Ervoor zorgen dat zowel **nalevingsbeleid** als **beleid voor voorwaardelijke toegang** zijn gericht op de gewenste groepen gebruikers. Hiervoor moeten mogelijk specifieke groepen gebruikers worden gemaakt in Azure Active Directory. 
    
Lees meer:
  
- [Aanbevolen procedures voor voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Aan de slag met voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

