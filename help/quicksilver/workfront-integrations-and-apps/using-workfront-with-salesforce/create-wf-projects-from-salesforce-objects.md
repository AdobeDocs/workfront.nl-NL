---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-salesforce
title: Maken [!DNL Adobe Workfront] projecten van [!DNL Salesforce] objecten
description: Na installatie [!DNL Adobe Workfront] voor Salesforce kunt u triggers definiëren die [!DNL Workfront] projecten waarbij aan bepaalde criteria is voldaan [!DNL Salesforce] Kansen en accounts.
author: Becky
feature: Workfront Integrations and Apps
exl-id: b38c91ae-342b-4002-a947-7a0ab1aaca93
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# Maken [!DNL Adobe Workfront] projecten van [!DNL Salesforce] objecten

Na installatie [!DNL Adobe Workfront] voor Salesforce kunt u triggers definiëren die [!DNL Workfront] projecten waarbij aan bepaalde criteria is voldaan [!DNL Salesforce] [!UICONTROL Opportunities] en [!UICONTROL Accounts].

## Toegangsvereisten

U moet de volgende toegang hebben om de in dit artikel beschreven functionaliteit te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

Een [!DNL Workfront] verzoek van een [!DNL Salesforce] [!UICONTROL Opportunity] of Account zorgt ervoor dat u het volgende in uw omgeving hebt:

