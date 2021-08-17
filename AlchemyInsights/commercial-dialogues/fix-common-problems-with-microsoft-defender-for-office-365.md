---
title: Veelvoorkomende problemen met Microsoft Defender oplossen voor Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 9104615baa5bf6dc91468912168e42ece6727eadd5330f1eb34e2a9170568b26
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898239"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Veelvoorkomende problemen met Microsoft Defender oplossen voor Office 365

Hier zijn enkele oplossingen voor veelvoorkomende problemen met Microsoft Defender voor Office 365:

- **Berichtvertraging**:

  Vertragingen in e-mailbezorging kunnen worden veroorzaakt door Safe Bijlagen scannen van berichten. Zie de beleidsinstellingen [Safe bijlagen voor meer informatie.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Fout-positieve of negatieve resultaten rapporteren:**

  Zie voor meer informatie [berichten en bestanden rapporteren aan Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Koppelingsbeveiliging Safe inschakelen:**

  1. Ga in Microsoft 365 Defender portal naar <https://security.microsoft.com/> **E-mail & Samenwerkingsbeleid** & \> **beleidsregels** \> **voor** \>   bedreigingsregels Safe koppelingen in de sectie Beleid.

     Als u rechtstreeks naar de pagina Safe **koppelingen wilt** gaan, gebruikt <https://security.microsoft.com/safelinksv2> u .

  2. Selecteer op **Safe pagina Koppelingen** het beleid door op de naam van het beleid te klikken.
  3. Ga als volgt te werk in het detail flyout dat wordt weergegeven:
     - Als u een nieuw beleid wilt toevoegen, **selecteert u + Maken.** Er wordt een wizard gelanceerd om u te helpen uw beleidsinstellingen te definiëren.
     - Als u een bestaand beleid wilt bewerken, selecteert u het beleid door op de naam van het beleid te klikken. Selecteer bewerken **in** de flyout details die wordt weergegeven in de **sectie Beveiligingsinstellingen.**
  4. Configureer **op de pagina** Beveiligingsinstellingen de volgende instellingen:
     - Schakel De **actie selecteren voor onbekende potentieel schadelijke URL's in berichten in.**
     - Selecteer **Veilige koppelingen toepassen op berichten die binnen de organisatie zijn verzonden.**

  Zie Beleidsregels voor koppelingen [instellen in Microsoft Defender voor Safe meer Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
