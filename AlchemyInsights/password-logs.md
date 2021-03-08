---
title: Wachtwoordlogboeken
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525141"
---
# <a name="password-logs"></a><span data-ttu-id="8ea49-102">Wachtwoordlogboeken</span><span class="sxs-lookup"><span data-stu-id="8ea49-102">Password logs</span></span>

<span data-ttu-id="8ea49-103">**Ik heb problemen met het openen van auditlogboeken voor het opnieuw instellen van wachtwoorden**</span><span class="sxs-lookup"><span data-stu-id="8ea49-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="8ea49-104">Voer de volgende stap uit om problemen met betrekking tot toegang tot auditlogboeken voor wachtwoord opnieuw instellen op te lossen:</span><span class="sxs-lookup"><span data-stu-id="8ea49-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="8ea49-105">Controleer of u bevoegd bent om auditlogboeken weer te geven.</span><span class="sxs-lookup"><span data-stu-id="8ea49-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="8ea49-106">Alleen de volgende rollen zijn geautoriseerd:</span><span class="sxs-lookup"><span data-stu-id="8ea49-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="8ea49-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="8ea49-107">Global administrator</span></span>
 - <span data-ttu-id="8ea49-108">Beveiligingsbeheerder</span><span class="sxs-lookup"><span data-stu-id="8ea49-108">Security administrator</span></span>
 - <span data-ttu-id="8ea49-109">Beveiligingslezer</span><span class="sxs-lookup"><span data-stu-id="8ea49-109">Security reader</span></span>

<span data-ttu-id="8ea49-110">**Ik wil alle auditgebeurtenissen voor het opnieuw instellen van wachtwoorden zien vanaf het moment dat ik ze in eerste instantie heb geïmplementeerd**</span><span class="sxs-lookup"><span data-stu-id="8ea49-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="8ea49-111">Er worden maximaal 120.000 gebeurtenissen voor wachtwoord opnieuw instellen/registratie opgeslagen in de rapporten van de afgelopen 30 dagen.</span><span class="sxs-lookup"><span data-stu-id="8ea49-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="8ea49-112">Deze maximumlimiet is van toepassing op de gebruikersinterface bij het downloaden van de CSV.</span><span class="sxs-lookup"><span data-stu-id="8ea49-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="8ea49-113">Er zijn 1 miljoen gebeurtenissen beschikbaar via PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8ea49-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="8ea49-114">Zie de onderstaande koppelingen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="8ea49-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="8ea49-115">Selfservice voor wachtwoordresetgebeurtenissen vanuit de Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="8ea49-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8ea49-116">Registratiegebeurtenissen voor wachtwoord opnieuw instellen snel downloaden met PowerShell</span><span class="sxs-lookup"><span data-stu-id="8ea49-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="8ea49-117">**Ik wil meer weten over de rapportagemogelijkheden voor wachtwoord opnieuw instellen**</span><span class="sxs-lookup"><span data-stu-id="8ea49-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="8ea49-118">Controleer wie zich registreert voor wachtwoorden of stel deze opnieuw in met auditlogboeken voor het opnieuw instellen van wachtwoorden voor Azure AD in de Azure Portal onder **Gebruikers en groepen.**</span><span class="sxs-lookup"><span data-stu-id="8ea49-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="8ea49-119">Zie de volgende koppelingen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="8ea49-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="8ea49-120">Overzicht van rapporten voor wachtwoord opnieuw instellen</span><span class="sxs-lookup"><span data-stu-id="8ea49-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8ea49-121">Rapporten over het opnieuw instellen van wachtwoorden weergeven in de Azure Portal</span><span class="sxs-lookup"><span data-stu-id="8ea49-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8ea49-122">Selfservice voor wachtwoordresetgebeurtenissen vanuit de Azure AD Reports and Events API</span><span class="sxs-lookup"><span data-stu-id="8ea49-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="8ea49-123">Registratiegebeurtenissen voor wachtwoord opnieuw instellen snel downloaden met PowerShell</span><span class="sxs-lookup"><span data-stu-id="8ea49-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


