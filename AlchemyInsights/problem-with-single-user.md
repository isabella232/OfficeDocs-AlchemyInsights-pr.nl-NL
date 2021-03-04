---
title: Probleem met één gebruiker
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429716"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="fffdd-102">Probleem met één gebruiker</span><span class="sxs-lookup"><span data-stu-id="fffdd-102">Problem with single user</span></span>

- <span data-ttu-id="fffdd-103">De gebruiker is mogelijk niet ingericht omdat de service de gebruiker nog niet heeft kunnen evalueren.</span><span class="sxs-lookup"><span data-stu-id="fffdd-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="fffdd-104">Bekijk de richtlijnen voor de tijd die nodig is voor de inrichting en voor de voortgangsbalk op de configuratiepagina voor inrichting.</span><span class="sxs-lookup"><span data-stu-id="fffdd-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="fffdd-105">Als de constante status die is opgegeven in de sectie met aanvullende gegevens vóór de datum valt waarop de gebruiker is gemaakt/bijgewerkt/verwijderd, betekent dit dat de gebruiker nog niet is geëvalueerd.</span><span class="sxs-lookup"><span data-stu-id="fffdd-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="fffdd-106">In dit scenario kunt u het beste wachten totdat de inrichtingsservice is voltooien.</span><span class="sxs-lookup"><span data-stu-id="fffdd-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="fffdd-107">Onze service is alleen op de hoogte van wijzigingen voor een gebruiker in het bronsysteem (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="fffdd-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="fffdd-108">Er moet een geldige wijziging zijn in het bronsysteem voor Azure AD om de wijziging te detecteren en deze door te stromen naar Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fffdd-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="fffdd-109">De inrichtingsservice heeft de gebruiker geëvalueerd en vastgesteld dat deze niet moet worden ingericht:</span><span class="sxs-lookup"><span data-stu-id="fffdd-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="fffdd-110">Als u een op een kenmerk gebaseerd bereikfilter hebt ingesteld, controleert u of de gebruiker voldoet aan de criteria die u hebt opgegeven.</span><span class="sxs-lookup"><span data-stu-id="fffdd-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="fffdd-111">Als er al gebruikers in het doelsysteem aanwezig zijn en de status van de gebruiker in de bron- en doel-overeenkomst, worden er geen verdere acties ondernomen.</span><span class="sxs-lookup"><span data-stu-id="fffdd-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="fffdd-112">Er is een poging ondernomen om de gebruiker in te inrichting. De inrichtingsservice is mislukt.</span><span class="sxs-lookup"><span data-stu-id="fffdd-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="fffdd-113">Voor deze scenario's bekijkt u het tabblad Probleemoplossing en aanbevelingen van de inrichtingslogboeken:</span><span class="sxs-lookup"><span data-stu-id="fffdd-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="fffdd-114">Een vereist kenmerk van de gebruiker ontbreekt mogelijk in on-premises Active Directory of Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fffdd-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="fffdd-115">De regels userPrincipalName of sAMAccountName genereren bijvoorbeeld niet de juiste waarde.</span><span class="sxs-lookup"><span data-stu-id="fffdd-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="fffdd-116">Het overeenkomende kenmerk (meestal employeeId) kan niet worden opgelost voor een unieke gebruiker in on-premises Active Directory of Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fffdd-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="fffdd-117">Er zijn bijvoorbeeld twee gebruikers met dezelfde employeeId in AD en de service retourneert een foutcode die dubbele doelgegevens aangeeft voor dezelfde broninvoer.</span><span class="sxs-lookup"><span data-stu-id="fffdd-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="fffdd-118">Zie De inrichtingslogboeken voor een probleem met een specifieke gebruiker bekijken als u logboeken voor één gebruiker en groepen [wilt bekijken.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="fffdd-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
