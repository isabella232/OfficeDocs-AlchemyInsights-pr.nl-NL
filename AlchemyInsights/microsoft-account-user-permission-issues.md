---
title: Maken en gebruiken van een gedeeld postvak
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762396"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="d7bf3-102">Oplossen van probleem - gebruiker is niet gevonden in de directory</span><span class="sxs-lookup"><span data-stu-id="d7bf3-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="d7bf3-103">Als gebruikers fout bericht "gebruiker kan niet worden gevonden' in de map ontvangt.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="d7bf3-104">Probeer het opnieuw wanneer het Type probleem is gebruiker niet in de directory.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="d7bf3-105">De volgende stappen kunnen worden uitgevoerd voor het oplossen van het probleem.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="d7bf3-106">Controleer de account die de e-mailuitnodiging dezelfde account die wordt gebruikt voor het later inloggen is geaccepteerd.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="d7bf3-107">Zorg ervoor dat de gebruiker de uitnodiging accepteren en inloggen op de site gebruikt dezelfde account.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="d7bf3-108">Zie voor meer info [aliassen voor uw Microsoft-account beheren</a> voor het beheren van aanmelding bij de Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="d7bf3-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="d7bf3-109">Ga naar elke site (s) waarin de fout wordt ontvangen van de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="d7bf3-110">Toevoegen "/ _layouts/15/people.aspx/membershipgroupid=0" (tussen de dubbele aanhalingstekens) aan het einde van de URL van de site.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="d7bf3-111">Voorbeeld: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="d7bf3-112">Selecteer de gebruiker uit de lijst.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-112">Select the user from the list.</span></span>

- <span data-ttu-id="d7bf3-113">Klik op **Gebruikersmachtigingen verwijderen** uit het lint.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="d7bf3-114">Toevoegen van de gebruiker en de uitnodiging te verzenden naar de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="d7bf3-114">Add back the User and Resend the invite to the user.</span></span>

