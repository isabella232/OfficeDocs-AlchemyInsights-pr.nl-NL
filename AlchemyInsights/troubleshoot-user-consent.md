---
title: Problemen met gebruikers instemming oplossen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900960"
---
# <a name="troubleshoot-user-consent"></a>Problemen met gebruikers instemming oplossen

1. U kunt configureren hoe eindgebruikers toestemming verlenen tot toepassingen via de Azure-portal of PowerShell. Zie [instellingen voor gebruikers toestemming](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) voor meer informatie.
1. Een beheerder kan de [API Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) ook gebruiken om toestemming te verlenen aan gedelegeerde machtigingen namens één gebruiker. Zie toegang verkrijgen namens [een gebruiker](https://docs.microsoft.com/graph/auth-v2-user)voor meer informatie.
1. [Fouten](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)in de gebruikersnamen: dit artikel bevat een beschrijving van de fouten die kunnen optreden tijdens de procedure voor het doorsturen van een toepassing. Als u problemen ondervindt bij het oplossen van onverwachte toestemmingen die geen foutberichten bevatten, raadpleegt u [verificatie scenario's voor Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).