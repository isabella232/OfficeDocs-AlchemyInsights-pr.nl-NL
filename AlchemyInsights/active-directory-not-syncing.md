---
title: Active Directory wordt niet gesynchroniseerd
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822846"
---
# <a name="active-directory-not-syncing"></a>Active Directory wordt niet gesynchroniseerd

Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie', of de adreslijstsynchronisatiestatus in de Office-beheerportal 'Laatst gesynchroniseerd meer dan 3 dagen geleden' ziet, kan het zijn dat AADConnect onjuiste instellingen of onvoldoende machtigingen heeft om een synchronisatie uit te voeren.  

Als u AADConnect opnieuw installeert met behulp van express-instellingen, kan het probleem snel worden opgelost:

1. [Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Volg de instructies voor het snel installeren.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)

Zie [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.
