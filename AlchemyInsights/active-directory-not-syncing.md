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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937096"
---
# <a name="active-directory-not-syncing"></a>Active Directory wordt niet gesynchroniseerd

Als u synchronisatiefouten ontvangt, zoals 'geen recente synchronisatie', of als u ziet dat de adreslijstsynchronisatiestatus in de beheerportal van Office zegt: 'Laatst gesynchroniseerd meer dan 3 dagen geleden', kan het zijn dat AADConnect onjuiste instellingen of onvoldoende machtigingen heeft om een synchronisatie uit te voeren.  

Als u AADConnect opnieuw installeert met behulp van express-instellingen, kan het probleem snel worden opgelost:

1. [Download de nieuwste versie van AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Volg de instructies voor het snel installeren.](/azure/active-directory/hybrid/how-to-connect-install-express)

Azure AD Connect moet worden geïnstalleerd op Windows Server 2012 of hoger. Deze server moet lid zijn van een domein en kan een domeincontroller of een lidserver zijn. Bekijk Vereisten voor Azure AD-Verbinding maken vereisten en vereisten voor [Azure AD-Verbinding maken.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Zie [Azure AD-Verbinding maken: Accounts en machtigingen](/azure/active-directory/hybrid/reference-connect-accounts-permissions)voor meer informatie over AADConnect-serviceaccounts.
