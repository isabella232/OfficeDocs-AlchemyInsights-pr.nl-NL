---
title: AD FS-Federation verlopen certificaat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499886"
---
# <a name="adfs-federation-certificate-expiring"></a>AD FS-Federation verlopen certificaat

Dit probleem oplossen door de volgende stappen uit:
  
1. De Microsoft Azure Active Directory-Module voor Windows PowerShell installeren op de computer (als de module niet is geïnstalleerd). Ga hiervoor naar [Azure AD met Windows PowerShell beheren](https://aka.ms/aadposh).

2. Volg de stappen in de ' Scenario 1: de AD FS tokenhandtekeningcertificaat verlopen "sectie van het [foutbericht 'Er is een probleem met het openen van de site' van AD FS wanneer een federatieve gebruiker zich bij Office 365, Azure, of Intune aanmeldt](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Volg de stappen in [het bijwerken of herstellen van de instellingen van een federatieve domein in Office 365, Azure, of Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).

    Zie voor meer informatie over het vernieuwen van certificaten Federation, [federation-certificaten vernieuwen voor Office 365 en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
