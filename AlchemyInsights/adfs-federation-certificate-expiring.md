---
title: ADFS-federatiecertificaat verloopt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710402"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-federatiecertificaat verloopt

Voer de volgende stappen uit om dit probleem op te lossen:
  
1. Installeer de Microsoft Azure Active Directory Module voor Windows PowerShell op de computer (als de module nog niet is geïnstalleerd). Ga hiervoor naar [Azure AD beheren met Windows PowerShell](https://aka.ms/aadposh).

2. Volg de stappen in het gedeelte 'Scenario 1: het AD FS-tokenondertekenencertificaat is verlopen' van [de fout 'Er was een probleem met de toegang tot de site' van AD FS wanneer een federatieve gebruiker zich aanmeldt bij Microsoft 365, Azure of Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Volg de stappen in [Bijwerken of herstellen van de instellingen van een federatief domein in Microsoft, Azure of Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Zie [Federatiecertificaten voor Microsoft 365 en Azure Active Directory vernieuwen voor](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)meer informatie over het vernieuwen van Federation-certificaten.
