---
title: Probleem met AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481463"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="d3102-102">Probleem met AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="d3102-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="d3102-103">Controleer of u gemachtigd bent om de bewerking uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="d3102-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="d3102-104">Globale beheerders hebben standaard toegang.</span><span class="sxs-lookup"><span data-stu-id="d3102-104">Global Admins have access by default.</span></span> <span data-ttu-id="d3102-105">Daarnaast kunt u toegangsbeheer op basis van rollen gebruiken [om](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) registratiemachtigingen te delegeren aan Inzender.</span><span class="sxs-lookup"><span data-stu-id="d3102-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="d3102-106">Zorg ervoor dat de vereiste eindpunten zijn ingeschakeld en niet worden geblokkeerd vanwege de firewall.</span><span class="sxs-lookup"><span data-stu-id="d3102-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="d3102-107">Zie de vereisten voor [meer informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="d3102-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="d3102-108">De registratie kan mislukken omdat uitgaande communicatie wordt onderworpen aan SSL-inspectie door de netwerklaag.</span><span class="sxs-lookup"><span data-stu-id="d3102-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="d3102-109">Controleer of u de instellingen voor meldingen voor Azure AD Connect Health hebt gecontroleerd.</span><span class="sxs-lookup"><span data-stu-id="d3102-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="d3102-110">Controleer de instelling.</span><span class="sxs-lookup"><span data-stu-id="d3102-110">Please review your setting.</span></span> <span data-ttu-id="d3102-111">In [deze handleiding](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) vindt u meer informatie over het configureren van de meldingsinstellingen voor statusmeldingen voor Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d3102-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="d3102-112">Zie het synchronisatierapport op objectniveau voor meer informatie over het synchronisatierapport voor AAD Connect Health en over het downloaden [ervan.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="d3102-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="d3102-113">Voor het oplossen van problemen met statusmeldingen voor [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) volgt u de gids voor het oplossen van problemen met de statusinformatie van AAD Connect en voor veelgestelde vragen, zie Veelgestelde vragen over de [AAD Connect-statusinstallatie.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="d3102-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
