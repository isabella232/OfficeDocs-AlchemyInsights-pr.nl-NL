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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769334"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="28e93-102">OnChange-gebeurtenis treedt niet op als het veld programmatisch wordt gewijzigd</span><span class="sxs-lookup"><span data-stu-id="28e93-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="28e93-103">De gebeurtenis *onchange* vindt niet plaats als het veld programmatisch wordt gewijzigd met het *kenmerk.* methode [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="28e93-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="28e93-104">Als u wilt dat gebeurtenis-handlers voor de gebeurtenis *onchange* worden uitgevoerd nadat u de waarde hebt ingesteld, moet u de methode *formcontext. data. entity attribuut* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) gebruiken in uw code.</span><span class="sxs-lookup"><span data-stu-id="28e93-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
