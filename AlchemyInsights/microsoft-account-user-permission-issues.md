---
title: Probleem oplossen - Gebruiker niet gevonden in directory
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702733"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="a2b5f-102">Probleem oplossen - Gebruiker niet gevonden in directory</span><span class="sxs-lookup"><span data-stu-id="a2b5f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="a2b5f-103">Als gebruikers een foutbericht 'gebruiker kan niet niet worden gevonden' in de map ontvangen, probeert u het opnieuw waar het type probleem gebruiker niet in de map is.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="a2b5f-104">De volgende stappen kunnen worden voltooid om het probleem op te lossen.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="a2b5f-105">Zorg ervoor dat het account dat de e-mailuitnodiging heeft geaccepteerd, hetzelfde account is dat wordt gebruikt om later in te loggen.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="a2b5f-106">Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en u aan te melden bij de site.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="a2b5f-107">Zie [Aliassen beheren voor</a> uw Microsoft-account om de Microsoft 365-aanmelding te beheren voor](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="a2b5f-108">Blader naar elke site(s) waarin de gebruiker de fout ontvangt.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="a2b5f-109">Voeg "/_layouts/15/people.aspx/membershipgroupid=0" (binnen de dubbele aanhalingstekens) toe aan het einde van de SITE-URL.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="a2b5f-110">Voorbeeld: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="a2b5f-111">Selecteer de gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-111">Select the user from the list.</span></span>

- <span data-ttu-id="a2b5f-112">Klik **op Gebruikersmachtigingen verwijderen** van het lint.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="a2b5f-113">Voeg de gebruiker terug en stuur de uitnodiging opnieuw naar de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="a2b5f-113">Add back the User and Resend the invite to the user.</span></span>

