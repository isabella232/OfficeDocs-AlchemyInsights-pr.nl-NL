---
title: Active Directory synchroniseert niet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265156"
---
# <a name="active-directory-not-syncing"></a>Active Directory synchroniseert niet

Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie' of de status van adreslijstsynchronisatie in de Office-beheerportal opmerkt: 'Laatst gesynchroniseerd meer dan 3 dagen geleden', kan het zijn dat AADConnect onjuiste instellingen of onvoldoende heeft machtigingen om een synchronisatie uit te voeren.  

Het opnieuw installeren van AADConnect met behulp van expresinstellingen kan het probleem snel oplossen:

1. [Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Volg de instructies voor express installatie](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Zie [Azure AD Connect: Accounts en machtigingen](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.
