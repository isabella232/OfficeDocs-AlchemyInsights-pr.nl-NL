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
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="a41ba-102">ADFS-federatie certificaat verloopt</span><span class="sxs-lookup"><span data-stu-id="a41ba-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="a41ba-103">Voer de volgende stappen uit om dit probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="a41ba-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="a41ba-104">Installeer de Microsoft Azure Active Directory-module voor Windows PowerShell op de computer (als de module nog niet is geïnstalleerd).</span><span class="sxs-lookup"><span data-stu-id="a41ba-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="a41ba-105">Ga hiervoor naar [Azure AD beheren met Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="a41ba-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="a41ba-106">Voer de stappen uit in het gedeelte ' scenario 1: het certificaat voor AD FS-ondertekening certificaat is verlopen ' in het gedeelte ' [Er is een fout opgetreden bij het openen van de site ' in AD FS wanneer een federatieve gebruiker zich aanmeldt bij Microsoft 365, Azure of intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="a41ba-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="a41ba-107">Volg de stappen in [de instellingen van een federatief domein in Microsoft, Azure of intune bijwerken of herstellen](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="a41ba-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="a41ba-108">Als u meer wilt weten over het verlengen van Federatie certificaten, raadpleegt u [Federatie certificaten voor Microsoft 365 en Azure Active Directory verlengen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="a41ba-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
