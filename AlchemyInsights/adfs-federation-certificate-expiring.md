---
title: ADFS-Federation-certificaat verloopt
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
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737184"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-Federation-certificaat verloopt

Voer de volgende stappen uit om dit probleem op te lossen:
  
1. Installeer de Microsoft Azure Active Directory-module voor Windows PowerShell op de computer (als de module nog niet is geïnstalleerd). Ga hiervoor naar [Azure AD beheren met behulp van Windows PowerShell](https://aka.ms/aadposh).

2. Volg de stappen in de sectie ' scenario 1: de AD FS token-ondertekening certificaat verlopen ' van ' [Er is een probleem met het openen van de site ' fout van AD FS wanneer een federatieve gebruiker zich aanmeldt bij Office 365, Azure of intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Volg de stappen in [bijwerken of herstellen van de instellingen van een federatief domein in Office 365, Azure of intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Zie voor meer informatie over het vernieuwen van Federation-certificaten, [Federation-certificaten voor Office 365 en Azure Active Directory vernieuwen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
