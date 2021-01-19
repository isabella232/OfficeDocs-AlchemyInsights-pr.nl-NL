---
title: Problemen met gebruikers oplossen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900877"
---
# <a name="announcements"></a>Aankondigingen

Volg de richtlijnen van Google voor de compatibiliteit testen om te testen of uw apps van invloed zijn op uw apps. De richtlijnen van Google is beschikbaar in https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Zorg ervoor dat u de systeemweergave of de systeem browser gebruikt wanneer u zich aanmeldt bij uw gebruikers met Google-accounts van de consument. Zie [problemen met het aanmelden bij toepassing (en) met alleen de Chrome-browser](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)voor meer informatie.


**Ik kan geen nieuwe gebruiker maken in mijn Azure AD-Directory**

Voer de volgende stappen uit om het probleem met het maken van een nieuwe gebruiker in azure AD op te lossen:

1. Zorg ervoor dat u gemachtigd bent om een nieuwe standaardgebruiker te maken. Alleen de rol globale beheerder of gebruikersbeheerder in azure Active Directory (AD) kan een nieuwe standaardgebruiker maken. Als u niet bij een van deze rollen zit, vraagt u een beheerder u aan een van deze rollen toe te voegen of om een nieuwe gebruikersaccount voor u te maken.
2. Zorg ervoor dat de gebruikersnaam zich in een domein bevindt dat is geverifieerd in uw Azure AD. Als u in azure AD geen geverifieerde aangepaste domeinnamen hebt, kunt u uw eerste Azure AD-domein gebruiken, dat eindigt met *. onmicrosoft.com.
3. Zorg ervoor dat de gebruikersnaam zich in een domein bevindt dat niet via uw on-premises AD-Federatie is verbonden met Azure AD. Gebruikers kunnen niet worden toegevoegd aan de Cloud met domeinnamen die federatieve zijn van on-premises.
4. Zorg ervoor dat er geen andere gebruiker of contactpersoon de gebruikersnaam heeft die u wilt toewijzen aan de nieuwe gebruiker. Gebruikersnamen moeten uniek zijn in azure AD.
5. Zie [rollen en beheerders van Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) voor uw Azure AD.
6. Zie de [domeinnamen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) voor uw Azure AD.
7. Bekijk [controlelogboeken](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) voor meer informatie over een onlangs gemaakte of verwijderde gebruiker, alsof de actie en wanneer ze zijn uitgevoerd.
8. Voor meer informatie over het toevoegen van nieuwe gebruikers raadpleegt u [de Azure-Portal gebruiken voor het maken van een nieuwe gebruiker in azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Zie voor meer informatie over machtigingen voor beheerdersrollen in azure AD de [beheerdersrollen in azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Zie [Azure AD PowerShell om een nieuwe gebruiker te maken](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)voor meer informatie over het maken van een gebruiker via Azure AD Powershell.

**Probleem met selfservice registratie**

Voer de volgende stappen uit om problemen op te lossen met betrekking tot selfservice registratie:

1. Als u zelf wilt registreren met uw toepassingen, schakelt u eerst selfservice registratie voor uw Tenant in. 
2. Als u een toepassing wilt inschakelen voor ondersteuning van selfservice registratie, voegt u deze toe aan uw gebruikers stroom. De volgende keer dat u naar de aanmeldingspagina voor de toepassing gaat, ziet u een optie **_geen account? Maak er een._* _. Hiermee start u het zelfregistratie proces.
3. Zie [selfservice registratie voor Azure AD voor](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)informatie over het gebruik van selfservice registratie voor het invullen van een organisatie in azure AD.
4. Wanneer u de gebruikers stroom met een of meer toepassingen hebt gekoppeld, kunnen gebruikers die naar die app gaan, zich registreren en een gastaccount maken met behulp van de opties die in de gebruikers stroom zijn geconfigureerd. Als u meer wilt weten over het registreren van een gastaccount en het verkrijgen van een gastaccount, dan kunnen de gebruikers [selfservice registratie voor gastgebruikers](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)zien.

_ *Probleem met uitnodigen van een externe gebruiker**

Voer de volgende stap uit om problemen op te lossen met betrekking tot het uitnodigen van een externe gebruiker:

Zorg ervoor dat u de uitnodiging van een gebruiker verzendt naar het e-mailadres waarmee de gebruiker zich aanmeldt. Als u de uitnodiging verzendt naar het e-mailadres van een gebruiker, kan de gebruiker de uitnodiging niet inwisselen. Zie voor meer informatie [Azure AD B2B-documentatie](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Ik kan geen licenties toewijzen aan een gebruiker**

Voer de volgende stappen uit als u problemen wilt oplossen met het toewijzen van licenties aan een gebruiker:

1. Voor het beheren van gebruikerslicenties zorgt u ervoor dat u een account gebruikt met een van de vereiste beheerdersrollen: globale beheerder, licentiebeheerder of gebruikersbeheerder. U kunt de rol van de gebruiker controleren op het tabblad **Mapreplicatie** van de gebruikers bladerende.
2. Als u de Azure-Portal en een licentietoewijzing niet ziet, klikt u in de rechterbovenhoek op de melding. Hiermee opent u een blad met details over wat er fout is gegaan. In de meeste gevallen is het voldoende om het probleem te begrijpen en op te lossen.
3. Voordat een licentie aan een gebruiker kan worden toegewezen, moet u ervoor zorgen dat de eigenschap **gebruikslocatie** voor de gebruiker is ingesteld. Controleer of de gebruiker heeft die eigenschap ingesteld door het tabblad **profiel** van de Blade van de gebruiker weer te geven.
4. Zorg ervoor dat er voldoende licenties beschikbaar zijn voor het product dat u wilt toewijzen. U kunt het aantal beschikbare licenties bekijken in de Azure-Portal, via [licenties voor Azure Active Directory->-> alle producten](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. De gebruiker heeft mogelijk al een andere licentie, waarvan de services in de nieuwe licentie die u wilt toewijzen, conflicteert. Als de gebruiker bijvoorbeeld de service Exchange Online (abonnement 1) heeft ingeschakeld, kunt u geen licentie toewijzen met Exchange Online (abonnement 2). Schakel een van de services uit om de nieuwe licentie te kunnen toewijzen. Als u de cmdlets van Azure portal of PowerShell gebruikt, ziet u op de pagina met **probleem Details** de specifieke services die het conflict veroorzaken.
6. Als u probeert een licentie te verwijderen en de fout is opgetreden, heeft de gebruiker mogelijk andere licenties met services die afhankelijk zijn van de services die u wilt verwijderen. Als u de cmdlets van Azure portal of PowerShell gebruikt, worden in het foutbericht de specifieke services weergegeven met afhankelijkheden.
7. Als u wilt weten waarom een licentie is toegevoegd/verwijderd van een gebruiker (bijvoorbeeld de persoon in uw organisatie die wijzigingen heeft aangebracht), controleert u de controlelogboeken. Stel het filter in op **licentie activiteiten** om alle wijzigingen weer te geven, waaronder de ' actor ' waarmee ze worden uitgevoerd.
8. Als u Exchange Online gebruikt, zijn sommige gebruikers in uw Tenant mogelijk niet correct geconfigureerd met dezelfde proxy waarde. In dergelijke gevallen ziet u mogelijk algemene foutberichten wanneer een licentie bewerking mislukt. In [dit artikel](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) vindt u meer informatie over dit probleem, waaronder informatie over [verbinding maken met Exchange Online via externe PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Als u wilt zien welke gebruikers in uw Tenant hetzelfde proxyadres hebben, voert u deze cmdlet van Exchange Online uit:

Uitgevoerd

Get-Recipient | waarbij {$ _. EmailAddress-overeenkomst-overeenkomst <user principal name> } | fL name, RecipientType, EmailAddress





