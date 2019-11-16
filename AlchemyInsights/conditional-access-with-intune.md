---
title: Voorwaardelijke toegang met intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "36504989"
---
# <a name="conditional-access-with-intune"></a>Voorwaardelijke toegang met intune

Het gebruik van **voorwaardelijke toegang** met intune vereist 3 stappen: 
  
- Maak een **beleid voor voorwaardelijke toegang** waarin wordt gedefinieerd welke resources worden beveiligd en aan welke voorwaarden moet worden voldaan om toegang te krijgen tot deze resources. Een apparaat moet bijvoorbeeld compatibel zijn voordat u toegang tot zakelijke e-mail. 
    
- Maak een **nalevingsbeleid** om instellingen te definiëren waaraan moet worden voldaan voordat het apparaat als compatibel wordt beschouwd. Een apparaat moet bijvoorbeeld een pincode hebben van ten minste 6 cijfers voordat het als compatibel wordt beschouwd. 
    
- Ervoor te zorgen dat zowel **nalevingsbeleid** en **beleid voor voorwaardelijke toegang** zijn gericht op de gewenste groepen gebruikers. Dit kan nodig zijn voor het maken van specifieke groepen gebruikers in azure Active Directory. 
    
Lees meer:
  
- [Aanbevolen procedures voor voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [Aan de slag met voorwaardelijke toegang](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

