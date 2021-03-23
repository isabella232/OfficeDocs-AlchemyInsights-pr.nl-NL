---
title: Service Connection Point (SCP) configureren
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035450"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="1c863-102">Service connection Point (SCP) configureren</span><span class="sxs-lookup"><span data-stu-id="1c863-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="1c863-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="1c863-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="1c863-104">**Reden:** Kan het SCP-object niet lezen en de Azure AD-tenantgegevens verkrijgen</span><span class="sxs-lookup"><span data-stu-id="1c863-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="1c863-105">**Oplossing:** Raadpleeg de sectie [Een serviceverbindingspunt configureren](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="1c863-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="1c863-106">**Actieplan**</span><span class="sxs-lookup"><span data-stu-id="1c863-106">**Action plan**</span></span>

- <span data-ttu-id="1c863-107">Controleer of het apparaat het GPO voor de gecontroleerde validatie heeft ontvangen.</span><span class="sxs-lookup"><span data-stu-id="1c863-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="1c863-108">Controleer of het GPO de registersleutels heeft gemaakt.</span><span class="sxs-lookup"><span data-stu-id="1c863-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="1c863-109">Zorg ervoor dat u twee sleutels hebt gemaakt met uw Adreslijst-id en onmicrosoft-domein.</span><span class="sxs-lookup"><span data-stu-id="1c863-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="1c863-110">**Registerinstelling aan clientzijde configureren voor SCP**</span><span class="sxs-lookup"><span data-stu-id="1c863-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="1c863-111">Gebruik het volgende voorbeeld om een groepsbeleidsobject (GPO) te maken om een registerinstelling te implementeren die een SCP-item configureert in het register van uw apparaten.</span><span class="sxs-lookup"><span data-stu-id="1c863-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="1c863-112">Open een groepsbeleidsconsole en maak een nieuw GPO in uw domein.</span><span class="sxs-lookup"><span data-stu-id="1c863-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="1c863-113">Geef uw zojuist gemaakte GPO een naam (bijvoorbeeld ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="1c863-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="1c863-114">Bewerk het GPO en zoek het volgende pad: **Computerconfiguratie > voorkeuren > Windows-instellingen > Register**.</span><span class="sxs-lookup"><span data-stu-id="1c863-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="1c863-115">Klik met de rechtermuisknop op **Register** en selecteer **Nieuw > registeritem**.</span><span class="sxs-lookup"><span data-stu-id="1c863-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="1c863-116">Configureer **op het** tabblad Algemeen het volgende:</span><span class="sxs-lookup"><span data-stu-id="1c863-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="1c863-117">**Actie**: Bijwerken</span><span class="sxs-lookup"><span data-stu-id="1c863-117">**Action**: Update</span></span>
    
- <span data-ttu-id="1c863-118">**Bijenkorf**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="1c863-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="1c863-119">**Sleutelpad:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="1c863-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="1c863-120">**Waardenaam:** TenantId</span><span class="sxs-lookup"><span data-stu-id="1c863-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="1c863-121">**Waardetype**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="1c863-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="1c863-122">**Waardegegevens:** de GUID- of Adreslijst-id van uw Azure **AD-exemplaar**(Deze waarde vindt u in Azure Portal > Azure Active Directory > Properties > Directory ID )</span><span class="sxs-lookup"><span data-stu-id="1c863-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="1c863-123">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c863-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="1c863-124">Klik met de rechtermuisknop op **Register** en selecteer **Nieuw > registeritem**.</span><span class="sxs-lookup"><span data-stu-id="1c863-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="1c863-125">Configureer **op het** tabblad Algemeen het volgende:</span><span class="sxs-lookup"><span data-stu-id="1c863-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="1c863-126">**Actie**: Bijwerken</span><span class="sxs-lookup"><span data-stu-id="1c863-126">**Action**: Update</span></span>
    
- <span data-ttu-id="1c863-127">**Bijenkorf**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="1c863-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="1c863-128">**Sleutelpad:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="1c863-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="1c863-129">**Waardenaam:** TenantName</span><span class="sxs-lookup"><span data-stu-id="1c863-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="1c863-130">**Waardetype**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="1c863-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="1c863-131">**Waardegegevens:** uw geverifieerde domeinnaam als u federatief gebruik maakt van omgevingen zoals AD FS.</span><span class="sxs-lookup"><span data-stu-id="1c863-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="1c863-132">Uw geverifieerde domeinnaam of uw onmicrosoft.com domeinnaam (bijvoorbeeld contoso.onmicrosoft).com als u een beheerde omgeving gebruikt</span><span class="sxs-lookup"><span data-stu-id="1c863-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="1c863-133">Klik op **OK**.</span><span class="sxs-lookup"><span data-stu-id="1c863-133">Click **OK**.</span></span>

7. <span data-ttu-id="1c863-134">Sluit de editor voor het nieuwe GPO.</span><span class="sxs-lookup"><span data-stu-id="1c863-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="1c863-135">Koppel het zojuist gemaakte GPO aan de gewenste BOU met domeincomputers die deel uitmaken van uw gecontroleerde implementatiepopulatie.</span><span class="sxs-lookup"><span data-stu-id="1c863-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="1c863-136">Zie Gecontroleerde validatie van hybride [Azure AD-join - Azure AD-| Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="1c863-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









