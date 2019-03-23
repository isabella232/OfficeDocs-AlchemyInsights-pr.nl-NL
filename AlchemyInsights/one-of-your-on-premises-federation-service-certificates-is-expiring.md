---
title: Een van de certificaten op ruimten Federation Service verloopt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753025"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="2143f-102">Een van de certificaten op ruimten Federation Service verloopt</span><span class="sxs-lookup"><span data-stu-id="2143f-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="2143f-103">Dit probleem oplossen door de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="2143f-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="2143f-104">De Microsoft Azure Active Directory-Module voor Windows PowerShell installeren op de computer (als de module niet is geïnstalleerd).</span><span class="sxs-lookup"><span data-stu-id="2143f-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="2143f-105">Ga hiervoor naar [Azure Active Directory PowerShell voor grafiek](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="2143f-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="2143f-106">Volg de stappen in de ' Scenario 1: de AD FS tokenhandtekeningcertificaat verlopen "sectie van het [foutbericht 'Er is een probleem met het openen van de site' van AD FS wanneer een federatieve gebruiker zich bij Office 365, Azure, of Intune aanmeldt](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="2143f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="2143f-107">Volg de stappen in t[bijwerken of herstellen van de instellingen van een federatieve domein in Office 365, Azure, of Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="2143f-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="2143f-108">Zie voor meer informatie over het vernieuwen van certificaten Federation [certificaatvernieuwing voor O365 en Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="2143f-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

