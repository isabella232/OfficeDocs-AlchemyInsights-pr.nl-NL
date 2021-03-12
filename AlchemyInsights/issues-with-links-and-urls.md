---
title: Problemen met koppelingen en URL's
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707877"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="e3e87-102">Problemen met koppelingen en URL's</span><span class="sxs-lookup"><span data-stu-id="e3e87-102">Issues with links and URLs</span></span>

<span data-ttu-id="e3e87-103">Redirect URI/reply-URL's (beide uitdrukkingen worden gebruikt) zijn URL's die gebruikt worden door het Microsoft identity platform om tokens die door de app aangevraagd werden terug te geven.</span><span class="sxs-lookup"><span data-stu-id="e3e87-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="e3e87-104">Zie de volgende artikelen voor meer informatie:</span><span class="sxs-lookup"><span data-stu-id="e3e87-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="e3e87-105">[Verificatiestromen en toepassingsscenario's](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios): Informatie over de redirect URI's in de pagina **App-registratie** voor elk scenario.</span><span class="sxs-lookup"><span data-stu-id="e3e87-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="e3e87-106">Beperkingen voor URI/reply-URL's</span><span class="sxs-lookup"><span data-stu-id="e3e87-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="e3e87-107">**Ik weet niet hoe de juiste redirect URI/reply URL te registreren voor mijn app**</span><span class="sxs-lookup"><span data-stu-id="e3e87-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="e3e87-108">Wanneer je je aanmeldt bij de toepassing die je aan het ontwikkelen bent, moet je, als het aanmeldingsdialoogvenster **AADSTS50011: De reply-url die werd opgegeven in de aanvraag komt niet overeen met de reply url's die zijn geconfigureerd voor de toepassing <your app ID>** wordt weergegeven, de redirect URI toevoegen die gebruikt werd door de code in de token-aanvraag aan het Microsoft identity platform aan de registratie van jouw toepassing.</span><span class="sxs-lookup"><span data-stu-id="e3e87-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="e3e87-109">Voeg een reply URL toe door naar het tabblad **Verificatie** te gaan in de pagina **Registratie van toepassing** in het Azure Portal en voer het in de sectie **Redirect URI's**.</span><span class="sxs-lookup"><span data-stu-id="e3e87-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="e3e87-110">De waarde die je moet invoeren hangt af van het type toepassing dat je aan het bouwen bent, zoals beschreven hieronder:</span><span class="sxs-lookup"><span data-stu-id="e3e87-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="e3e87-111">Voor toepassing van een enkele pagina en web-apps is de reply URL een URL in jouw toepassing.</span><span class="sxs-lookup"><span data-stu-id="e3e87-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="e3e87-112">Zie [Registratie van enkele-paginatoepassing](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) of [Een web-app registreren met Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="e3e87-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="e3e87-113">Voor desktop-apps hangt de waarde die je nodig hebt af van:</span><span class="sxs-lookup"><span data-stu-id="e3e87-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="e3e87-114">het platform (MacOS verschilt van Windows en Linux)</span><span class="sxs-lookup"><span data-stu-id="e3e87-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="e3e87-115">de manier waarop je een token verkrijgt (interactief, met codestroom van apparaat, met geïntegreerde Windows-verificatie [IWA] of met gebruikersnaam/wachtwoord).</span><span class="sxs-lookup"><span data-stu-id="e3e87-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="e3e87-116">Voor meer informatie, zie [Desktop-apps - app-registratie- redirect URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="e3e87-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="e3e87-117">Voor mobiele toepassingen hangt de URI af van:</span><span class="sxs-lookup"><span data-stu-id="e3e87-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="e3e87-118">het platform (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="e3e87-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="e3e87-119">de informatie die werd gebruikt bij het bouwen van de app, zoals de bundel-id in iOS en de naam van het pakket en handtekening hash op Android. De Azure Portal-appregistratie helpt je hierbij.</span><span class="sxs-lookup"><span data-stu-id="e3e87-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="e3e87-120">Voor meer informatie, zie [Platformconfiguratie en redirect URI's](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="e3e87-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="e3e87-121">Web API's en enkele stille manieren om tokens te verkrijgen (IWA en gebruikersnaam/wachtwoord) vereisen geen redirect URI.</span><span class="sxs-lookup"><span data-stu-id="e3e87-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="e3e87-122">**Ik heb mijn webtoepassing geïmplementeerd en ik krijg een reply url mismatch-bericht wanneer ik de geïmplementeerde app uitprobeer**</span><span class="sxs-lookup"><span data-stu-id="e3e87-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="e3e87-123">Voeg redirect URI's toe voor alle locaties waarop je de webtoepassing implementeert.</span><span class="sxs-lookup"><span data-stu-id="e3e87-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="e3e87-124">Voor meer informatie, zie [Web-app registreren met Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="e3e87-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="e3e87-125">Voeg redirect URI toe aan een locatie van zodra je er de app geïmplementeerd hebt.</span><span class="sxs-lookup"><span data-stu-id="e3e87-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="e3e87-126">**Ik kan niet genoeg reply URL's registreren**</span><span class="sxs-lookup"><span data-stu-id="e3e87-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="e3e87-127">Je bent een Independent Software Vendor en hebt een of meerdere redirect URI's voor elke klant.</span><span class="sxs-lookup"><span data-stu-id="e3e87-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="e3e87-128">Je wilt migreren van ADAL/Azure AD v1.0 naar MSAL/Microsoft identity platform en je hebt het [maximum aantal redirect URI's](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) bereikt.</span><span class="sxs-lookup"><span data-stu-id="e3e87-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="e3e87-129">Je kan dit oplossen door [Redirect URI's toe te voegen aan service-principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) die overeenkomen met iedere klant.</span><span class="sxs-lookup"><span data-stu-id="e3e87-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
