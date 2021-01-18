---
title: Domein service configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884984"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Kan AAD-DS niet activeren of de implementatie mislukt

Voer de volgende stappen uit om het probleem van Azure AD Domain Service (AAD-DS) te verhelpen die niet is ingeschakeld of niet kan worden geïmplementeerd:

1. Als u een bestaand virtueel netwerk gebruikt, raadpleegt u uw NSG voor regels waarmee de poorten worden geblokkeerd die nodig zijn voor synchronisatie in AAD-DS in de portal https://aka.ms/aadds-networking .
2. Kijk of uw foutbericht in deze probleemoplossings handleiding is beantwoord, dat beschikbaar is in  https://aka.ms/aadds-troubleshoot-enable .
3. Probeer Azure AD Domain Services te implementeren in een nieuw, virtueel netwerk.
4. Volg de handleiding aan de slag voor het implementeren van AAD-DS: [domein Services voor Aad maken en configureren](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Als u problemen ondervindt met de implementatie van Azure AD Domain Services, raadpleegt u [problemen met Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) oplossen om veelvoorkomende fouten op te lossen zodat u ze weer kunt gebruiken. 

**Kan AAD-DS niet uitschakelen**

AAD-Active Directory kan niet worden onderbroken. Als u uw beheerde domein niet langer wilt gebruiken, moet deze worden verwijderd.
Als u uw beheerde domein wilt verwijderen, raadpleegt u de [domein service Aad verwijderen](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



