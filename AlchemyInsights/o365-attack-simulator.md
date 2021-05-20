---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545721"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="04111-102">Attack Simulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="04111-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="04111-103">Ontbreekt Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="04111-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="04111-104">Voor Attack Simulator **is Microsoft Defender vereist Office 365 plan 2** of Office 365 Enterprise **E5.**</span><span class="sxs-lookup"><span data-stu-id="04111-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="04111-105">Attack Simulator is **niet** opgenomen in Microsoft Defender voor Office 365 abonnement 1, Office 365 Enterprise E3 of Microsoft 365-apps voor bedrijven abonnementen.</span><span class="sxs-lookup"><span data-stu-id="04111-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="04111-106">Voor het account dat u gebruikt om gesimuleerde aanvallen te starten, zijn machtigingen van globale beheerders of beveiligingsbeheerders en meervoudige verificatie (MFA) vereist.</span><span class="sxs-lookup"><span data-stu-id="04111-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="04111-107">Zie dit onderwerp voor meer informatie over de vereisten [voor](/microsoft-365/security/office-365-security/attack-simulator)Attack Simulator.</span><span class="sxs-lookup"><span data-stu-id="04111-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="04111-108">Belangrijke dingen die u moet weten over brute force-aanvalssimulaties: </span><span class="sxs-lookup"><span data-stu-id="04111-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="04111-109">Als het doelaccount MFA heeft ingeschakeld en het wachtwoord correct is geraden, wordt het account niet als gecompromitteerd (de tweede verificatiefactor is onvolledig).</span><span class="sxs-lookup"><span data-stu-id="04111-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="04111-110">Het wachtwoordbestand mag niet groter zijn dan 10 MB.</span><span class="sxs-lookup"><span data-stu-id="04111-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="04111-111">Gebruik één wachtwoord per regel en voeg na het laatste wachtwoord in de lijst een lege regel (retour van het vervoer) toe.</span><span class="sxs-lookup"><span data-stu-id="04111-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="04111-112">Belangrijke dingen die u moet weten over De phishing-nasimulaties van **de speer:**</span><span class="sxs-lookup"><span data-stu-id="04111-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="04111-113">U kunt geen aangepaste waarde opgeven voor de URL van de **phishing-aanmeldingsserver.**</span><span class="sxs-lookup"><span data-stu-id="04111-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="04111-114">Als een geadresseerde de invoegvoeging Rapportbericht [inschakelen](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te melden, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).</span><span class="sxs-lookup"><span data-stu-id="04111-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="04111-115">Rapporten: Nadat de gesimuleerde aanval is voltooid, kunt u op **Details van** aanvallen klikken om het rapport te bekijken.</span><span class="sxs-lookup"><span data-stu-id="04111-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="04111-116">Zie Attack Simulator in Microsoft 365 voor gedetailleerde instructies en [nieuwe functies in Attack Simulator.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="04111-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
