---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: Er is een klein probleem. Dat veld wordt gebruikt in een configuratie met meerdere formulieren.'''
description: Wanneer u een berekening in een berekend aangepast veld wijzigt op een aangepast formulier en een foutbericht laat zien dat het veld wordt gebruikt in een configuratie met meerdere formulieren, moet u het veld vervangen door een nieuw veld dat de berekening bevat die u wilt gebruiken.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1175'
ht-degree: 0%

---

# Foutbericht: Er is een klein probleem. Dat veld wordt gebruikt in een configuratie met meerdere formulieren

## Probleem

Wanneer u een berekening wijzigt in een berekend aangepast veld op een aangepast formulier, [!DNL Adobe Workfront] zou de volgende waarschuwing kunnen tonen:

Er is een klein probleem

[Het veld] wordt gebruikt in een configuratie met meerdere formulieren. Als u deze formule wilt wijzigen, moet u dit veld verwijderen en vervangen door een nieuw veld dat de gewenste berekening bevat.

## Oorzaak

Ten minste twee aangepaste formulieren met het berekende aangepaste veld dat u wilt wijzigen, worden gekoppeld aan één object in uw [!DNL Workfront] -instantie.

**Voorbeeld:** Aangepaste formulieren A en B zijn beide aan dezelfde taak gekoppeld. Beide formulieren bevatten een berekend aangepast veld met de naam Winst. Er treedt een fout op wanneer u de berekening probeert te bewerken in het veld Winst op aangepast formulier A.

U kunt de berekening voor het aangepaste veld niet wijzigen in een van de formulieren omdat dat in strijd zou zijn met de formule in hetzelfde veld in het andere formulier.
U lost dit conflict op door het object te zoeken waaraan de meerdere formulieren met hetzelfde berekende aangepaste veld zijn gekoppeld. Voer vervolgens een van de volgende handelingen uit:

* Verwijder een van de formulieren uit het object.
* Wijzig de berekening naar wens, maar wel in alle aangepaste formulieren die aan het object zijn gekoppeld.
* Voeg in alle aangepaste formulieren die aan het object zijn gekoppeld een nieuw berekend aangepast veld toe met de berekening die u nodig hebt en markeer het oude berekende aangepaste veld als verouderd.

In dit artikel wordt uitgelegd hoe u het object kunt vinden en het probleem vervolgens op een van deze drie manieren kunt oplossen.

## Object zoeken waaraan aangepaste formulieren zijn gekoppeld {#find-the-object-where-the-custom-forms-are-attached}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Users]** ![](assets/users-icon-in-main-menu.png).

1. Klik op **[!UICONTROL Custom Forms]** > **[!UICONTROL Fields]**.
1. Pas de **[!UICONTROL Field List]** om het berekende veld te zoeken dat u wilt wijzigen en noteer elk aangepast formulier waarop het wordt gebruikt (bijvoorbeeld formulier 1, formulier 2, formulier 3).
1. Klikken **[!UICONTROL Forms]** en past vervolgens de **[!UICONTROL Form List]** weergeven.
1. Klik op de knop **[!UICONTROL Filter]** vervolgkeuzelijst, dan **[!UICONTROL New Filter]**.

1. Klikken **[!UICONTROL Add a Filter Rule]** Typ vervolgens &quot;aangepaste formuliernaam&quot; en selecteer deze waarde wanneer deze in de lijst wordt weergegeven.
1. Selecteren **[!UICONTROL Equal]** voor de filtermodifier, begin de naam van elke vorm te typen u nota van in Stap 1 maakte, dan selecteer het wanneer het toont.

   **Voorbeeld:** Aangepaste formuliernaam is gelijk aan formulier 1, formulier 2, formulier 3.

1. Klikken **[!UICONTROL Save Filter]** geeft u het nieuwe filter een naam en klikt u op **[!UICONTROL Save Filter]**.

1. Noteer in de lijst met formulieren het objecttype van het filter, zoals Taak of uitgave, dat wordt weergegeven in het dialoogvenster **[!UICONTROL Type]** kolom.
1. Voor elk douaneformulier u in Stap 1 vond, creeer een nieuw Douane gebied Checkbox met één enkele standaardwaarde van ja.

   **Voorbeeld:** Veld 1 op formulier 1 = Ja, veld 2 op formulier 2 = Ja, veld 3 op formulier 3 = Ja. Dit betekent ‘Het berekende aangepaste veld bestaat op formulier 1’ of ‘Het berekende aangepaste veld bestaat op formulier 2’, enzovoort.

1. In de **[!UICONTROL Search icon]** ![](assets/search-icon.png) in de rechterbovenhoek van het scherm klikt u op **[!UICONTROL Advanced Search]**.
1. Klik op het object van het aangepaste formulier (bijvoorbeeld Issue) en klik op **[!UICONTROL Filter your results]** en klik vervolgens op **[!UICONTROL Add a filter]**.
1. Typ de naam van een veld Selectievakje in het vak **[!UICONTROL Start typing field name]** en selecteer het wanneer het in de lijst toont, dan selecteren **[!UICONTROL Equal]** en type **[!UICONTROL Yes]** (zonder aanhalingstekens) in het volgende vak.

   **Voorbeeld:** Veld 1 gelijk (hoofdlettergevoelig) Ja.

1. Klikken **[!UICONTROL Add a Filter]** en voeg alle velden Selectievakje toe aan uw geavanceerde zoekopdracht.

   Zoek naar elke mogelijke combinatie.

   **Voorbeeld:** Stel verschillende filters samen met de combinaties die u vindt, zoals hieronder wordt weergegeven. U moet objecten zoeken met meerdere aangepaste formulieren die dezelfde berekende velden bevatten. U zou de volgende scenario&#39;s kunnen vinden:

   * Veld 1= Ja + veld 2 = Ja + veld 3 = Ja (bijvoorbeeld geen objecten)
   * Veld 1= Ja + veld 2 = Ja (bijvoorbeeld geen objecten)
   * Veld 1= Ja + veld 3 = Ja (bijvoorbeeld twee objecten)

   Dit betekent dat het berekende veld aanwezig is op zowel formulier 1 als formulier 3, omdat de bijbehorende selectievakjes (Veld 1 en veld 3) op deze objecten bestaan.

   Veld 2 = Ja + veld 3 = Ja (bijvoorbeeld geen objecten)

1. Doorgaan naar een van de volgende secties in dit artikel:

   * [Een van de aangepaste formulieren uit het object verwijderen en de berekening daar bewerken](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Dezelfde bewerkingen aanbrengen in de berekening in alle bijgevoegde aangepaste formulieren](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Voeg een nieuw berekend veld met de bewerkte berekening toe aan een of alle bijgevoegde aangepaste formulieren](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Een van de aangepaste formulieren uit het object verwijderen en de berekening daar bewerken {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Het object zoeken waaraan de aangepaste formulieren zijn gekoppeld, zoals wordt uitgelegd in [Object zoeken waaraan aangepaste formulieren zijn gekoppeld](#find-the-object-where-the-custom-forms-are-attached) in dit artikel, opent u het object.
1. Verwijder een van de aangepaste formulieren van het object en sla het object op.

   >[!NOTE]
   >
   >Als u de velden wilt toevoegen van het formulier dat u uit het object hebt verwijderd, moet u mogelijk het aangepaste formulier bewerken dat aan het object gekoppeld blijft. Op deze manier kunt u de aangepaste gegevensgegevens van het object behouden.

1. Bewerk in het aangepaste formulier dat u hebt verwijderd de berekening voor het aangepaste veld dat u oorspronkelijk probeerde bij te werken en klik vervolgens op **[!UICONTROL Save]**.

   Deze keer [!DNL Workfront] mogen geen conflict tegenkomen.

1. (Optioneel) Verwijder de velden Selectievakje van de aangepaste formulieren of verwijder deze uit [!DNL Workfront].

## Dezelfde bewerkingen aanbrengen in de berekening in alle bijgevoegde aangepaste formulieren {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Gegevens gaan verloren in de objecten waaraan het aangepaste formulier al is gekoppeld wanneer u deze stappen uitvoert. Als het berekende veld echter verwijst naar statische velden en niet naar berekende velden, kunt u [!UICONTROL Recalculate Custom Expressions] optie voor het object om de verloren gegevens te herstellen

1. Het object zoeken waaraan de aangepaste formulieren zijn gekoppeld, zoals wordt uitgelegd in [Object zoeken waaraan aangepaste formulieren zijn gekoppeld](#find-the-object-where-the-custom-forms-are-attached) in dit artikel.
1. Verwijder het veld uit alle aangepaste formulieren die aan het object zijn gekoppeld en sla de formulieren vervolgens op.

1. Voeg het aangepaste veld met de nieuwe berekening toe aan de aangepaste formulieren.

   >[!IMPORTANT]
   >
   >De berekeningen moeten identiek zijn in alle bijgevoegde aangepaste formulieren.

1. (Optioneel) Verwijder de velden in het selectievakje uit de formulieren of verwijder deze uit de formulieren [!DNL Workfront].

## Voeg een nieuw berekend veld met de bewerkte berekening toe aan een of alle bijgevoegde aangepaste formulieren {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Als u wilt voorkomen dat gegevens verloren gaan in het bestaande berekende aangepaste veld of als u de bewerkte berekening wilt uitvoeren in slechts een van de aangepaste formulieren die aan het object zijn gekoppeld dat u hebt gevonden:

1. Het object zoeken waaraan de aangepaste formulieren zijn gekoppeld, zoals wordt uitgelegd in [Object zoeken waaraan aangepaste formulieren zijn gekoppeld](#find-the-object-where-the-custom-forms-are-attached) in dit artikel.
1. Voeg een nieuw berekend aangepast veld met de berekening die u nodig hebt toe aan een of alle formulieren.
1. De naam van het oude berekende aangepaste veld wijzigen **Achterhaald**.

   Op alle formulieren die aan het object zijn gekoppeld, behoudt dit oudere berekende aangepaste formulier de historische gegevens, maar gebruikers gebruiken het niet meer.

   >[!IMPORTANT]
   >
   >In andere berekende aangepaste velden kan naar het oudere veld worden verwezen. U moet deze berekeningen dus bijwerken nadat u de naam hebt gewijzigd.

1. (Optioneel) Verwijder de velden Selectievakje van de formulieren of verwijder deze uit Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
