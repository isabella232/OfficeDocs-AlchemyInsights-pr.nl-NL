---
title: Dynamics 365 Forms Business Rules-bedrijfsregel niet geactiveerd voor een formulier
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711486"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="242d9-102">OnChange-gebeurtenis doet zich niet voor als het veld via programmacode wordt gewijzigd</span><span class="sxs-lookup"><span data-stu-id="242d9-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="242d9-103">De gebeurtenis *onchange* treedt niet op als het veld via programmacode wordt gewijzigd via het *kenmerk.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) , methode</span><span class="sxs-lookup"><span data-stu-id="242d9-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="242d9-104">Als u wilt dat gebeurtenis-handlers worden uitgevoerd nadat *u de waarde* hebt ingesteld, moet u de *formContext. data. entity. entity kenmerk* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) in uw code gebruiken.</span><span class="sxs-lookup"><span data-stu-id="242d9-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
