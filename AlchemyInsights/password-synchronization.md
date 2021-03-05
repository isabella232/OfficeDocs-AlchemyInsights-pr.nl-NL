---
title: Wachtwoordsynchronisatie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481443"
---
# <a name="password-synchronization"></a><span data-ttu-id="b8135-102">Wachtwoordsynchronisatie</span><span class="sxs-lookup"><span data-stu-id="b8135-102">Password synchronization</span></span>

<span data-ttu-id="b8135-103">**Wachtwoord-hashsynchronisatie werkt helemaal niet**</span><span class="sxs-lookup"><span data-stu-id="b8135-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="b8135-104">Sommige veelvoorkomende problemen die klanten ondervinden wanneer wachtwoord-hashsynchronisatie niet werkt, zijn:</span><span class="sxs-lookup"><span data-stu-id="b8135-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="b8135-105">Aan het Active Directory-account dat door Azure AD Connect  wordt gebruikt  om te communiceren met on-premises Active Directory worden geen machtigingen verleend voor Repliceren directorywijzigingen en Repliceren Van alle( die zijn vereist voor wachtwoordsynchronisatie). U moet dit oplossen door deze machtigingen aan het Active Directory-account te verlenen.</span><span class="sxs-lookup"><span data-stu-id="b8135-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="b8135-106">Wachtwoord-hashsynchronisatie wordt uitgeschakeld nadat een beheerder de  methode User Sign-In heeft gewijzigd van Wachtwoordsynchronisatie in een andere optie, zoals Federatie  met **AD FS** in de wizard Azure AD Connect. U kunt dit oplossen door de functie voor wachtwoordhashsynchronisatie opnieuw in te stellen in de wizard Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="b8135-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="b8135-107">Verbindingsprobleem met on-premises Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b8135-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="b8135-108">Sommige domeincontrollers zijn bijvoorbeeld niet toegankelijk voor [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Azure AD Connect, of de vereiste poorten worden geblokkeerd door Firewall. U moet dit oplossen door ervoor te zorgen dat de verbinding tussen de Azure AD Connect-server en de on-premises Active Directory correct werkt.</span><span class="sxs-lookup"><span data-stu-id="b8135-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="b8135-109">De Azure AD Connect-server wordt momenteel in de testmodus uitgevoerd, waardoor de server geen toegang heeft tot de wachtwoordhashes. Om het probleem op te lossen, volgt u de stappen in sectie Problemen met wachtwoordsynchronisatie oplossen met [Azure AD Connect-synchronisatie -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)Er worden geen wachtwoorden gesynchroniseerd.</span><span class="sxs-lookup"><span data-stu-id="b8135-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="b8135-110">**Wachtwoord-hashsynchronisatie werkt niet voor sommige van mijn gebruikers**</span><span class="sxs-lookup"><span data-stu-id="b8135-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="b8135-111">Als het u is opgevallen dat wachtwoordhash  niet wordt gesynchroniseerd voor een gebruiker, gebruikt u de probleemoplossingstaak in Azure AD Connect om het probleem te onderzoeken en op te lossen.</span><span class="sxs-lookup"><span data-stu-id="b8135-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="b8135-112">Voer de volgende taken uit:</span><span class="sxs-lookup"><span data-stu-id="b8135-112">Perform the following tasks:</span></span>

    <span data-ttu-id="b8135-113">a.</span><span class="sxs-lookup"><span data-stu-id="b8135-113">a.</span></span> [<span data-ttu-id="b8135-114">De taak voor probleemoplossing in de wizard uitvoeren</span><span class="sxs-lookup"><span data-stu-id="b8135-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="b8135-115">b.</span><span class="sxs-lookup"><span data-stu-id="b8135-115">b.</span></span> [<span data-ttu-id="b8135-116">Gebruik de cmdlet probleemoplossing om het probleem met wachtwoordhashsynchronisatie voor een specifiek gebruik te onderzoeken</span><span class="sxs-lookup"><span data-stu-id="b8135-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="b8135-117">Het on-premises Active Directory User-object is ingeschakeld voor Gebruiker moet **het wachtwoord wijzigen bij de volgende aanmeldingsoptie.**</span><span class="sxs-lookup"><span data-stu-id="b8135-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="b8135-118">Wanneer deze optie is ingeschakeld, krijgt de gebruiker een tijdelijk wachtwoord toegewezen en wordt hem of haar gevraagd het wachtwoord te wijzigen bij de volgende aanmelding.</span><span class="sxs-lookup"><span data-stu-id="b8135-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="b8135-119">Tijdelijke wachtwoorden worden niet gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8135-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="b8135-120">Voer een van de volgende taken uit om het bovenstaande probleem op te lossen:</span><span class="sxs-lookup"><span data-stu-id="b8135-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="b8135-121">Vraag de gebruiker zich aan te melden bij de on-premises toepassing (bijvoorbeeld Windows-bureaublad) en het wachtwoord te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="b8135-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="b8135-122">Het nieuwe wachtwoord wordt gesynchroniseerd met Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b8135-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="b8135-123">Laat een beheerder het wachtwoord van de gebruiker bijwerken zonder de optie in teschakelen. Gebruiker moet het wachtwoord wijzigen bij de volgende aanmelding en het nieuwe wachtwoord delen met de gebruiker.</span><span class="sxs-lookup"><span data-stu-id="b8135-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="b8135-124">Het on-premises Active Directory User-object is niet **correct** geconfigureerd voor objectsynchronisatie of wachtwoordsynchronisatie.</span><span class="sxs-lookup"><span data-stu-id="b8135-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="b8135-125">Om dit probleem op te lossen, volgt u de stappen die worden beschreven in [wachtwoord-hashsynchronisatie oplossen met Azure AD Connect-synchronisatie.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="b8135-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







