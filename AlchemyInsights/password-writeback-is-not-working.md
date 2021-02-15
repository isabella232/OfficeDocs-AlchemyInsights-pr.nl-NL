---
title: Wachtwoord terugschrijven werkt niet
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243289"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="c97c5-102">Wachtwoord terugschrijven werkt niet</span><span class="sxs-lookup"><span data-stu-id="c97c5-102">Password Writeback is not working</span></span>

<span data-ttu-id="c97c5-103">**Ik heb problemen met het configureren van wachtwoordin writeback**</span><span class="sxs-lookup"><span data-stu-id="c97c5-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="c97c5-104">Wachtwoord terugschrijven is een premium-functie.</span><span class="sxs-lookup"><span data-stu-id="c97c5-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="c97c5-105">Zorg ervoor dat u de licentievereisten begrijpt:</span><span class="sxs-lookup"><span data-stu-id="c97c5-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="c97c5-106">Er moet ten minste één licentie zijn toegewezen in uw organisatie</span><span class="sxs-lookup"><span data-stu-id="c97c5-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="c97c5-107">**Alleen cloudgebruikers:** betaalde SKU's voor Office 365 (O365) of Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="c97c5-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="c97c5-108">**Cloud- en/of on-premises** gebruikers: Azure AD Premium P1 of P2, Enterprise Mobility + Security (EMS) of Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="c97c5-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="c97c5-109">Zie Licentievereisten voor selfservice voor wachtwoord opnieuw instellen voor Azure AD voor meer informatie [over licentievereisten](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="c97c5-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="c97c5-110">U hebt ten minste één beheerdersaccount en één gebruikersaccount voor de test met een van de juiste licenties.</span><span class="sxs-lookup"><span data-stu-id="c97c5-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="c97c5-111">U moet Azure AD Connect verbinden met de Primaire domeincontroller Emulator om terugschrijven van wachtwoorden te laten werken.</span><span class="sxs-lookup"><span data-stu-id="c97c5-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="c97c5-112">U kunt Azure AD Connect configureren voor het gebruik  van een primaire domeincontroller door met de rechtermuisknop op de eigenschappen van de Active Directory-synchronisatieconnector te klikken en vervolgens adreslijstpartities **configureren te selecteren.**</span><span class="sxs-lookup"><span data-stu-id="c97c5-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="c97c5-113">Zoek hier de sectie verbindingsinstellingen voor de **domeincontroller** en vink het selectievakje aan met de naam **Alleen voorkeursdomeincontrollers gebruiken.**</span><span class="sxs-lookup"><span data-stu-id="c97c5-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="c97c5-114">Als de voorkeurs-DC geen PDC-emulator is, neemt Azure AD Connect nog steeds contact op met de PDC voor terugschrijven met een wachtwoord.</span><span class="sxs-lookup"><span data-stu-id="c97c5-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="c97c5-115">Wachtwoord opnieuw instellen is geconfigureerd en ingeschakeld in uw tenant.</span><span class="sxs-lookup"><span data-stu-id="c97c5-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="c97c5-116">Zie Gebruikers in staat stellen [hun Azure AD-wachtwoorden opnieuw in te stellen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="c97c5-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="c97c5-117">Zorg ervoor dat het administratoraccount dat wordt gebruikt voor het inschakelen van Wachtwoord terugschrijven een cloudbeheerdersaccount is (gemaakt in Azure AD, niet on-premises AD)</span><span class="sxs-lookup"><span data-stu-id="c97c5-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="c97c5-118">U hebt één on-premises implementatie of een on-premises AD-implementatie voor meerdere forest uitgevoerd Windows Server 2008 R2, Windows Server 2012 of Windows Server 2012 R2 met de nieuwste servicepacks geïnstalleerd</span><span class="sxs-lookup"><span data-stu-id="c97c5-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="c97c5-119">U hebt het hulpprogramma Azure AD Connect geïnstalleerd en u hebt uw AD-omgeving voorbereid voor synchronisatie met de cloud.</span><span class="sxs-lookup"><span data-stu-id="c97c5-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="c97c5-120">Voordat u wachtwoordschrijven test, moet u eerst een volledige import en volledige synchronisatie uitvoeren vanuit AD en Azure AD in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="c97c5-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="c97c5-121">Voor meer informatie, zie hoe u een volledige synchronisatie en volledige [import in Azure AD Connect kunt uitvoeren](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="c97c5-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="c97c5-122">**Ik heb een probleem met de connectiviteit voor terugschrijven met wachtwoorden**</span><span class="sxs-lookup"><span data-stu-id="c97c5-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="c97c5-123">De nieuwste versie van [Azure AD Connect downloaden en inschakelen](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="c97c5-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="c97c5-124">Firewallconfiguratie: Het hulpprogramma Azure AD Connect (1.1.443 en hoger) heeft uitgaande **HTTPS-toegang** nodig voor:</span><span class="sxs-lookup"><span data-stu-id="c97c5-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="c97c5-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c97c5-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="c97c5-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="c97c5-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="c97c5-127">Inactieve verbindingen ten minste 2-3 minuten laten aanhouden</span><span class="sxs-lookup"><span data-stu-id="c97c5-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="c97c5-128">**Ik heb nog steeds problemen met het terugschrijven van wachtwoorden**</span><span class="sxs-lookup"><span data-stu-id="c97c5-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="c97c5-129">Als u nog steeds problemen hebt, kunt u proberen de service voor wachtwoordschrijven in het hulpprogramma Azure AD Connect uit te stellen en opnieuw in teschakelen.</span><span class="sxs-lookup"><span data-stu-id="c97c5-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="c97c5-130">Voor meer informatie, zie hoe u wachtwoordschrijven uit- en [opnieuw inschakelen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="c97c5-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