* Uw [!DNL Workfront] beheerder heeft geïnstalleerd [!DNL Workfront for Salesforce].\
   Meer informatie over installeren [!DNL Workfront for Salesforce], zie [Installeren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Uw [!DNL Workfront] beheerder heeft de [!DNL Workfront] in uw [!UICONTROL Opportunity] en accountpaginalay-outs.\
   Voor meer informatie over het toevoegen van de [!DNL Workfront] sectie naar een pagina-indeling, zie [Configureer de [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* U hebt een [!DNL Workfront] en u kunt zich hier aanmelden via het dialoogvenster [!DNL Workfront] sectie in uw [!UICONTROL Opportunity] of account.

## De creatie van [!DNL Workfront] Projecten van [!DNL Salesforce]

* [De automatische creatie van projecten begrijpen](#understanding-the-automatic-creation-of-projects-understanding-the-automatic-creation-of-projects)
* [Triggers configureren](#configuring-triggers-configuring-triggers)
* [Projectnamen](#understanding-project-names-understanding-project-names)

### De automatische creatie van projecten begrijpen {#understanding-the-automatic-creation-of-projects}

Als de [!DNL Salesforce] systeembeheerder, kunt u trekkers bepalen die projecten in kunnen automatisch tot stand brengen [!DNL Workfront] wanneer de volgende dingen gebeuren in [!DNL Salesforce]:

* De [!UICONTROL Stage] van een [!UICONTROL Opportunity] wordt bijgewerkt.
* De [!UICONTROL Type] van een account is bijgewerkt.

Triggers kunnen alleen worden geconfigureerd nadat u hebt geïnstalleerd [!DNL Workfront for Salesforce].  \
Voor informatie over installeren [!DNL Workfront for Salesforce], zie [Installeren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Overweeg het volgende wanneer het vormen van trekkers om automatisch tot stand te brengen [!DNL Workfront] projecten wanneer [!DNL Salesforce] items worden gemaakt of bijgewerkt:

* U moet een [!DNL Salesforce] en [!DNL Workfront] systeembeheerder om triggers te configureren.
* Nadat u de triggers hebt geconfigureerd, iedereen die de [!UICONTROL Stage] van een [!UICONTROL Opportunity] of de [!UICONTROL Type] van een account kan het maken van een [!DNL Workfront] project. Dit omvat [!DNL Salesforce] gebruikers die geen [!DNL Workfront] account.
* Er is geen limiet voor het aantal triggers dat u kunt gebruiken.
* U kunt geen meerdere triggers maken op basis van dezelfde voorwaarden. Triggers zijn standaard uniek.
* Zodra het project wordt gecreeerd wordt het automatisch verbonden met de kans of de rekening waar het werd geproduceerd. Zodra gevestigd, kan deze verbinding niet worden gebroken.
* Eén mogelijkheid of account kan worden gekoppeld aan meerdere projecten in [!DNL Workfront] wanneer meerdere malen is voldaan aan een getriggerde voorwaarde gedurende de looptijd van de opportuniteit of de rekening.

   Als u bijvoorbeeld meer dan één code definieert [!UICONTROL Stage] voor een [!UICONTROL Opportunity] om een project te activeren, wordt een project gemaakt voor elke gedefinieerde fase die de kans bereikt, gedurende de levensduur van die kans. Ook als u de [!UICONTROL Stage] van een [!UICONTROL Opportunity] van het ene gedefinieerde werkgebied naar het andere, en het vervolgens weer bij te werken naar het gedefinieerde werkgebied, wordt een tweede project gemaakt voor de tweede keer dat u de [!UICONTROL Stage] naar hetzelfde gedefinieerde werkgebied.

* Eén project in [!DNL Workfront] kan slechts aan één kans of één rekening in worden verbonden [!DNL Salesforce] op elk moment, maar niet op beide tegelijk.

### Triggers configureren {#configuring-triggers}

Zodra u de trekkers vormt, het proces om [!DNL Workfront] projecten zijn ingeschakeld voor beide [!UICONTROL Salesforce Classic] of [!DNL Lightning Experience] frameworks.

Om triggers te configureren in [!UICONTROL Salesforce]:

1. Aanmelden bij [!DNL Salesforce] als de systeembeheerder.
1. (Voorwaardelijk) In [!DNL Salesforce Classic], klikt u op **[!UICONTROL Setup]** en onder de **[!UICONTROL Build]** sectie, uitvouwen **[!UICONTROL Lightning Bolt]**.

   of

   In [!DNL Salesforce] Bliksem-ervaring, klik op de knop **[!UICONTROL Setup]pictogram** vervolgens **[!UICONTROL Setup]** en onder **[!UICONTROL PLATFORM TOOLS]** uitbreiden **[!UICONTROL Apps]**.

1. Klik op **[!UICONTROL Installed Packages]**.

   Let erop dat de **[!DNL Workfront]** pakket is geïnstalleerd.

1. Klikken **[!UICONTROL Configure]** naast **[!DNL Workfront]**.

1. Aanmelden bij [!DNL Workfront] als systeembeheerder.

   De **[!UICONTROL Triggers]** wordt weergegeven.

   ![salesforce_triggers_page_empty.png](assets/salesforce-triggers-page-empty-350x134.png)

1. Klik op **[!UICONTROL New Trigger]**.
1. Van de **[!UICONTROL [!DNL Salesforce] Object]** vervolgkeuzelijst, selecteert u **[!UICONTROL Opportunity]**.

   Dit is een verplicht veld.

1. (Voorwaardelijk) Geef het volgende op:

   1. Van de **[!UICONTROL Stage]** vervolgkeuzelijst, selecteert u een **[!UICONTROL Stage]**.\

      Wanneer een kans de [!UICONTROL Stage] hier opgegeven, wordt een project gemaakt in [!DNL Workfront]. Dit is een verplicht veld.

   1. In de **[!UICONTROL Portfolio or Program]** veld, typ de naam van een Portfolio of Programma waarin u het project wilt plaatsen [!DNL Workfront]en selecteert u deze wanneer deze in de lijst wordt weergegeven.\

      Als u geen Portfolio of Programma specificeert, wordt het nieuwe project gecreeerd en aan toegevoegd [!UICONTROL Projects I Own] lijst met de gebruiker die zich heeft aangemeld bij [!DNL Workfront] wanneer het vormen van de trekkers. Die gebruiker is ook de Eigenaar van het Project voor het nieuwe project.

   1. Typ de naam van een sjabloon die u aan het nieuwe sjabloon wilt koppelen [!DNL Workfront] en selecteert u deze wanneer deze in de lijst wordt weergegeven.\

      Dit is een verplicht veld.


      >[!NOTE]
      >
      >Als u een Eigenaar van het Malplaatje op het malplaatje hebt gespecificeerd dat u voor deze integratie wilt gebruiken, wordt dat de Eigenaar van het Project van het nieuwe project. De nieuwe projecten worden onder de [!UICONTROL Projects I Own] lijst van de gebruiker die de eigenaar van het nieuwe project, volgens het malplaatje is.

   1. (Optioneel) Selecteer de optie **[!UICONTROL Create a new project for each sold product type]field**, als u een nieuw project wilt maken voor elk type product dat onder om het even welke kans wordt verkocht.
   1. (Voorwaardelijk) Selecteer een **[!UICONTROL Product]** in de **[!UICONTROL Product]** vervolgkeuzemenu.

      Dit is een verplicht veld.

   1. (Voorwaardelijk) Typ de naam van een **[!UICONTROL Template]** die u aan het nieuwe wilt associëren [!DNL Workfront] project als het gespecificeerde Product op het gespecificeerde Product is [!UICONTROL Opportunity]. Selecteer het wanneer het in de lijst verschijnt.

      Dit is een verplicht veld.

      Het project dat wordt gemaakt wanneer een nieuw product wordt toegevoegd aan de [!DNL Salesforce] wordt in de Portfolio of het Programma geplaatst die voor de kans worden geselecteerd.

      >[!IMPORTANT]
      >
      >Het project wordt alleen gemaakt wanneer het werkgebied wordt bijgewerkt op het tabblad [!UICONTROL Opportunity]. Er wordt een uniek project gemaakt voor elk product dat wordt opgegeven wanneer het veld Werkgebied wordt bijgewerkt, en niet wanneer de producten worden toegevoegd aan [!UICONTROL Opportunities].

1. (Optioneel) Klik op **[!UICONTROL New Trigger]**.
1. (Optioneel) Van de **[!UICONTROL [!DNL Salesforce] Object]** Selecteer **Account **.

   Dit is een verplicht veld.
1. (Voorwaardelijk) Geef het volgende op:

   1. Selecteer een **[!UICONTROL Type]** van de **[!UICONTROL Type]** vervolgkeuzemenu.

      Wanneer een **Account ** is aangewezen als **[!UICONTROL Type]** hier opgegeven [!DNL Salesforce], **[!UICONTROL Project]** is gemaakt in [!DNL Workfront].

      Dit is een verplicht veld.

   1. (Optioneel) Typ de naam van een **[!UICONTROL Portfolio]** of **[!UICONTROL Program]** waar u het project wilt plaatsen [!DNL Workfront] in de **[!UICONTROL Portfolio or Program]** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

      Als u geen Portfolio of Programma specificeert, wordt het nieuwe project gecreeerd en aan toegevoegd **[!UICONTROL Projects I Own]** lijst met de gebruiker die zich heeft aangemeld bij [!DNL Workfront] van [!DNL Salesforce]. De gebruiker is ook de Eigenaar van het Project voor het nieuwe project.

   1. Typ de naam van een **[!UICONTROL Template]** die u aan het nieuwe wilt associëren [!DNL Workfront] en selecteert u deze wanneer deze in de lijst wordt weergegeven.

      Dit is een verplicht veld.

      >[!NOTE]
      >
      >Als u een Eigenaar van het Malplaatje op het malplaatje hebt gespecificeerd dat u voor deze integratie wilt gebruiken, wordt dat de Eigenaar van het Project van het nieuwe project. De nieuwe projecten worden onder de **[!UICONTROL Projects I Own]** lijst van de gebruiker die de eigenaar van het nieuwe project, volgens het malplaatje is.
   ![salesforce_triggers_page_with_clean_up_template_names.png](assets/salesforce-triggers-page-with-cleaned-up-template-names-350x157.png)

1. Klik op **[!UICONTROL Save]**.

   [!DNL Workfront] er worden nu projecten gegenereerd telkens wanneer aan een van de triggers wordt voldaan .

### Projectnamen {#understanding-project-names}

Afhankelijk van welke trigger de projecten heeft gegenereerd, worden de namen van de projecten in [!DNL Workfront] kan een van de volgende patronen volgen:

* Als het project wordt gecreeerd gebaseerd op een opportuniteit of rekeningstrekker, is de naam van het project: *`<Salesforce object name>`: `<Project template name>` (via [!DNL Salesforce])*.
* Als het project wordt gecreeerd gebaseerd op een opportuniteitstrekker die ook de toevoeging van een nieuw Product omvat, is de naam van het project: *`<Salesforce object name>`: `<Salesforce product name>` (via [!DNL Salesforce])*.

## Weergave [!DNL Workfront] projecten

Als uw [!DNL Workfront] beheerder heeft de [!DNL Workfront] in uw [!UICONTROL Opportunity] of de pagina-indeling van de account, kunt u de projecten zien die automatisch zijn gemaakt in het dialoogvenster [!UICONTROL Projects] tabblad van deze sectie.\
Voor meer informatie over het toevoegen van de [!DNL Workfront] aan de pagina-indeling van een [!UICONTROL Opportunity] of account, zie [Configureer de [!DNL Adobe Workfront] sectie voor [!DNL Salesforce] gebruikers](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

U moet beschikken over een [!DNL Workfront] account en aangemeld bij [!DNL Workfront] om de [!UICONTROL Projects] tab.

Projecten weergeven die zijn gemaakt op basis van een [!UICONTROL Opportunity] of Account:

1. Ga naar een [!UICONTROL Opportunity] of account.
1. Ga naar de **[!DNL Workfront]** sectie.

   >[!NOTE]
   >
   >Afhankelijk van hoe uw [!DNL Workfront] beheerder vormde deze sectie, zou het een verschillende naam kunnen hebben.

1. Selecteer **[!UICONTROL Projects]** tab.

   Alle projecten die door bepaalde triggers worden gemaakt, worden op dit tabblad weergegeven. Willekeurige gebruiker in [!DNL Salesforce] die ook een [!DNL Workfront] account en wie machtigingen hebben om deze projecten te bekijken in [!DNL Workfront] kan ze ook zien in [!DNL Salesforce] voor de [!UICONTROL Opportunity] of de account die ze heeft gegenereerd.

   U kunt de volgende informatie over de projecten bekijken die door de integratie worden gecreeerd:

   * Projectnaam
   * Referentienummer
   * Invoerdatum
   * Naam van de eigenaar
   * Status
   * Voorwaarde
   * Geplande afsluitdatum
   * Percentage voltooid

      Wanneer deze informatie wordt bijgewerkt in [!DNL Workfront], kunt u de velden zien die in deze lijst zijn bijgewerkt.

1. (Optioneel) Klik op de naam van een project om het te openen in Workfront.
1. (Optioneel) Klik op [!UICONTROL **[!UICONTROL Go to Salesforce]**] in de [!UICONTROL Project Details] gebied of de projectheader om tot [!UICONTROL Opportunity] of de rekening waar het project is ontstaan. Uw systeem- of groepsbeheerder moet de [!UICONTROL Integrations] aan uw lay-outmalplaatje om het in de projectheader te vinden.

   >[!NOTE]
   >
   >De [!UICONTROL Go to Salesforce] koppeling is voor iedereen zichtbaar [!DNL Workfront] gebruikers die het project kunnen bekijken. U moet beschikken over een [!DNL Salesforce] om naar de [!DNL Salesforce] Opportunity of Account vanaf waar het project is gegenereerd.
