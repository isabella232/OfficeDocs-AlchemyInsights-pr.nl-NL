---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713461"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="7e41d-102">Attack Simulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7e41d-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="7e41d-103">Mis je Attack Simulator?</span><span class="sxs-lookup"><span data-stu-id="7e41d-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="7e41d-104">Attack Simulator vereist **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** of **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="7e41d-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="7e41d-105">Attack Simulator is **niet** opgenomen in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 of Microsoft 365 Apps voor zakelijke abonnementen.</span><span class="sxs-lookup"><span data-stu-id="7e41d-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="7e41d-106">Voor het account dat u gebruikt om gesimuleerde aanvallen uit te voeren, zijn algemene machtigingen voor beheerders of beveiligingsbeheerders en multi-factor authenticatie (MFA) vereist.</span><span class="sxs-lookup"><span data-stu-id="7e41d-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="7e41d-107">Zie [dit onderwerp](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin)voor meer informatie over de vereisten van Attack Simulator.</span><span class="sxs-lookup"><span data-stu-id="7e41d-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="7e41d-108">Belangrijke dingen die u moet weten over **Brute Force Password** aanval simulaties:</span><span class="sxs-lookup"><span data-stu-id="7e41d-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="7e41d-109">Als het doelaccount MFA heeft ingeschakeld en het wachtwoord correct is geraden, wordt het account niet weergegeven als gecompromitteerd (de tweede verificatiefactor is onvolledig).</span><span class="sxs-lookup"><span data-stu-id="7e41d-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="7e41d-110">Het wachtwoordbestand mag niet groter zijn dan 10 MB.</span><span class="sxs-lookup"><span data-stu-id="7e41d-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="7e41d-111">Gebruik één wachtwoord per regel en voeg een lege regel (vervoer retour) toe na het laatste wachtwoord in de lijst.</span><span class="sxs-lookup"><span data-stu-id="7e41d-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="7e41d-112">Belangrijke dingen die u moet weten over **Spear Phishing** voeg simulaties toe:</span><span class="sxs-lookup"><span data-stu-id="7e41d-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="7e41d-113">Door het ontwerp u geen aangepaste waarde opgeven voor **de URL van de phishing-inlogserver.**</span><span class="sxs-lookup"><span data-stu-id="7e41d-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="7e41d-114">Als een ontvanger de [invoegtoepassing Rapportbericht](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) inschakelen gebruikt om het bericht als phishing te melden, ontvangt u mogelijk geen waarschuwingen voor het bericht (omdat dit een gesimuleerde aanval is).</span><span class="sxs-lookup"><span data-stu-id="7e41d-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="7e41d-115">Rapporten: Nadat de gesimuleerde aanval is voltooid, u op **Aanvalsdetails** klikken om het rapport te bekijken.</span><span class="sxs-lookup"><span data-stu-id="7e41d-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="7e41d-116">Zie [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)voor gedetailleerde instructies en nieuwe functies in Attack Simulator.</span><span class="sxs-lookup"><span data-stu-id="7e41d-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
