---
title: Dynamics 365 formulieren bedrijfsregels - zakelijke regel niet is geactiveerd voor een formulier
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747363"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>De gebeurtenis OnChange vindt niet plaats als u het veld via programmacode wordt gewijzigd

De *BijWijzigen* -gebeurtenis treedt niet op als het veld wordt gewijzigd via programmacode met behulp van het *attribuut.* de methode [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Als u wilt dat gebeurtenis-handlers voor de gebeurtenis *OnChange* uit te voeren nadat u de waarde moet u de *-kenmerk formContext.data.entity.* de methode [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) in uw code.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
