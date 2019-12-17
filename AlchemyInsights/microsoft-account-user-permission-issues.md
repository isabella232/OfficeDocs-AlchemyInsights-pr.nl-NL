---
title: Probleem oplossen-gebruiker niet gevonden in map
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054805"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6e9cb-102">Probleem oplossen-gebruiker niet gevonden in map</span><span class="sxs-lookup"><span data-stu-id="6e9cb-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6e9cb-103">Als gebruikersfout bericht ' gebruiker kan niet worden gevonden ' in de map ontvangt, probeert u opnieuw waar het probleem type is gebruiker niet in de map.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6e9cb-104">De volgende stappen kunnen worden voltooid om het probleem op te lossen.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6e9cb-105">Zorg ervoor dat het account dat de e-mail uitnodiging heeft geaccepteerd hetzelfde account is dat wordt gebruikt om later aan te melden.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6e9cb-106">Zorg ervoor dat de gebruiker hetzelfde account gebruikt om de uitnodiging te accepteren en zich aan te melden bij de site.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6e9cb-107">Zie voor meer informatie, [over het beheren van aliassen voor uw micro</a> Soft-account voor het beheren van de aanmelding bij Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="6e9cb-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6e9cb-108">Blader naar elke site (s) waarin de gebruiker de fout ontvangt.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6e9cb-109">Voeg '/_layouts/15/people.aspx/membershipgroupid = 0 ' (binnen de dubbele aanhalingstekens) toe aan het einde van de site-URL.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6e9cb-110">Voorbeeld: https://< ' Contoso ' >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6e9cb-111">Selecteer de gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-111">Select the user from the list.</span></span>

- <span data-ttu-id="6e9cb-112">Klik op **Gebruikersmachtigingen verwijderen** uit het lint.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6e9cb-113">Voeg de gebruiker terug en verzend de uitnodiging opnieuw naar de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="6e9cb-113">Add back the User and Resend the invite to the user.</span></span>

