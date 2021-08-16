---
title: Migratie van AIP naar MIP/Unified Labeling in het compliancecentrum
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000351"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migratie van AIP naar MIP/Unified Labeling in het compliancecentrum

Ga als volgt te werk om te migreren van AIP-labels naar Unified Labeling in het Beveiligings- en compliancecentrum:

**Beveiliging activeren vanuit de Azure-portal**

1. Als u dit nog niet hebt gedaan, opent u een nieuw browservenster en meld [u aan bij de Azure-portal.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Ga naar het **Azure Information Protection-blad.** Klik bijvoorbeeld in het hubmenu op **Alle services** en begin gegevens te **typen** in het vak Filter. Selecteer **Azure Information Protection**. Als u het Azure Information Protection-blad nog niet eerder [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) hebt geopend, bekijkt u de een-tijd extra stappen om dit blad toe te voegen aan de portal. Als u het Azure Information Protection-blade wilt openen, moet u een [Azure Information Protection-Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) of een Office 365-abonnement met Rights Management. Als u een van deze abonnementen hebt, maar een bericht ziet dat een geldig abonnement niet kan worden gevonden, [neem dan contact](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) op met Microsoft Support of gebruik uw standaardondersteuningskanalen.

2. Zoek de **menuopties** beheren en selecteer **Activering van beveiliging.** Klik **op Activeren** en bevestig uw actie. Wanneer de activering is voltooid, wordt op de informatiebalk **weergegeven dat activering is voltooid.**

**Azure Information Protection-labels migreren naar Office 365 beveiligingscentrum & compliancecentrum**

1. Zorg ervoor dat u bent aangemeld als gebruiker met de machtiging Globale beheerder.

2. Ga naar het **Azure Information Protection-blad.**

3. Selecteer unified labeling in **de** optie Menu **beheren.**

4. Klik op **azure information protection - Unified labeling** blade op **Activeren** en volg de onlineinstructies.

**Opmerking:** Controleer of u de juiste machtigingen hebt voordat u de migratie van & Beveiligingscentrum activeert. Zie deze artikelen voor meer informatie:

1. [Moet u een globale beheerder zijn om Azure Information Protection te configureren of kan ik delegeren aan andere beheerders?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Belangrijke informatie over beheerdersrollen na de migratie naar & compliancecentrum.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Zie Labels migreren voor meer informatie over de migratie van AIP naar Unified Labeling naar het Beveiligings- en [compliancecentrum.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
