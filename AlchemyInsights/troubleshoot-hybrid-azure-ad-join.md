---
title: Problemen met hybride Azure AD-join oplossen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401902"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Problemen met hybride Azure AD-join oplossen

Het wordt ten zeerste aanbevolen ervoor te zorgen dat een apparaat toegang heeft tot de eindpunten voor apparaatregistratie onder het systeemaccount met behulp van het [script Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Als u apparaatregistraties voor de eerste keer instelt, lees dan eerst I[nleiding tot apparaatbeheer in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) voor meer informatie over het laten beheren van apparaten door Azure AD.
1. Als u apparaten rechtstreeks bij Azure AD registreert en deze inschrijft bij Intune, moet u [Intune hebben geconfigureerd](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) en een [licentie](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) hebben.
1. Zorg ervoor dat u bent gemachtigd om bewerkingen uit te voeren in Azure AD en on-premises AD. Alleen een globale beheerder in Azure AD kan instellingen voor apparaatregistraties beheren. Als u automatische registraties in uw on-premises Active Directory instelt, moet u bovendien een beheerder zijn van Active Directory en AD FS (indien van toepassing).

Voor meer details over het oplossen van mogelijke problemen met hybride joins raadpleegt u [Problemen met hybride joins oplossen](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Voor het instellen van hybride Azure AD-gekoppeld en beheer van apparaten met Azure Ad portal raadpleegt u [Hybride Azure AD-gekoppeld (on-premises domeingekoppeld) apparaten instellen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) en [Apparaten beheren met Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Zie [Veelgestelde vragen over hybride Azure AD-join](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq) voor het oplossen van veelvoorkomende problemen met hybride Azure Active Directory (AD) join.
