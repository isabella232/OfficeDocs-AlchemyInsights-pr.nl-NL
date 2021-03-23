---
title: Melding AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035431"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="23556-102">Melding AAD Connect</span><span class="sxs-lookup"><span data-stu-id="23556-102">Notification AAD Connect</span></span>

- <span data-ttu-id="23556-103">Controleer of u gemachtigd bent om de bewerking uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="23556-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="23556-104">Globale beheerders hebben standaard toegang.</span><span class="sxs-lookup"><span data-stu-id="23556-104">Global Admins have access by default.</span></span> <span data-ttu-id="23556-105">Daarnaast kunt u toegangsbeheer [op basis van rollen gebruiken](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) om registratiemachtigingen te delegeren aan Inzender.</span><span class="sxs-lookup"><span data-stu-id="23556-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="23556-106">Controleer of de vereiste eindpunten zijn ingeschakeld en niet worden geblokkeerd vanwege de firewall.</span><span class="sxs-lookup"><span data-stu-id="23556-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="23556-107">Zie vereisten voor [meer informatie.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="23556-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="23556-108">Registratie kan mislukken als gevolg van uitgaande communicatie die wordt onderworpen aan SSL-inspectie door de netwerklaag.</span><span class="sxs-lookup"><span data-stu-id="23556-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="23556-109">Controleer of u de meldingsinstellingen voor Azure AD Connect Health hebt geverifieerd en controleer uw instelling.</span><span class="sxs-lookup"><span data-stu-id="23556-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="23556-110">Zie deze handleiding voor meer informatie over het configureren van de meldingsinstellingen voor Azure AD Connect [Health-meldingen.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="23556-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="23556-111">Zie Synchronisatierapport op objectniveau voor meer informatie over het synchronisatierapport AAD Connect Health en hoe u het [downloadt.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="23556-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="23556-112">Als u problemen met AAD Connect Health Alerts wilt oplossen, volgt u de handleiding voor probleemoplossing voor [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) data freshness alerts en voor veelgestelde vragen, zie Veelgestelde [AAD Connect Health-installatievragen.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="23556-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
