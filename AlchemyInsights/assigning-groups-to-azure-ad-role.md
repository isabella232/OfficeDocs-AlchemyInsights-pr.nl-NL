---
title: Groepen toewijzen aan de functie Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884913"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Groepen toewijzen aan de functie Azure AD

Voer de volgende stappen uit om een Azure AD-groep met bron autoriteit in azure AD toe te wijzen aan een Azure AD-rol:

1. Maak een nieuwe groep om een nieuwe groep te maken:

    a. Meld u aan bij het Azure AD-Beheercentrum met bevoegdheden voor de **beheerder** of **globale beheerders** machtigingen.
    b. Selecteer **Azure Active Directory-> groepen > alle groepen > nieuwe groep**.
    c. Maak de groep.

2. Wijs tijdens het maken van groepen een rol toe aan de groep of nadat de groep is gemaakt.

    a. Als u tijdens het maken van een groep een rol wilt toewijzen aan de groep, kunt u overstappen op de wisselknop **Azure AD** en de groep maken.
    b. Als u een rol aan de groep wilt toewijzen nadat deze is gemaakt, gaat u naar het tabblad **toegewezen rollen** voor de nieuwe groep en wijst u de rol toe aan de groep.  

**Lidmaatschap van een groep beheren die is toegewezen aan de rol van Azure AD**

Om de verhoging van bevoegdheden te voorkomen, kunnen standaard alleen geprivilegieerde beheerders en globale beheerders het lidmaatschap van een groep wijzigen die aan een rol is toegewezen. Ze kunnen echter wel een eigenaar voor een dergelijke groep toewijzen en deze taak delegeren.

Zie voor meer informatie over het toewijzen van Cloud groepen aan Azure AD-rollen [een AD-rol toewijzen aan Cloud groep](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Zie voor meer informatie over het oplossen van rollen die zijn toegewezen aan Cloud groepen, [problemen oplossen met rollen die zijn toegewezen aan Cloud groepen](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





