---
title: 2681 aanvals Simulator in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305327"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="ba8b3-102">Aanvals Simulator in Office 365</span><span class="sxs-lookup"><span data-stu-id="ba8b3-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="ba8b3-103">Mist u Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="ba8b3-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="ba8b3-104">Voor aanvals Simulator is **office 365 Advanced Threat Protection Plan 2 (ATP-abonnement 2)** of **Office 365 Enterprise E5**vereist.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="ba8b3-105">Aanvals Simulator is **niet** opgenomen in Office 365 Advanced Threat Protection Plan 1 (ATP-abonnement 1), Office 365 Enterprise E3 of Office 365 Business-abonnementen.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="ba8b3-106">Het account dat u gebruikt voor het starten van gesimuleerde aanvallen vereist globale beheerder of beveiligingsbeheerder machtigingen en multi-factor Authentication (MFA).</span><span class="sxs-lookup"><span data-stu-id="ba8b3-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="ba8b3-107">Zie [dit onderwerp](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)voor meer informatie over de vereisten van de aanvals Simulator.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="ba8b3-108">Belangrijke dingen om te weten over **Brute Force Password** Attack simulaties:</span><span class="sxs-lookup"><span data-stu-id="ba8b3-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="ba8b3-109">Als de doelaccount MFA is ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gecompromitteerd (de tweede verificatiefactor is onvolledig).</span><span class="sxs-lookup"><span data-stu-id="ba8b3-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="ba8b3-110">Het wachtwoordbestand mag niet groter zijn dan 10 MB.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="ba8b3-111">Gebruik één wachtwoord per regel en neem een lege regel (Return) op na het laatste wachtwoord in de lijst.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="ba8b3-112">Belangrijke dingen om te weten over **spear phishing** attach simulaties:</span><span class="sxs-lookup"><span data-stu-id="ba8b3-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="ba8b3-113">U geen aangepaste waarde opgeven voor de URL van de **aanmeldingsserver van phishing**.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="ba8b3-114">Als een geadresseerde de [invoegtoepassingen rapportbericht inschakelen](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) gebruikt om het bericht als phishing te rapporteren, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).</span><span class="sxs-lookup"><span data-stu-id="ba8b3-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="ba8b3-115">Rapporten: nadat de gesimuleerde aanval is voltooid, u op **aanvals Details** klikken om het rapport te bekijken.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="ba8b3-116">Zie [aanvals Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor gedetailleerde instructies en nieuwe functies in de aanvals Simulator.</span><span class="sxs-lookup"><span data-stu-id="ba8b3-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
