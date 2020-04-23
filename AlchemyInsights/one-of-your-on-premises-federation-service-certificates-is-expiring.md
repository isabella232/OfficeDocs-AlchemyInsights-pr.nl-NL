---
title: Een van uw on-premises Federation Service-certificaten verloopt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785298"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="f897b-102">Een van uw on-premises Federation Service-certificaten verloopt</span><span class="sxs-lookup"><span data-stu-id="f897b-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="f897b-103">Voer de volgende stappen uit om dit probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="f897b-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="f897b-104">Installeer de Microsoft Azure Active Directory Module voor Windows PowerShell op de computer (als de module nog niet is geïnstalleerd).</span><span class="sxs-lookup"><span data-stu-id="f897b-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f897b-105">Ga hiervoor naar [Azure Active Directory PowerShell voor Grafiek](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="f897b-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="f897b-106">Volg de stappen in het gedeelte 'Scenario 1: het AD FS-tokenondertekenencertificaat is verlopen' van [de fout 'Er was een probleem met de toegang tot de site' van AD FS wanneer een federatieve gebruiker zich aanmeldt bij Microsoft 365, Azure of Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)</span><span class="sxs-lookup"><span data-stu-id="f897b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="f897b-107">Volg de stappen in [Het bijwerken of herstellen van de instellingen van een federatief domein in Microsoft 365, Azure of Intune.](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)</span><span class="sxs-lookup"><span data-stu-id="f897b-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="f897b-108">Zie [Certificaatverlenging voor O365 en Azure AD voor](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)meer informatie over het vernieuwen van Federatiecertificaten.</span><span class="sxs-lookup"><span data-stu-id="f897b-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

