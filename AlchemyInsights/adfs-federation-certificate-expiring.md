---
title: ADFS Federation Certificate Expiring
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 3ba6e6a6f93225bc843dfd1a028d31223f01280c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821946"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation Certificate Expiring

Als u dit probleem wilt oplossen, gaat u als volgt te werk:
  
1. Installeer de Microsoft Azure Active Directory-module voor Windows PowerShell op de computer (als de module nog niet is geïnstalleerd). Ga hiervoor naar [Azure AD beheren met Windows PowerShell.](https://aka.ms/aadposh)

2. Volg de stappen in de sectie 'Scenario 1: Het certificaat voor het ondertekenen van AD FS-tokens verlopen' van de fout 'Er is een probleem opgetreden bij het openen van de site' van AD FS wanneer een federatief gebruiker zich aanmeldt bij [Microsoft 365, Azure of Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Volg de stappen in De instellingen van een federatief domein [in Microsoft, Azure of Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)bijwerken of herstellen.

    Zie Federatiecertificaten voor [Microsoft 365](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)en Azure Active Directory verlengen voor meer informatie over het verlengen van federatiecertificaten.
