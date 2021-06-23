---
title: SMTP-verificatie en probleemoplossing inschakelen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077646"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="7b77a-102">SMTP-verificatie en probleemoplossing inschakelen</span><span class="sxs-lookup"><span data-stu-id="7b77a-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="7b77a-103">Als u SMTP-verificatie wilt inschakelen voor een postvak of als u een fout 'Client niet geverifieerd' of 'Verificatie mislukt' of 'SmtpClientAuthentication' krijgt met code 5.7.57 of 5.7.3 of 5.7.139 wanneer u e-mail probeert door te sturen door een apparaat of toepassing te verifiëren met Microsoft 365, voert u deze drie acties uit om het probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="7b77a-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="7b77a-104">Schakel de [Azure-beveiligings defaults uit](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) door Beveiligingsinstellingen inschakelen te wijzigen **in** **Nee.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="7b77a-105">a.</span><span class="sxs-lookup"><span data-stu-id="7b77a-105">a.</span></span> <span data-ttu-id="7b77a-106">Meld u aan bij de Azure-portal als beveiligingsbeheerder, beheerder van voorwaardelijke toegang of globale beheerder.</span><span class="sxs-lookup"><span data-stu-id="7b77a-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="7b77a-107">b.</span><span class="sxs-lookup"><span data-stu-id="7b77a-107">b.</span></span> <span data-ttu-id="7b77a-108">Blader naar Azure Active Directory > **Eigenschappen.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="7b77a-109">c.</span><span class="sxs-lookup"><span data-stu-id="7b77a-109">c.</span></span> <span data-ttu-id="7b77a-110">Selecteer **Beveiligingsinstellingen beheren.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="7b77a-111">d.</span><span class="sxs-lookup"><span data-stu-id="7b77a-111">d.</span></span> <span data-ttu-id="7b77a-112">Stel **Beveiligingsinstellingen inschakelen in** op **Nee.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="7b77a-113">e.</span><span class="sxs-lookup"><span data-stu-id="7b77a-113">e.</span></span> <span data-ttu-id="7b77a-114">Kies **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="7b77a-114">Select **Save**.</span></span>

2. <span data-ttu-id="7b77a-115">[Smtp-inzending van client inschakelen](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) in het gelicentieerde postvak.</span><span class="sxs-lookup"><span data-stu-id="7b77a-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="7b77a-116">a.</span><span class="sxs-lookup"><span data-stu-id="7b77a-116">a.</span></span> <span data-ttu-id="7b77a-117">Ga in Microsoft 365-beheercentrum naar **Actieve gebruikers** en selecteer de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="7b77a-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="7b77a-118">b.</span><span class="sxs-lookup"><span data-stu-id="7b77a-118">b.</span></span> <span data-ttu-id="7b77a-119">Ga naar het tabblad E-mail en selecteer onder **E-mail-apps** de optie **E-mail-apps beheren.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="7b77a-120">d.</span><span class="sxs-lookup"><span data-stu-id="7b77a-120">d.</span></span> <span data-ttu-id="7b77a-121">Controleer of **Geverifieerde SMTP** is ingeschakeld (ingeschakeld).</span><span class="sxs-lookup"><span data-stu-id="7b77a-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="7b77a-122">e.</span><span class="sxs-lookup"><span data-stu-id="7b77a-122">e.</span></span> <span data-ttu-id="7b77a-123">Selecteer **Wijzigingen opslaan**.</span><span class="sxs-lookup"><span data-stu-id="7b77a-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="7b77a-124">[Meervoudige verificatie (MFA) uitschakelen in](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) het gelicentieerde postvak.</span><span class="sxs-lookup"><span data-stu-id="7b77a-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="7b77a-125">a.</span><span class="sxs-lookup"><span data-stu-id="7b77a-125">a.</span></span> <span data-ttu-id="7b77a-126">Ga naar de Microsoft 365-beheercentrum en selecteer gebruikers actieve gebruikers in het  >  **linkernavigatiemenu.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="7b77a-127">b.</span><span class="sxs-lookup"><span data-stu-id="7b77a-127">b.</span></span> <span data-ttu-id="7b77a-128">Selecteer **Meervoudige verificatie**.</span><span class="sxs-lookup"><span data-stu-id="7b77a-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="7b77a-129">c.</span><span class="sxs-lookup"><span data-stu-id="7b77a-129">c.</span></span> <span data-ttu-id="7b77a-130">Selecteer de gebruiker en schakel **Multi-Factor auth uit.**</span><span class="sxs-lookup"><span data-stu-id="7b77a-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
