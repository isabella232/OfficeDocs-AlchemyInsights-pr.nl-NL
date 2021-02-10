---
title: Een door de gebruiker toegewezen beheerde identiteit beheren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177462"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="3c5ef-102">Een door de gebruiker toegewezen beheerde identiteit beheren</span><span class="sxs-lookup"><span data-stu-id="3c5ef-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="3c5ef-103">Het beheer van een door de gebruiker toegewezen beheerde identiteit omvat:</span><span class="sxs-lookup"><span data-stu-id="3c5ef-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="3c5ef-104">Rollen toewijzen aan een door de gebruiker toegewezen beheerde identiteit</span><span class="sxs-lookup"><span data-stu-id="3c5ef-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="3c5ef-105">Een door de gebruiker toegewezen beheerde identiteit verwijderen</span><span class="sxs-lookup"><span data-stu-id="3c5ef-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="3c5ef-106">Een door de gebruiker toegewezen beheerde identiteit notatie geven</span><span class="sxs-lookup"><span data-stu-id="3c5ef-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="3c5ef-107">Zie de volgende artikelen voor meer informatie over de hierboven genoemde taken:</span><span class="sxs-lookup"><span data-stu-id="3c5ef-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="3c5ef-108">[Een door de gebruiker toegewezen](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) beheerde identiteit maken voor het toewijzen van rollen aan een door de gebruiker toegewezen beheerde identiteit</span><span class="sxs-lookup"><span data-stu-id="3c5ef-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="3c5ef-109">[Een door de gebruiker toegewezen beheerde](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) identiteit verwijderen - voor het verwijderen van een door de gebruiker toegewezen beheerde identiteit</span><span class="sxs-lookup"><span data-stu-id="3c5ef-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="3c5ef-110">[Een door de gebruiker toegewezen beheerde](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) identiteit op een lijst zetten voor een door de gebruiker toegewezen beheerde identiteit</span><span class="sxs-lookup"><span data-stu-id="3c5ef-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="3c5ef-111">Controleer of u de roltoewijzing **Inzender beheerde** identiteit hebt.</span><span class="sxs-lookup"><span data-stu-id="3c5ef-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="3c5ef-112">Deze roltoewijzing is vereist voor het maken/verwijderen van aan de gebruiker toegewezen beheerde identiteiten.</span><span class="sxs-lookup"><span data-stu-id="3c5ef-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
