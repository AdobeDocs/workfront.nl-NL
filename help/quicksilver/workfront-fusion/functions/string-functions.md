---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Tekenreeksfuncties in Adobe Workfront Fusion
description: De volgende tekenreeksfuncties zijn beschikbaar in het Adobe Workfront Fusion-toewijzingspaneel.
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 0%

---

# Tekenreeksfuncties in [!DNL Adobe Workfront Fusion]

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licentie**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p><p>[!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii (text; [remove diacritics])]

Hiermee worden alle niet-ascii-tekens uit een tekstreeks verwijderd.

>[!INFO]
>
>**Voorbeelden:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   Retourneert: [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   Retourneert: [!UICONTROL escrz]


## [!UICONTROL base64 (text)]

Transformeert tekst naar base64.

>[!INFO]
>
>**Voorbeeld:**
>
>`base64( workfront )`
>
>Retourneert: d29ya2Zyb250==

## [!UICONTROL capitalize (text)]

Zet het eerste teken in een tekstreeks om in hoofdletters.

>[!INFO]
>
>**Voorbeeld:**
>
>`capitalize( workfront )`
>
>Retourneert: [!DNL Workfront]

## bevat (tekst; zoektekenreeks)

Controleert of tekst de zoektekenreeks bevat.

>[!INFO]
>
>**Voorbeelden:**
>
>* `contains( Hello World ; Hello )`
   >
   >   Retourneert: [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   Retourneert: [!UICONTROL false]


## [!UICONTROL decodeURL (text)]

Hiermee worden speciale tekens in een URL gedecodeerd naar tekst.

>[!INFO]
>
>**Voorbeeld:**
>`decodeURL( Automate%20your%20workflow )`
>
>Retourneert: [!UICONTROL Automate your workflow]

## [!UICONTROL encodeURL (text)]

Hiermee worden speciale tekens in bepaalde tekst gecodeerd als een geldig URL-adres.

## [!UICONTROL escapeHTML (text)]

Hiermee kunt u alle HTML-tags in tekst laten knippen.

>[!INFO]
>
>**Voorbeeld:**
>
>`escapeHTML( <b>Hello</b> )`
>
> Retourneert: `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

Hiermee kunt u alle markeringen voor markeringen in tekst laten knippen.

>[!INFO]
>
>**Voorbeeld:**
>
>`escapeMarkdown( # Header )`
>
>Retourneert: `&#35; Header`

## [!DNL indexOf (string; value; [start])]

Retourneert de positie van de eerste instantie van een opgegeven waarde in een tekenreeks. Deze methode retourneert &#39;-1&#39; als de waarde waarnaar wordt gezocht er niet is. De beginwaarde geeft aan waar in de tekenreeks de zoekopdracht moet beginnen.

>[!INFO]
>
>**Voorbeelden:**
>
>* `indexOf( Workfront ; o )`
   >
   >   Retourneert: 1
>
>* `indexOf( Workfront ; x )`
   >
   >   Retourneert: -1
>
>* `indexOf( Workfront ; o ; 3 )`
   >
   >   Retourneert: 6


## [!UICONTROL length (text or buffer)]

Retourneert de lengte van de tekstreeks (aantal tekens) of binaire buffer (buffergrootte in bytes).

>[!INFO]
>
>**Voorbeeld:**
>
>`length( hello )`
>
>Retourneert: 5

## [!UICONTROL lower (text)]

Hiermee worden alle alfabetische tekens in een tekstreeks omgezet in kleine letters.

>[!INFO]
>
>**Voorbeeld:**
>
>`lower( Hello )`
>
>Retourneert: hallo

## [!UICONTROL md5 (text)]

Berekent de md5 hash van een tekenreeks.

>[!INFO]
>
>**Voorbeeld:**
>
>`md5( Workfront )`
>
>Retourneert: `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL replace (text;search string; replacement string)]

Vervangt de zoekreeks door de nieuwe tekenreeks.

>[!INFO]
>
>**Voorbeeld:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>Retourneert: [!UICONTROL Hi World]

Reguliere expressies (ingesloten in `/.../`) kan worden gebruikt als zoekreeks met een combinatie van markeringen (zoals `g`, `i`, `m`) toegevoegd:

>[!INFO]
>
>**Voorbeeld:**
>
>![](assets/replace---1-350x31.png)
>
>Al deze getallen X X X X worden vervangen door X

De vervangende tekenreeks kan de volgende speciale vervangingspatronen bevatten:

* `$&` Voegt de overeenkomende subtekenreeks in.
* `$n` Wanneer n een positief geheel getal is dat kleiner is dan 100, wordt de tekenreeks nde parenthesized van submatch ingevoegd. Dit is 1-geïndexeerd.

>[!INFO]
>
>**Voorbeelden:**
>
>![](assets/variable-value-350x63.png)
>
>Retourneert: Telefoonnummer `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>Retourneert: Telefoonnummer: `+420777111222`

>[!CAUTION]
Gebruik geen benoemde vastleggroepen, zoals `/ is (?<number>\d+)/` in het vervangingstekenreeksargument. Dit resulteert in een fout.

Zie voor meer informatie over reguliere expressies [Tekstparser](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (text; [encoding]; [key])]

Berekent de sha1 hash van een tekenreeks. Als het belangrijkste argument wordt gespecificeerd, is sha1 HMAC hash in plaats daarvan teruggekeerd. Ondersteunde coderingen: &quot;hex&quot; (standaardwaarde), &quot;base64&quot; of &quot;latin1.&quot;

>[!INFO]
**Voorbeeld:**
`sha1( workfront )`
Retourneert: b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [encoding]; [key])]

Berekent de sha256 hash van een tekenreeks. Als het zeer belangrijke argument wordt gespecificeerd, sha256 hash HMAC in plaats daarvan is teruggekeerd. Ondersteunde coderingen: &quot;hex&quot; (standaardwaarde), &quot;base64&quot; of &quot;latin1&quot;.>

>[!INFO]
**Voorbeeld:**
`sha256( workfront )`
Retourneert: ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (text; [output encoding]; [key]; [key encoding])]

