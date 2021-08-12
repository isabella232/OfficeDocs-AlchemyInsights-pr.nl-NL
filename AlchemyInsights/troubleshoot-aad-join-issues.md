---
title: Problemen met Azure AD-join oplossen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939914"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Problemen met Azure AD-join oplossen

1. Als u apparaatregistraties voor de eerste keer instelt, controleert u of u Inleiding tot apparaatbeheer [in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) hebt bekeken, zodat u weet hoe u Apparaten onder het besturingselement naar Azure AD kunt verplaatsen. 
1. Als u apparaten rechtstreeks registreert bij Azure AD en deze registreert bij Intune, moet u ervoor zorgen dat u [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) hebt geconfigureerd en de licentie eerst [hebt](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) ingesteld.
1. Controleer of u gemachtigd bent om bewerkingen uit te voeren in Azure AD. Alleen een globale beheerder in Azure AD kan instellingen voor apparaatregistraties beheren.
1. Zie Azure AD Join plannen als u azure AD join [wilt implementeren.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Zie Veelgestelde vragen over [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) voor meer informatie over het oplossen van veelvoorkomende problemen met Azure AD Windows 10 join en zie Kan niet deelnemen aan [Windows 10 Pro-computer](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) met Azure AD - Moet een upgrade uitvoeren naar - Microsoft Community
