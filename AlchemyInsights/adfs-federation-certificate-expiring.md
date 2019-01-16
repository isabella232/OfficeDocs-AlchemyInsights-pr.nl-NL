---
title: AD FS-Federation verlopen certificaat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/15/2019
ms.locfileid: "28284053"
---
# <a name="adfs-federation-certificate-expiring"></a>AD FS-Federation verlopen certificaat

Dit probleem oplossen door de volgende stappen uit:
  
1. De Microsoft Azure Active Directory-Module voor Windows PowerShell installeren op de computer (als de module niet is geïnstalleerd). Ga hiervoor naar [Azure AD met Windows PowerShell beheren](https://aka.ms/aadposh).
    
2. Volg de stappen in de ' Scenario 1: de AD FS tokenhandtekeningcertificaat verlopen "sectie van het [foutbericht 'Er is een probleem met het openen van de site' van AD FS wanneer een federatieve gebruiker zich bij Office 365, Azure, of Intune aanmeldt](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. Volg de stappen in [het bijwerken of herstellen van de instellingen van een federatieve domein in Office 365, Azure, of Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    Zie voor meer informatie over het vernieuwen van certificaten Federation, [federation-certificaten vernieuwen voor Office 365 en Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

