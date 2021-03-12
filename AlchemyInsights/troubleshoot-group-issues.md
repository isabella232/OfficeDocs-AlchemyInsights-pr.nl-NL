---
title: Problemen met groepen oplossen
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713649"
---
# <a name="troubleshoot-group-issues"></a>Problemen met groepen oplossen

**Ik moet een groep toewijzen aan een Azure AD-rol**

Als u een Azure Active Directory-groep (AD)-groep wilt toewijzen aan een Azure AD-rol, voert u de volgende stappen uit:

1. Een nieuwe groep maken: een nieuwe groep maken:

    a. Meld u aan bij het Azure AD-beheercentrum met bevoegdheden voor rolbeheerders of globale beheerdersmachtigingen. 
    b. Selecteer Azure Active Directory > groepen > alle groepen > nieuwe groep. 
    c. Maak de groep.

2. Wijs de rol aan de groep toe tijdens het maken van de groep of nadat de groep is gemaakt.

    a. Als u een rol wilt toewijzen aan de groep op het moment dat de groep wordt gemaakt, schakelt u de wisselknop Azure AD-rollen in om deze aan de groep toe te wijzen en de groep te maken.
    b. Als u een rol aan de groep wilt toewijzen nadat deze is gemaakt, gaat u naar het tabblad Toegewezen rollen voor de nieuwe groep en wijst u de rol aan de groep toe.

**Ik moet het lidmaatschap beheren van een groep die is toegewezen aan de Azure AD-rol**