Berekent de sha512 hash van een tekenreeks. Als het belangrijkste argument wordt gespecificeerd, sha512 hash HMAC is in plaats daarvan teruggekeerd.

Ondersteunde coderingen:

* &quot;[!UICONTROL hex]&quot; (standaard)
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

Ondersteunde toetscoderingen:

* &quot;[!UICONTROL text]&quot; (standaard)
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot; of &quot;[!UICONTROL binary]&quot;

Wanneer u &quot;[!UICONTROL binary]&quot; sleutelcodering, moet een sleutel een buffer zijn, niet een koord.

>[!INFO]
**Voorbeeld:**
`sha512(workfront)`
Retourneert: 789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd19cd b85e1e19db58bb44b234493af35fd431639c0345adf2cf7ec26e9f4a7fb19

## [!UICONTROL split (text; separator)]

Splitst een tekenreeks in een array van tekenreeksen door de tekenreeks in subtekenreeksen te scheiden.

>[!INFO]
**Voorbeeld:**
`split( John, George, Paul ; , )`

## [!UICONTROL startcase (text)]

Hiermee zet u de eerste letter van elk woord om in hoofdletters en alle andere letters in kleine letters.

>[!INFO]
**Voorbeeld:**
`startcase( hello WORLD )`
Retourneert: [!UICONTROL Hello World]

## [!UICONTROL stripHTML (text)]

Hiermee verwijdert u alle HTML-tags uit tekst.

>[!INFO]
**Voorbeeld:**
`stripHTML( <b>Hello</b> )`
Retourneert: Hallo

## [!UICONTROL substring (text; start;end)]

Retourneert een gedeelte van een tekstreeks tussen de positie &quot;start&quot; en &quot;end&quot;.

>[!INFO]
**Voorbeelden:**
* `substring( Hello ; 0 ; 3)`

   Retourneert: Hel
* `substring( Hello ; 1 ; 3 )`

   Retourneert: el


## [!UICONTROL toBinary (value)]

Zet om het even welke waarde in binaire gegevens om.

U kunt het coderen als tweede argument ook specificeren om binaire omzettingen van hexuitdraai of base64 op binaire gegevens toe te passen.

>[!INFO]
**Voorbeelden:**
* `toBinary( Workfront )`

   Retourneert: 57 6f 72 6b 66 72 6f 6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   Retourneert: 57 6f 72 6b 66 72 6f 6e 74


## [!UICONTROL toString (value)]

Zet een waarde om in een tekenreeks.

## [!UICONTROL trim (text)]

Hiermee verwijdert u spatietekens aan het begin of einde van de tekst.

## [!UICONTROL upper (text)]

Zet alle alfabetische tekens in een tekstreeks om in hoofdletters.

>[!INFO]
**Voorbeeld:**
`upper( Hello )`
Retourneert: [!UICONTROL HELLO]
