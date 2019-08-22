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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529014"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>De gebeurtenis OnChange vindt niet plaats als u het veld via programmacode wordt gewijzigd

De *BijWijzigen* -gebeurtenis treedt niet op als het veld wordt gewijzigd via programmacode met behulp van het *attribuut.* de methode [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Als u wilt dat gebeurtenis-handlers voor de gebeurtenis *OnChange* uit te voeren nadat u de waarde moet u de *-kenmerk formContext.data.entity.* de methode [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) in uw code.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
