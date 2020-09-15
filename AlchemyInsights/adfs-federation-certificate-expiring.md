---
title: ADFS-federatie certificaat verloopt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686709"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-federatie certificaat verloopt

Voer de volgende stappen uit om dit probleem op te lossen:
  
1. Installeer de Microsoft Azure Active Directory-module voor Windows PowerShell op de computer (als de module nog niet is geïnstalleerd). Ga hiervoor naar [Azure AD beheren met Windows PowerShell](https://aka.ms/aadposh).

2. Voer de stappen uit in het gedeelte ' scenario 1: het certificaat voor AD FS-ondertekening certificaat is verlopen ' in het gedeelte ' [Er is een fout opgetreden bij het openen van de site ' in AD FS wanneer een federatieve gebruiker zich aanmeldt bij Microsoft 365, Azure of intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Volg de stappen in [de instellingen van een federatief domein in Microsoft, Azure of intune bijwerken of herstellen](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Als u meer wilt weten over het verlengen van Federatie certificaten, raadpleegt u [Federatie certificaten voor Microsoft 365 en Azure Active Directory verlengen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
