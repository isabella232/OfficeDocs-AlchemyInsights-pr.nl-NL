---
title: 902 (Synchronisatiefouten veroorzaakt door dubbele objecten)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708057"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synchronisatiefouten veroorzaakt door dubbele objecten

Mogelijk ontvangt u een van de volgende foutberichten wanneer adreslijstsynchronisatie is bereikt in Microsoft 365:

- Kan dit object niet bijwerken in Microsoft Online Services omdat de volgende kenmerken die zijn gekoppeld aan dit object waarden hebben die mogelijk al zijn gekoppeld aan een ander object in uw lokale adreslijst.

- Er bestaat al een gesynchroniseerd object met hetzelfde proxyadres in uw Microsoft Online Services-adreslijst.

- Dit object kan niet worden bijgewerkt omdat de volgende kenmerken die aan dit object zijn gekoppeld, waarden hebben die mogelijk al zijn gekoppeld aan een ander object in uw lokale adreslijstservices: UserPrincipalName.

U kunt het probleem identificeren en oplossen door [idFix DirSync Error Remediation Tool te](https://github.com/Microsoft/idfix)downloaden en uit te voeren.

Zie [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)voor meer informatie.
