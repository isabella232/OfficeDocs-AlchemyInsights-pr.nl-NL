---
title: 902 (Synchronisatiefouten als gevolg van dubbele objecten)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998784"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisatiefouten als gevolg van dubbele objecten

Mogelijk ontvangt u een van de volgende foutberichten wanneer adreslijstsynchronisatie wordt Microsoft 365:

- Kan dit object niet bijwerken in Microsoft Online Services omdat de volgende kenmerken die aan dit object zijn gekoppeld, waarden bevatten die mogelijk al zijn gekoppeld aan een ander object in uw lokale adreslijst.

- Er bestaat al een gesynchroniseerd object met hetzelfde proxyadres in uw Microsoft Online Services-adreslijst.

- Kan dit object niet bijwerken omdat de volgende kenmerken die aan dit object zijn gekoppeld, waarden bevatten die mogelijk al zijn gekoppeld aan een ander object in uw lokale adreslijstservices: UserPrincipalName.

Als u het probleem wilt identificeren en oplossen, downloadt en runt u het [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).

Zie [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)voor meer informatie.
