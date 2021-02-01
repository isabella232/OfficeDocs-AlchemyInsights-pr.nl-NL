---
title: Problemen met referenties
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063626"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="e1d8e-102">Problemen met referenties</span><span class="sxs-lookup"><span data-stu-id="e1d8e-102">Issues with credentials</span></span>

<span data-ttu-id="e1d8e-103">[In het Microsoft-identiteitsplatform en de stroom voor OAuth 2.0-clientreferenties](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) wordt beschreven hoe u rechtstreeks kunt programma's met de OAuth 2.0-clientgegevensstroom.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="e1d8e-104">**Hoe beheer ik het wachtwoord of certificaatreferenties van een toepassing?**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="e1d8e-105">In de Azure CLI kunt u de referenties van [az ad-app](https://docs.microsoft.com/cli/azure/ad/app/credential) gebruiken om het wachtwoord of certificaat van een toepassing te verwijderen, op te nemen in een lijst of opnieuw in te stellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="e1d8e-106">**Hoe kunnen mijn gebruikers hun wachtwoorden opnieuw instellen?**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="e1d8e-107">Gebruikers moeten zichzelf [registreren om zelf hun wachtwoord opnieuw in te stellen](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) voordat ze hun wachtwoorden opnieuw kunnen instellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="e1d8e-108">Wanneer een gebruiker zich heeft geregistreerd, kan deze de instructies in dit artikel volgen om het wachtwoord opnieuw in te stellen: Het wachtwoord van uw werk of [school opnieuw instellen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="e1d8e-109">**Hoe wijzigen mijn gebruikers hun wachtwoorden?**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="e1d8e-110">Gebruikers kunnen de stappen in dit artikel volgen om hun wachtwoorden te wijzigen: [Uw wachtwoord wijzigen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="e1d8e-111">Ze kunnen ook [app-wachtwoorden beheren voor verificatie in twee stappen.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="e1d8e-112">**Mijn gebruiker krijgt een foutmelding bij het wijzigen of opnieuw instellen van het wachtwoord**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="e1d8e-113">Deze koppeling geeft informatie over veelvoorkomende problemen die kunnen optreden wanneer een gebruiker zijn of haar wachtwoord opnieuw probeert in te [stellen: Algemene problemen en hun oplossingen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="e1d8e-114">**Ik heb problemen met het opnieuw instellen van het wachtwoord van een gebruiker**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="e1d8e-115">Zorg ervoor dat u bent gemachtigd om wachtwoorden opnieuw in te stellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="e1d8e-116">*Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen.*</span><span class="sxs-lookup"><span data-stu-id="e1d8e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="e1d8e-117">Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="e1d8e-118">Zorg ervoor dat u de licentievereisten begrijpt:</span><span class="sxs-lookup"><span data-stu-id="e1d8e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="e1d8e-119">Er moet ten minste één licentie zijn toegewezen in uw organisatie:</span><span class="sxs-lookup"><span data-stu-id="e1d8e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="e1d8e-120">**Alleen cloudgebruikers:** betaalde SKU's voor Office 365 (O365) of Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="e1d8e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="e1d8e-121">**Cloud- en/of on-premises** gebruikers: Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="e1d8e-122">Zie licentievereisten voor selfservice voor wachtwoord opnieuw instellen voor Azure AD voor meer informatie over [licentievereisten.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="e1d8e-123">Zoek de gebruiker in Azure AD om het wachtwoord van een gebruiker opnieuw in te stellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="e1d8e-124">Klik vervolgens op het overzichts blade voor die gebruiker op de knop Wachtwoord opnieuw instellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="e1d8e-125">**De knop Wachtwoord opnieuw instellen heeft een grijze kleur**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="e1d8e-126">U bent niet gemachtigd om wachtwoorden van **deze** gebruiker opnieuw in te stellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="e1d8e-127">*Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen.*</span><span class="sxs-lookup"><span data-stu-id="e1d8e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="e1d8e-128">Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="e1d8e-129">**Ik zie het wachtwoord niet om het blade opnieuw in te stellen**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="e1d8e-130">U bent niet gemachtigd om wachtwoorden opnieuw in te stellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="e1d8e-131">*Alleen globale gebruikers, wachtwoordbeheerders en gebruikersbeheerders kunnen wachtwoorden van gebruikers opnieuw instellen.*</span><span class="sxs-lookup"><span data-stu-id="e1d8e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="e1d8e-132">Globale beheerders kunnen ook wachtwoorden van andere bevoegde beheerders opnieuw instellen.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="e1d8e-133">**Ik zie het on-premises integratie blade niet in wachtwoord opnieuw instellen**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="e1d8e-134">De on-premises integratie blade wordt alleen weergegeven in hybride omgevingen, wat betekent dat u wachtwoordschrijven gebruikt om on-premises gebruikerswachtwoorden te manipuleren.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="e1d8e-135">U ziet dit blade niet als:</span><span class="sxs-lookup"><span data-stu-id="e1d8e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="e1d8e-136">U gebruikt wachtwoordschrijven niet</span><span class="sxs-lookup"><span data-stu-id="e1d8e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="e1d8e-137">Er is een probleem met de installatie/connectiviteit van wachtwoordopschrijven</span><span class="sxs-lookup"><span data-stu-id="e1d8e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="e1d8e-138">Er is een probleem met de installatie/connectiviteit van Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e1d8e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="e1d8e-139">Zie Problemen met wachtwoordopschrijven oplossen voor meer stappen voor het oplossen van problemen met [wachtwoordopschrijven.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="e1d8e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="e1d8e-140">**Ik weet niet hoe ik het wachtwoord van een gebruiker opnieuw moet instellen**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="e1d8e-141">Meld u aan bij de Azure Portal als een geschikte beheerder.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="e1d8e-142">Ga naar de **blade Gebruikers en groepen,** selecteer **Alle gebruikers.**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="e1d8e-143">Selecteer een gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="e1d8e-144">Selecteer Voor de geselecteerde gebruiker Overzicht **en** selecteer vervolgens Wachtwoord opnieuw instellen op de **opdrachtbalk.**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="e1d8e-145">Selecteer de **knop Wachtwoord opnieuw** instellen en volg de instructies op het scherm.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="e1d8e-146">Alleen resets uitgevoerd via de **ondersteuning van Azure Portal** bieden ondersteuning voor wachtwoordschrijven.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="e1d8e-147">**Ik stel het wachtwoord van een on-premises gebruiker opnieuw in vanuit de Office 365-beheerportal of de mobiele Office 365-toepassing, maar de gebruiker kan zich nog steeds niet aanmelden**</span><span class="sxs-lookup"><span data-stu-id="e1d8e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="e1d8e-148">Wachtwoord terugschrijven wordt niet ondersteund in deze portal.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="e1d8e-149">Stel het wachtwoord van de gebruiker opnieuw in in de Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="e1d8e-149">Reset the user's password again in the Azure portal.</span></span>