1. Als u wilt voorkomen dat machtigingen worden ingetrokken, kunnen standaard alleen bevoegde rolbeheerders en globale beheerders het lidmaatschap wijzigen van een groep die aan een rol is toegewezen. Ze kunnen er echter voor kiezen om een eigenaar voor een dergelijke groep toe te wijzen en deze taak te delegeren. Zie cloudgroepen gebruiken om [roltoewijzingen in Azure Active Directory te beheren voor meer informatie.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Zie Problemen oplossen met rollen die zijn toegewezen aan [cloudgroepen](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)voor algemene vragen en tips voor het oplossen van problemen voor het toewijzen van rollen aan groepen in Azure AD.

**Dynamische groepen**

1. Als u de ingebouwde gebruikerskenmerken niet kunt vinden, controleert u of het kenmerk in de lijst met ondersteunde eigenschappen staat.
2. Als u op zoek bent naar ingebouwde apparaatkenmerken, controleert u of het kenmerk zich in de lijst met apparaatkenmerken 
3. Naast de ingebouwde kenmerken van gebruikers en apparaten kunt u ook [Uitbreidingskenmerken gebruiken.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Na het synchroniseren van extensiekenmerken van on-premises Windows Server AD of vanuit een verbonden SaaS-toepassing, moeten de kenmerken zichtbaar zijn in de vervolgkeuzelijst van de opbouwtoepassing voor regels. U vindt de naam van het aangepaste kenmerk in de adreslijst door een query uit te voeren op het kenmerk van een gebruiker met Behulp van PowerShell en te zoeken naar de naam van het kenmerk. Deze kunnen ook worden gebruikt bij het maken van regels in de syntaxis van de regel.
4. Controleer of uw tenant de juiste licentie heeft. Dynamische groepen vereisen dat de tenant een Azure AD P1 Premium-licentie heeft. De lijst met Azure AD-licentieplannen is hier [toegankelijk.](https://azure.microsoft.com/pricing/details/active-directory/) Enterprise Mobility + Security-licentieplannen zijn hier [toegankelijk.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Controleer of de gebruiker die de dynamische groep maakt, een globale beheerder, een intune-beheerder, een groepsbeheerder of een gebruikersbeheerder is.
6. Geef de groep de tijd om ze te vullen. Afhankelijk van de grootte van uw tenant kan het de eerste keer of na een regelwijziging tot 24 uur duren voordat de groep is ingevuld.
7. Zie Kenmerkregels maken voor dynamisch groepslidmaatschap voor meer [informatie.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Ik moet een groep verwijderen**

1. Groepen kunnen worden verwijderd uit de directory met behulp van Remove-AzureADGroup-cmdlet in de Azure AD Powershell-module.
2. Voordat u een gesynchroniseerde groep verwijdert in Azure AD, moet u ervoor zorgen dat u alle toegewezen licenties hebt verwijderd om fouten te voorkomen.
3. Zie Een groep verwijderen met een toegewezen licentie voor meer informatie over het verwijderen van [groepen.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Ik wil een verwijderde groep herstellen**

1. Als een Office 365-groep wordt verwijderd, kan deze maximaal 30 dagen vóór een permanente verwijdering worden teruggezet. Nadat de groep definitief is verwijderd, kan deze niet meer worden hersteld. Hier kunt u meer informatie vinden over het herstellen [van groepen.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Deze functionaliteit wordt niet ondersteund voor beveiligingsgroepen en distributiegroepen.
3. Controleer of u bevoegd bent om een Office 365-groep te herstellen. Globale beheerders, groepsbeheerders, beheerders van gebruikersaccounts, intune-servicebeheerders, partnerlaag1- of laag2-ondersteuning en de eigenaar van de groep kunnen een groep herstellen.
4. Wanneer een dynamische groep wordt verwijderd en hersteld, wordt deze gezien als een nieuwe groep en opnieuw ingevuld volgens de regel. Dit proces kan tot 24 uur duren.
5. Zie Een verwijderde [Office 365-groep herstellen in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)voor meer informatie over het herstellen van een verwijderde groep.

**Configuratie van groep verloopbeleid**

1. Deze functionaliteit wordt alleen ondersteund voor Office 365-groepen en niet voor beveiligings- en distributiegroepen.
2. Voor het configureren en gebruiken van het verloopbeleid voor Office 365-groepen is een Azure AD Premium-licentie vereist.
3. Op dit moment kan slechts één verloopbeleid worden geconfigureerd voor Office 365-groepen op een tenant.
4. Alleen globale beheerders, groepsbeheerders, gebruikersbeheerders en de eigenaar van de groep kunnen een groep verlengen.
5. Als een Office 365-groep is verlopen, wordt deze verwijderd en kan deze maximaal 30 dagen voordat permanent wordt verwijderd, worden hersteld. Nadat de groep definitief is verwijderd, kan deze niet meer worden hersteld. Meer informatie over het herstellen van groepen kunt u [hier vinden.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Automatische verlenging op basis van activiteit**

Gebruikersactiviteiten vanuit SharePoint, Outlook en Teams kunnen automatische verlenging van groepen activeren. Activiteiten worden na 35 dagen gecontroleerd voordat een groep verloopt. Als er activiteit is tijdens de huidige levenscyclus van de groep, wordt de groep automatisch verlengd en wordt er geen e-mailmelding verzonden naar groepseigenaren.

**Tijdsinstellingen voor verlopen groepen**

1. E-mailmeldingen worden 30 dagen, 15 dagen en 1 dag voor de afloop van de groep verzonden naar de eigenaren van de Office 365-groep.
2. Wanneer u verlooptijd de eerste keer in stelt, worden groepen die ouder zijn dan het verloopinterval ingesteld op 35 dagen tot de verlooptijd.
3. De verloopdatum van groepen wordt berekend op basis van de verlengingsdatum van de groep, niet op basis van de datum waarop het beleid is bijgewerkt. Als het verloopbeleid wordt bijgewerkt, verandert de vervaldatum niet.
4. Zie voor meer informatie [e-mails over het verloopbeleid](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) en verlenging van groepen en het herstellen van [een verwijderde Office 365-groep in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Machtiging voor het maken van een groep**

Controleer of u gemachtigd bent om een nieuwe groep te maken. Globale beheerders kunnen het maken van groepen uitschakelen in de Azure Portal of het Access-paneel. Mogelijk moet een beheerder de nieuwe groep voor u maken of u de juiste machtigingen geven.

1. [Een nieuwe groep maken en leden toevoegen in Azure Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Groepen maken in Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Het maken van groepen uitschakelen in Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Beheren wie groepen kan maken in Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Welkomstmelding voor Office 365 uitschakelen via PowerShell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Beheerdersrollen in Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Machtigingen voor het maken van groepen beheren**

1. Globale beheerders kunnen machtigingen voor het maken van groepen beheren voor beveiliging of Office 365-groepen die zijn gemaakt in de Azure Portal of het Access-venster. Gebruikers kunnen beveiligingsgroepen maken **in Azure-portals** of gebruikers kunnen **Office 365-groepen maken in** de instellingen van Azure-portals in Alle groepen > Algemeen **(Instellingen).**
2. U kunt ook het maken van groepen beperken tot het selecteren van een groep gebruikers als u een Azure AD P1 Premium-licentie hebt.

**Welkomstbericht voor nieuwe leden van een Office 365-groep uitschakelen**

De welkomstmelding die wordt verzonden naar gebruikers die zijn toegevoegd aan Office 365-groepen, kan worden uitgeschakeld door Onwaar `UnifiedGroupWelcomeMessageEnabled` in PowerShell in te stellen.  Meer informatie over deze instelling kunt u [hier vinden.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













