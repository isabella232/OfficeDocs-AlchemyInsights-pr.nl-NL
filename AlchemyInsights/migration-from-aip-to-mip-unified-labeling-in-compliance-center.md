---
title: Migratie van AIP naar MIP/Unified Labeling in het Compliance Center
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236359"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migratie van AIP naar MIP/Unified Labeling in het Compliance Center

Ga als volgt te werk om van AIP-labels naar Unified Labeling in het beveiligings- en compliancecentrum te migreren:

**Beveiliging activeren vanuit de Azure-portal**

1. Als u dit nog niet hebt gedaan, opent u een nieuw browservenster en [meldt u zich aan bij de Azure-portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Navigeer naar het azure **information protection-blad.** Klik bijvoorbeeld in het hubmenu op **Alle services** en typ **gegevens** in het vak Filter. Selecteer **Azure Information Protection**. Als u het Azure Information Protection-blad nog niet eerder hebt geopend, raadpleegt u de [eenmalige extra stappen](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) om dit blad aan de portal toe te voegen. Als u het azure information protection-blad wilt openen, moet u een [Azure Information Protection Premium-abonnement](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) of een Office 365-abonnement hebben dat rechtenbeheer bevat. Als u een van deze abonnementen hebt, maar een bericht ziet dat een geldig abonnement niet kan worden gevonden, neemt [u contact op met Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) of gebruikt u uw standaardondersteuningskanalen.

2. Zoek de **menuopties beheren** en selecteer **Beveiligingsactivering**. Klik **op Activeren**en bevestig uw actie. Wanneer de activering is voltooid, wordt op de informatiebalk **activering weergegeven die is voltooid.**

**Azure Information Protection-labels migreren naar Office 365-beveiliging & Compliance Center**

1. Zorg ervoor dat u bent ingelogd als gebruiker met toestemming van globale beheerder.

2. Navigeer naar het azure **information protection-blad.**

3. Selecteer **Unified labeling**in de **menuoptie Beheren** .

4. Klik op het **Azure Information Protection - Unified-labelblad** op **Activeren** en volg de online instructies.

**Opmerking:** controleer of u over de juiste machtigingen beschikt voordat u de migratie van security & Compliance Center activeert. Zie deze artikelen voor meer info:

1. [Moet u een globale beheerder zijn om Azure Information Protection te configureren of kan ik delegeren aan andere beheerders?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Belangrijke informatie over administratieve rollen na migratie naar Security & Compliance Center.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Zie [Labels migreren](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)voor meer informatie over de AIP naar Unified Labeling-migratie naar Beveiligings- en Compliancecenter.
