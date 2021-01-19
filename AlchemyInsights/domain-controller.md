---
title: Domeincontroller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900871"
---
# <a name="domain-controller"></a>Domeincontroller

**Kan AAD-DS niet activeren of de implementatie mislukt**

Voer de volgende stappen uit om het probleem van Azure AD Domain Service (AAD-DS) te verhelpen die niet is ingeschakeld of niet kan worden geïmplementeerd:

1. Als u een bestaand virtueel netwerk gebruikt, raadpleegt u uw NSG voor regels waarmee de poorten worden geblokkeerd die nodig zijn voor synchronisatie in AAD-DS in de portal https://aka.ms/aadds-networking .
2. Kijk of uw foutbericht in deze probleemoplossings handleiding is beantwoord, dat beschikbaar is in  https://aka.ms/aadds-troubleshoot-enable .
3. Probeer Azure AD Domain Services te implementeren in een nieuw, virtueel netwerk.
4. Volg de handleiding aan de slag voor het implementeren van AAD-DS, dat beschikbaar is in de [zelfstudie voor het maken van Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Als u problemen ondervindt met de implementatie van Azure AD Domain Services, raadpleegt u [problemen met Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) oplossen om veelvoorkomende fouten op te lossen zodat u ze weer kunt gebruiken. 

**Kan AAD-DS niet uitschakelen**

AAD-Active Directory kan niet worden onderbroken. Als u uw beheerde domein niet langer wilt gebruiken, moet deze worden verwijderd.

Als u problemen ondervindt bij het oplossen van veelvoorkomende foutberichten en de bijbehorende stappen voor het oplossen van problemen, raadpleegt u [problemen met Azure Active Directory Domain Services oplossen](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
