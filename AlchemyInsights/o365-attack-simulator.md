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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801546"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="b9d3c-102">Aanvals Simulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b9d3c-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="b9d3c-103">Mist u aanvals Simulator?</span><span class="sxs-lookup"><span data-stu-id="b9d3c-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b9d3c-104">Voor de aanvals Simulator is **Microsoft Defender for Office 365 plan 2 (ATP abonnement 2)** of **Office 365 Enterprise E5** vereist.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="b9d3c-105">Er is **geen** aanvals Simulator opgenomen in Microsoft Defender for Office 365 plan 1 (ATP plan 1), Office 365 Enterprise E3 of microsoft 365-apps voor Business-abonnementen.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="b9d3c-106">Het account dat u gebruikt om gesimuleerde aanvallen te starten, vereist een globale beheerder of beveiligingsmachtigingen voor de beheerder en meervoudige verificatie (MFA).</span><span class="sxs-lookup"><span data-stu-id="b9d3c-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b9d3c-107">Zie [het volgende onderwerp](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor meer informatie over de vereisten voor een aanvals Simulator.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="b9d3c-108">Belangrijke dingen die u moet weten over zwakke beveiligings simulaties van **Grove wachtwoorden** :</span><span class="sxs-lookup"><span data-stu-id="b9d3c-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b9d3c-109">Als voor het doelaccount MFA is ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gemanipuleerd (de tweede verificatie factor is niet volledig).</span><span class="sxs-lookup"><span data-stu-id="b9d3c-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b9d3c-110">Het wachtwoordbestand mag niet groter zijn dan 10 MB.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b9d3c-111">Eén wachtwoord per regel gebruiken en een lege regel (regeleinde) toevoegen na het laatste wachtwoord in de lijst.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b9d3c-112">Belangrijke dingen die u moet weten over simulaties van de verbinding van **spear phishing** :</span><span class="sxs-lookup"><span data-stu-id="b9d3c-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b9d3c-113">U kunt geen aangepaste waarde voor de URL van de **phishingwebsite aannaam** geven</span><span class="sxs-lookup"><span data-stu-id="b9d3c-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="b9d3c-114">Als een geadresseerde de [invoegtoepassing voor het melden van berichten](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te rapporteren, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).</span><span class="sxs-lookup"><span data-stu-id="b9d3c-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b9d3c-115">Rapporten: nadat de gesimuleerde aanval is voltooid, kunt u op **Details aanval** klikken om het rapport te bekijken.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b9d3c-116">Zie [aanvals Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor uitgebreide instructies en nieuwe functies in aanvals Simulator.</span><span class="sxs-lookup"><span data-stu-id="b9d3c-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
