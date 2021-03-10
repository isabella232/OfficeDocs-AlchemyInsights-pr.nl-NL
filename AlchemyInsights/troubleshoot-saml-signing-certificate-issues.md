---
title: Problemen met SAML-ondertekeningscertificaat oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692909"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="6ad5c-102">Problemen met SAML-ondertekeningscertificaat oplossen</span><span class="sxs-lookup"><span data-stu-id="6ad5c-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="6ad5c-103">Voer de volgende aanbevolen stappen uit om het probleem met het SAML-handtekeningcertificaat op te lossen:</span><span class="sxs-lookup"><span data-stu-id="6ad5c-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="6ad5c-104">Wanneer u een bedrijfstoepassing toevoegt die SSO ondersteunt, wordt in Azure een certificaat gegenereerd dat het [SAML-handtekeningcertificaat wordt genoemd.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="6ad5c-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="6ad5c-105">Dit certificaat heeft een vervaldatum van 3 jaar.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="6ad5c-106">Zie De vervaldatum voor uw federatiecertificaat aanpassen en doorvernieuwen naar een nieuw certificaat als u de vervaldatum van uw certificaat [wilt wijzigen.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="6ad5c-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="6ad5c-107">Azure gebruikt dit certificaat om de SAML-tokens te ondertekenen die door de toepassing zijn aangevraagd en deze naar de toepassing te sturen voor een succesvolle eenmalige aanmelding.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="6ad5c-108">Download het certificaat van de Azure Portal en stuur het naar de leverancier van de toepassing om het SSO-proces te voltooien.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="6ad5c-109">Nadat dit proces is voltooid, vertrouwt uw toepassing dit certificaat en worden alle SAML-tokens die door dit certificaat zijn ondertekend, geaccepteerd door de toepassing.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="6ad5c-110">Als dit certificaat is verlopen, maakt u een nieuw certificaat, werk het bij naar de leverancier van de toepassing en maakt u het vervolgens actief aan de Azure-kant.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="6ad5c-111">Zie Een certificaat verlengen [dat binnenkort verloopt, voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="6ad5c-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="6ad5c-112">Als het certificaat verloopt, wordt de gebruiker niet geblokkeerd.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="6ad5c-113">[Voeg een e-mailadres toe voor meldingen](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) die moeten worden ontvangen voordat het huidige certificaat verloopt.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="6ad5c-114">Stap 4 is optioneel.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="6ad5c-115">Wijzig de opties voor SAML-certificaat ondertekening van een toepassing en het algoritme voor certificaat ondertekening.</span><span class="sxs-lookup"><span data-stu-id="6ad5c-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="6ad5c-116">Zie Opties voor het ondertekenen van certificaten en het [handtekeningsalgoritme wijzigen voor meer informatie.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="6ad5c-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

