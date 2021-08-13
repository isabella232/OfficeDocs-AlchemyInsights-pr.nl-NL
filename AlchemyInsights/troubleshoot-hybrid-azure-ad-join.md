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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939266"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Problemen met hybride Azure AD-join oplossen

Het wordt ten zeerste aanbevolen ervoor te zorgen dat een apparaat toegang heeft tot de eindpunten voor apparaatregistratie onder het systeemaccount met behulp van het [script Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Als je apparaatregistraties voor de eerste keer instelt, lees je eerst [Inleiding tot apparaatbeheer in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) voor meer informatie over het laten beheren van apparaten met Azure AD.
1. Als je apparaten rechtstreeks bij Azure AD registreert en deze inschrijft bij Intune, moet je [Intune hebben geconfigureerd](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) en een [licentie](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) hebben.
1. Zorg ervoor dat je bent gemachtigd om bewerkingen uit te voeren in Azure AD en on-premises AD. Alleen een globale beheerder in Azure AD kan instellingen voor apparaatregistraties beheren. Als je automatische registraties in je on-premises Active Directory instelt, moet je bovendien een beheerder zijn van Active Directory en AD FS (indien van toepassing).

Voor meer details over het oplossen van mogelijke problemen met hybride joins raadpleeg je [Problemen met hybride joins oplossen](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current). Voor het instellen van hybride Azure AD-joins en het beheer van apparaten met de Azure AD-portal raadpleeg je [Hybride Azure AD-joins (on-premises domein-joins) voor apparaten instellen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) en [Apparaten beheren met de Azure-portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Zie [Veelgestelde vragen over hybride Azure AD-joins](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq) voor het oplossen van veelvoorkomende problemen met hybride Azure AD-joins (Active Directory).
