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
ms.openlocfilehash: 6170265dac1eebe8fa1acf766d2eb8d6b0a5908b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662358"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="736ce-102">AD FS-Federation verlopen certificaat</span><span class="sxs-lookup"><span data-stu-id="736ce-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="736ce-103">Dit probleem oplossen door de volgende stappen uit:</span><span class="sxs-lookup"><span data-stu-id="736ce-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="736ce-p101">De Microsoft Azure Active Directory-Module voor Windows PowerShell installeren op de computer (als de module niet is geïnstalleerd). Ga hiervoor naar [Azure AD met Windows PowerShell beheren](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="736ce-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="736ce-106">Volg de stappen in de ' Scenario 1: de AD FS tokenhandtekeningcertificaat verlopen "sectie van het [foutbericht 'Er is een probleem met het openen van de site' van AD FS wanneer een federatieve gebruiker zich bij Office 365, Azure, of Intune aanmeldt](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="736ce-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="736ce-107">Volg de stappen in [het bijwerken of herstellen van de instellingen van een federatieve domein in Office 365, Azure, of Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="736ce-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="736ce-108">Zie voor meer informatie over het vernieuwen van certificaten Federation, [federation-certificaten vernieuwen voor Office 365 en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="736ce-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

