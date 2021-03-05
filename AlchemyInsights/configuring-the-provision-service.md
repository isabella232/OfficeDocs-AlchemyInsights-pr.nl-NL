---
title: De inrichtingsservice configureren
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481851"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="e2b3a-102">De inrichtingsservice configureren</span><span class="sxs-lookup"><span data-stu-id="e2b3a-102">Configuring the Provision service</span></span>

<span data-ttu-id="e2b3a-103">Voor automatische inrichting door gebruikers moet Azure AD geldige referenties hebben waarmee verbinding kan worden maken met de Web Services-API van Werkdag.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="e2b3a-104">Verder wordt met de knop Verbinding testen op de app Werkdag naar AD-gebruikers inrichting ook gevalideerd of er verbinding kan worden gemaakt met de Azure AD Connect Provisioning-agent die is gekoppeld aan het AD-domein.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="e2b3a-105">Als azure portal een fout retourneert bij het opslaan van de referenties, volgt u de onderstaande aanbevolen stappen:</span><span class="sxs-lookup"><span data-stu-id="e2b3a-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="e2b3a-106">Bevestig dat u het gebruikersaccount van het Workday Integration System hebt geconfigureerd, zoals vermeld in het gedeelte Voor zelfstudie de gebruiker van het integratiesysteem [configureren in Werkdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="e2b3a-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="e2b3a-107">Controleer of de Azure AD Connect Provisioning Agent Service actief is op uw on-premises Windows-server met behulp van de servicebeheerconsole.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="e2b3a-108">U kunt ook de status van de agent in de Azure Portal controleren door te klikken op de knop On-premises agenten weergeven.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="e2b3a-109">Zorg ervoor dat u de waarde voor het veld 'Gebruikersnaam werkdag' in de notatie username@workday-tenantnaam.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="e2b3a-110">Als de naam van de werkdag-tenant ontbreekt, mislukt de verificatie op werkdag.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="e2b3a-111">Als u de integratie met de tenant voor de implementatie van Werkdag configureert, houd dan rekening met de geplande downtime van uw werkdag-tenant.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="e2b3a-112">Op de werkdag is de tijd voor de implementatie van tenants gepland in het weekend (meestal van vrijdagnacht tot zaterdagochtend) en storingen van de connectiviteit tijdens deze downtime zijn een bekend probleem dat automatisch wordt opgelost zodra de implementatieten weer online zijn.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="e2b3a-113">In zeldzame gevallen kan deze fout ook worden weergegeven als het wachtwoord van de gebruiker van het integratiesysteem is gewijzigd vanwege het vernieuwen van de tenant of als het account is vergrendeld of verlopen.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="e2b3a-114">Controleer de status van de gebruiker van het integratiesysteem met uw werkdagbeheerder.</span><span class="sxs-lookup"><span data-stu-id="e2b3a-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="e2b3a-115">Zie Zelfstudie: Werkdag configureren voor het automatisch inrichten van gebruikers voor meer informatie over het configureren van de werkdag voor automatische [inrichting.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="e2b3a-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
