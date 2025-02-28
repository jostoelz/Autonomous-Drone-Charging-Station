# Abstract
In diesem Projekt baue ich eine automatische Ladevorrichtung für Drohnen. Sobald die Drohne vom Piloten auf einer Plattform gelandet wurde, wird ein Mechanismus aktiviert, der die Drohne in die richtige Position bringt und den Ladevorgang startet. Nach Abschluss des Ladevorgangs ist die Drohne wieder abflugbereit.
# Projekt im Detail
Der Pilot landet auf einer Landeplattform. Die Landeplattform verfügt an zwei Seiten über Wände, an denen zwei Ultraschallsensoren angebracht sind. An den anderen beiden Seiten ist jeweils ein Linearantrieb mit einem Schieber angebracht. Sobald die Ultraschallsensoren eine Drohne auf der Landeplattform erfassen, bewegen die Linearantriebe die Drohne so weit in die Ecke, bis sie sich in der richtigen Position befindet. Unterhalb der Landeplattform ist ein wireless charging Sender montiert, während sich unterhalb der Drohne der entsprechende wireless charging Empfänger befindet. Sobald die Ultraschallsesonren erkennen, dass sich die Drohne in der Ecke befindet, fließt Strom von einem Netzteil zum wireless charging Sender. Der Empfänger an der Drohne wandelt die Wechselspannung in Gleichstrom um, der dann in den Akku der Drohne fließt, der über ein Kabel mit dem wireless charging Empfänger verbunden ist. Sobald der Ladevorgang abgeschlossen ist, kann die Drohne wieder abheben.
## Welche Features wurden umgesetzt?
Nebendessen, dass die Drohne in der Lage ist, auf einer Plattform zu landen, die Linearantriebe die Drohne in die richtige Position bewewegen können, sie über wireless charging selbständig aufgeladen und anschliessend wieder abheben kann, ist die Station mit LEDs ausgestattet, die den Landeplatz bei Dunkelheit beleuchten. So kann der Pilot die Drohne auch nachts oder bei schlechten Sichtverhältnissen sicher landen. Fernerhin zeichnet sich die Ladestation damit aus, dass sie dauerhaft geschlossen ist, um sich gegen Niederschlag zu schützen. Aber auch der robuste Aufbau macht die Handhabung mit der Station flexibel, so dass die Station variabel aufstellbar ist.
## Beschreibung der Hardware
Die verwendeten elektronischen Komponenten werden in der folgenden Tabelle aufgelistet.
<table>
  <thead>
    <tr>
      <th>Komponenten</th>
      <th>Preis pro Stück</th>
      <th>Link</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>wireless charging Sender & Empfänger</td>
      <td>7.71 Fr.</td>
      <td>https://www.mouser.ch/ProductDetail/Seeed-Studio/106990017?qs=SElPoaY2y5KdLskE1shzqQ%3D%3D&mgh=1&utm_id=20002739518&gad_source=1&gclid=CjwKCAiA3ZC6BhBaEiwAeqfvyuNlfda5-xuXoLrLc3qdhUh8dxR87X4ZW45SWwa3tzxUaDRKo-8zQBoC-xEQAvD_BwE</td>
    </tr>
    <tr>
      <td>offenes Ende zu USB C</td>
      <td>5.45 Fr.</td>
      <td>https://www.conrad.ch/de/p/usb-c-3-1-stecker-mit-offenem-kabelende-usb-c-3-1-tc-2509033-tru-components-inhalt-1-st-1587137.html</td>
    </tr>
    <tr>
      <td>Netzteil</td>
      <td>5.33 Fr.</td>
      <td>https://www.reichelt.com/ch/de/shop/produkt/steckernetzteil_10_w_5_v_2_a-370227?PROVID=2808&gad_source=1&gclid=Cj0KCQiAi_G5BhDXARIsAN5SX7rT-tWpARV_9-TJFdsRmyKfdBHIgLwCn7fREIx21GYVdz2y2PMDzvgaAjFpEALw_wcB&q=%2Fch%2Fde%2Fshop%2Fsteckernetzteil-10-w-5-v-2-a-ys12v-0502000e-p370227.html </td>
    <tr>
      <td>Transformator</td>
      <td>3.90 Fr.</td>
      <td>https://www.bastelgarage.ch/dc-dc-1-5a-step-up-boost-converter </td>
    </tr>
    <tr>
      <td>Mosfet</td>
      <td>2.25 Fr.</td>
      <td>https://www.adafruit.com/product/355 </td>
    </tr>
    <tr>
      <td>Linearantrieb</td>
      <td>35.90 Fr.</td>
      <td>https://www.bastelgarage.ch/6v-electric-cylinder-100mm-128n?gad_source=1&gclid=Cj0KCQiAi_G5BhDXARIsAN5SX7pOlEy0XSUf0RxYFtqWwyanmA4Y5NWjRPP5CRwlg6IoworPIEc1klAaAvznEALw_wcB</td>
    </tr>
    <tr>
    <td>Motor driver</td>
    <td>6.60 Fr.</td>
    <td>https://www.conrad.ch/de/p/joy-it-sbc-motodriver2-entwickler-platine-1-st-1573541.html?utm_source=google-shopping-de&utm_medium=search&utm_campaign=shopping-online-de&utm_content=shopping-ad_cpc&WT.srch=1&ef_id=Cj0KCQiAi_G5BhDXARIsAN5SX7o6_0Nbb4KqGNjm55Ye8g1xzGAJNyGisIYAgcIQBwoagaDJP2YjFNAaAjlnEALw_wcB%3AG%3As&utm_source=google&utm_medium=cpc&utm_campaign=ade_3_shopping_GERMAN&utm_id=319998844&gad_source=1&gclid=Cj0KCQiAi_G5BhDXARIsAN5SX7o6_0Nbb4KqGNjm55Ye8g1xzGAJNyGisIYAgcIQBwoagaDJP2YjFNAaAjlnEALw_wcB </td>
    </tr>
    <tr>
    <td>Ultraschallsensor</td>
    <td>3.28 Fr.</td>
    <td>https://www.reichelt.com/ch/de/shop/produkt/entwicklerboards_-_ultraschall_abstandssensor_hc-sr04-161487?PROVID=2788&gad_source=1&gclid=CjwKCAiAl4a6BhBqEiwAqvrquhSdVMxJ-SXono8RQaygsfe0myq6rt9zlikawhww3HqIJLXRNSHbShoCsIEQAvD_BwE&q=%2Fch%2Fde%2Fshop%2Fentwicklerboards-ultraschall-abstandssensor-hc-sr04-debo-sen-ultra-p161487.html </td>
    </tr>
  </tbody>
