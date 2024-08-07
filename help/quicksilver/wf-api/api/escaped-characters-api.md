---
content-type: api
navigation-topic: api-navigation-topic
title: Geslaagde tekens in API-reacties
description: Geslaagde tekens in API-reacties
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 4%

---

# Geslaagde tekens in API-reacties

De syntaxis van sommige API-reacties kan het escape-teken ( `\` backslash) bevatten. Een escape-teken geeft aan dat het teken of de tekenreeks van tekens die onmiddellijk na het escape-teken volgen, een speciale waarde heeft. `\t` geeft het leesapparaat bijvoorbeeld door dat `t` moet worden geïnterpreteerd als `tab` en niet als de letter &#39;t&#39;. Een tekenreeks van een of meer tekens na de backslash wordt een escapereeks genoemd.

Voor hexadecimale escapereeksen moeten geldige hexadecimale cijfers worden gebruikt. De volgende tabel bevat een lijst met escapereeksen die zijn gecodeerd in Adobe Workfront API-reacties:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Escape Opeenvolging </strong> </th> 
   <th><strong> het Karakter van Unicode </strong> </th> 
   <th><strong> Vertegenwoordigt </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000 <em> x </em></p> <p>Waar, <em> x </em> is de hexadecimale code voor aantallen 0 door 7</p> </td> 
   <td>0-7</td> 
   <td>Unicode-tekens vertegenwoordigd door codepunten 0 tot en met 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Backspace</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Tab</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Nieuwe regel</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Verticaal tabblad</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Formulierfeed</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Enter</td> 
  </tr> 
  <tr> 
   <td> <p>\u00 <em> xx </em></p> <p><em> waar, xx de hexadecimale code voor is  getallen 14 tot en met 31 </em> </p> </td> 
   <td>14 - 31</td> 
   <td>Unicode-tekens vertegenwoordigd door codepunten 14 tot en met 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Forward slash)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (Minder dan)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (backslash)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em> xxxx </em></p> <p>Waar, <em> xxxx </em> is de hexadecimale code voor om het even welk aantal meer dan 127</p> </td> 
   <td>128+</td> 
   <td>Unicode-tekens voor elk codepunt groter dan 127</td> 
  </tr> 
 </tbody> 
</table>
