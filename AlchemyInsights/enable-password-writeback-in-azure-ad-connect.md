---
title: Wachtwoord terugschrijven inschakelen in Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093350"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e98a2-102">Wachtwoord terugschrijven inschakelen in Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e98a2-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e98a2-103">Als u het zelf terugschrijven voor wachtwoordherstel wilt inschakelen, moet u eerst de optie terugschrijven inschakelen in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e98a2-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e98a2-104">Voer de volgende stappen uit vanaf de Azure AD Connect-server:</span><span class="sxs-lookup"><span data-stu-id="e98a2-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e98a2-105">Meld u aan bij de Azure AD Connect-server en start de **Azure AD Connect**-configuratiewizard.</span><span class="sxs-lookup"><span data-stu-id="e98a2-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e98a2-106">Klik op de **welkomstpagina** op **Configureren**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e98a2-107">Klik op de pagina **Aanvullende taken** op **Synchronisatieopties aanpassen** en klik dan op **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e98a2-108">Voer op de pagina **Verbinding maken met Azure AD** de referenties van de globale beheerder voor uw Azure-tenant in en klik vervolgens op **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e98a2-109">Klik op de pagina's **Mappen verbinden** en **Domein/OE filteren** op **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e98a2-110">Selecteer op de pagina **Optionele functies** het vakje naast **Wachtwoord terugschrijven** en klik op **Volgende**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e98a2-111">Klik op de pagina **Klaar om te configureren** op **Configureren** en wacht tot het proces is voltooid.</span><span class="sxs-lookup"><span data-stu-id="e98a2-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e98a2-112">Wanneer u ziet dat de configuratie is voltooid, klikt u op **Afsluiten**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e98a2-113">Wanneer het terugschrijven van wachtwoorden is ingeschakeld in Azure AD Connect, configureert u Azure AD SSPR voor terugschrijven.</span><span class="sxs-lookup"><span data-stu-id="e98a2-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e98a2-114">Voer de volgende stappen uit om het terugschrijven van wachtwoorden in SSPR in te schakelen:</span><span class="sxs-lookup"><span data-stu-id="e98a2-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e98a2-115">Meld u aan bij Azure Portal met het globale beheerdersaccount.</span><span class="sxs-lookup"><span data-stu-id="e98a2-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e98a2-116">Zoek en selecteer **Azure Active Directory**, klik op **Wachtwoord opnieuw instellen** en klik vervolgens op **On-premises integratie**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e98a2-117">Stel de optie voor **Wachtwoorden terugschrijven naar uw on-premises directory?** in op **Ja**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e98a2-118">Stel de optie voor **Gebruikers toestaan accounts te ontgrendelen zonder het wachtwoord opnieuw in te stellen?** in op **Ja**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e98a2-119">Wanneer u klaar bent, klikt u op **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="e98a2-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e98a2-120">Zie [Zelf in Azure Active Directory terugschrijven voor wachtwoordherstel naar een on-premises omgeving inschakelen](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e98a2-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e98a2-121">Wanneer een beheerder het wachtwoord van een gebruiker opnieuw instelt in Azure Portal, wordt het wachtwoord teruggeschreven naar on-premises bij een federatieve gebruiker of synchronisatie met een wachtwoord-hash.</span><span class="sxs-lookup"><span data-stu-id="e98a2-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e98a2-122">Deze functionaliteit vereist een Azure Premium-licentie (P1 of P2) en wordt momenteel niet ondersteund op de Office-beheerportal.</span><span class="sxs-lookup"><span data-stu-id="e98a2-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