</table>
Eine wichtige Bemerkung ist, dass ich zwei Ultraschallsensoren und zwei Linearantriebe verbaut habe. Dazu kommen ebenfalls noch günstige Standard-Komponenten wie Poti, Display, Slide Switch und Widerstände.
In der folgenden Darstellung wird die Hardware an der Drohne aufgezeigt. Der wireless charging Empfänger wurde an der Unterseite der Drohne mit Klebeband montiert. An den Empfänger wurde ein Kabel mit offenem Ende zu USB C gelötet, das schlussendlich in die Drohne gesteckt wurde.
![Hardware_Drohne](Bilder/Hardware_Drohne.jpg)

## Beschreibung der Software
## Benützung
Ein Netzteil mit 5V kann in die Power-Öffnung gesteckt werden.
## Demonstration
Ich habe ein <a href="https://kantonsschuleromanshorn-my.sharepoint.com/:v:/g/personal/jostoelz_ksr_ch/EYghmAxh7fZNp1EXa3LVJkMBQi_qL3hC4DV3Lf5EdQMKvw?e=Lkv3ng ">Video</a> aufgenommen, welches die Ladestation in Aktion demonstriert. Um nachzuweisen, dass tatsächlich die Drohne geladen wird, biete ich gerne an, dies auch nach Abgabe des Projektes direkt an der Drohne zu zeigen. Es ist leider nicht möglich, dies auf einem Video festzuhalten. Ebenso wird im Video der An- / Ausschalter, das Display, der Poti und die LEDs nicht genauer demonstriert.
# Entwicklung
# Diskussion & Reflexion
## Was hat gut geklappt, was weniger?
Als das Projekt startete, ging es zuerst an die Ideenfindung und die anschliessende Überlegung, wie man diese Idee umsetzen möchte. Dies war aber bei mir eine mühsame Angelegenheit, da es online keine Tutorials gibt, wie man eine selsbtändige DIJ Ladestation für Drohnen baut. Im speziellen war es schwierig herauszufinden, wie man die Drohne in die richtige Position bringt und wie man sie auflädt (per Kabel oder mit wireless charging). Einiger meiner Überlegungen dazu habe ich mir skizziert: 
![Skizzen](Bilder/Skizzen.jpg)
Eine andere Schwierigkeit war es, die passenden Teilchen herauszusuchen, denn auch in Bezug auf Stromstärke und Spannung musste beispielsweise Rücksicht auf die Drohne genommen werden. Die Recherche dafür hat lange in Anspruch genommen. Dazu kam noch die wochenlange verspätete Ankunft der Materialien, was dazu geführt hat, dass die Arbeit mit Teilchen erst ziemlich spät begonnen konnte.
Im Gegenzug dazu war dann die Zusammensetzung der verschiedenen elektronischen Komponenten unkompliziert. Widerrum der Bau der Station hat viele Ausmessungen benötigt und Zeit beansprucht. Es musste sich genau überlegt werden, wie und vor allem auch in welcher Reihenfolge man was herstellt und befestigt. Es musste vor allem genau gearbeitet werden, sodass die wireless charging Komponenten exakt übereinander ausgerichtet sind.
![wireless charging Sender & Empfänger](Bilder/Wireless_charging_Sender_Empfänger.png)
## Was würde ich anders machen?
Nächstes Mal würde ich mich mehr an meinen Zeitplan halten und zuerst die wichtigsten Ziele erreichen, bevor ich mich den Erweiterungen widme. Ich habe mich leider über mehrere Wochen dem optionalen Feature des Zugriffs der externe Wettervorhersagen über eine API gekümmert. Damit wollte ich dem Pilot eine Empfehlung (je nach Wind & Niederschlag) über das Fliegen geben. Jedoch ist dieses Feature immer an einem bestimmen Punkt gescheitert. Ich wollte nicht aufgeben und so schob ich die eigentlich wichtigen Dinge, wie die Herstellung der Box, immer weiter heraus. Schlussendlich bin ich in einen Stress gekommen und konnte deshalb gewünschte Änderungen aus zeitlichen Gründen nicht mehr umsetzen.
## Erweiterungen
* Eine bedeutende Verbesserung der Ladestation wäre, dass das Aufladen der Drohne nicht mehr (wie bis anhin) nur funktioniert, wenn die Drohne in einer speziellen Ausrichtung landet (mit der Kamera nach vorne und seitlich zur kurzen Seite der Station), sondern variabel landen kann. Dafür würde man aber zwei Linearantriebe mehr benötigen. Dies war aber im Rahmen des Budgets dieses Projektes nicht möglich.
* Eine andere Erweritung wäre, dass die Box mit Wettersensoren ausgestattet ist und dem Piloten je nach Wetterbedingungen Empfehlungen abgibt, ob er fliegen sollte oder nicht.
* Ebenso könnte man die Box durch Solarpanels erweitern, sodass sie autark ist und sich bei gutem Wetter selbst wieder aufladen.
* Man könnte aber auch die Station aus Metall herstellen und die elektronsichen Verbindungen isolieren, sodass sie vor Nässe besser geschützt sind.
* Eine weitere Erweiterung könnte die Installierung eines GPS sein, damit auch sicheres Landen ohne Sichtkontakt möglich ist, die schnellste Route zwischen Drohne und Ladestation angezeigt werden kann oder wenn die Station geklaut wurde, eine Nachverfolgung stattfinden kann.
# Code
