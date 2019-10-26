---
title: Dynamics 365 formulieren bedrijfsregels-zakelijke regel die niet wordt geactiveerd voor een formulier
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529014"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-gebeurtenis treedt niet op als het veld programmatisch wordt gewijzigd

De gebeurtenis *onchange* vindt niet plaats als het veld programmatisch wordt gewijzigd met het *kenmerk.* methode [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . Als u wilt dat gebeurtenis-handlers voor de gebeurtenis *onchange* worden uitgevoerd nadat u de waarde hebt ingesteld, moet u het *kenmerk formcontext. data. entity gebruiken.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -methode in uw code.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
