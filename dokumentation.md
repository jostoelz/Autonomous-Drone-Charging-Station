# Abstract
In diesem Projekt baue ich eine automatische Ladevorrichtung für Drohnen. Sobald die Drohne vom Piloten auf einer Plattform gelandet wurde, wird ein Mechanismus aktiviert, der die Drohne in die richtige Position bringt und den Ladevorgang startet. Nach Abschluss des Ladevorgangs ist die Drohne wieder abflugbereit.
# Projekt im Detail
Der Pilot landet auf einer Landeplattform. Die Landeplattform verfügt an zwei Seiten über Wände, an denen zwei Ultraschallsensoren angebracht sind. An den anderen beiden Seiten ist jeweils ein Linearantrieb mit einem Schieber angebracht. Sobald die Ultraschallsensoren eine Drohne auf der Landeplattform erfassen, bewegen die Linearantriebe die Drohne so weit in die Ecke, bis sie sich in der richtigen Position befindet. Unterhalb der Landeplattform ist ein wireless charging Sender montiert, während sich unterhalb der Drohne der entsprechende wireless charging Empfänger befindet. Sobald die Ultraschallsesonren erkennen, dass sich die Drohne in der Ecke befindet, fließt Strom von einem Netzteil zum wireless charging Sender. Der Empfänger an der Drohne wandelt die Wechselspannung in Gleichstrom um, der dann in den Akku der Drohne fließt, der über ein Kabel mit dem wireless charging Empfänger verbunden ist. Sobald der Ladevorgang abgeschlossen ist, kann die Drohne wieder abheben.
## Welche Features wurden umgesetzt?
Nebendessen, dass die Drohne in der Lage ist, auf einer Plattform zu landen, die Linearantriebe die Drohne in die richtige Position bewewegen können, sie über wireless charging selbständig aufgeladen und anschliessend wieder abheben kann, ist die Station mit LEDs ausgestattet, die den Landeplatz bei Dunkelheit beleuchten. So kann der Pilot die Drohne auch nachts oder bei schlechten Sichtverhältnissen sicher landen. Fernerhin zeichnet sich die Ladestation damit aus, dass sie dauerhaft geschlossen ist, um sich gegen Niederschlag zu schützen. Aber auch der robuste Aufbau macht die Handhabung mit der Station flexibel, so dass die Station variabel aufstellbar ist.
## Beschreibung der Hardware
## Beschreibung der Software
## Benützung
Ein Netzteil mit 5V kann in die Power-Öffnung gesteckt werden.
## Demonstration
Ich habe ein <a href="https://kantonsschuleromanshorn-my.sharepoint.com/:v:/g/personal/jostoelz_ksr_ch/EYghmAxh7fZNp1EXa3LVJkMBQi_qL3hC4DV3Lf5EdQMKvw?e=Lkv3ng ">Video</a> aufgenommen, welches die Ladestation in Aktion demonstriert. Um nachzuweisen, dass tatsächlich die Drohne geladen wird, biete ich gerne an, dies auch nach Abgabe des Projektes direkt an der Drohne zu zeigen. Es ist leider nicht möglich, dies auf einem Video festzuhalten. Ebenso wird im Video der An- / Ausschalter, das Display, der Poti und die LEDs nicht genauer demonstriert.
# Entwicklung
# Diskussion & Reflexion
## Was hat gut geklappt, was weniger?
Als das Projekt startete, ging es zuerst an die Ideenfindung und die anschliessende Überlegung, wie man diese Idee umsetzen möchte. Dies war aber bei mir eine mühsame Angelegenheit, da es online keine Tutorials gibt, wie man eine selsbtändige DIJ Ladestation für Drohnen baut. Im speziellen war es schwierig herauszufinden, wie man die Drohne in die richtige Position bringt und wie man sie auflädt (per Kabel oder mit wireless charging). Einiger meiner Überlegungen dazu habe ich mir skizziert: 
- Bestellung Materialien

## Was würde ich anders machen?
Nächstes Mal würde ich mich mehr an meinen Zeitplan halten und zuerst die wichtigsten Ziele erreichen, bevor ich mich den Erweiterungen widme. Ich habe mich leider über mehrere Wochen dem optionalen Feature des Zugriffs der externe Wettervorhersagen über eine API gekümmert. Damit wollte ich dem Pilot eine Empfehlung (je nach Wind & Niederschlag) über das Fliegen geben. Jedoch ist dieses Feature immer an einem bestimmen Punkt gescheitert. Ich wollte nicht aufgeben und so schob ich die eigentlich wichtigen Dinge, wie die Herstellung der Box, immer weiter heraus. Schlussendlich bin ich in einen Stress gekommen und konnte deshalb gewünschte Veränderungen aus zeitlichen Gründen nicht mehr umsetzen.
## Erweiterungen
* Eine bedeutende Verbesserung der Ladestation wäre, dass das Aufladen der Drohne nicht mehr (wie bis anhin) nur funktioniert, wenn die Drohne in einer speziellen Ausrichtung landet (mit der Kamera nach vorne und seitlich zur kurzen Seite der Station), sondern variabel landen kann. Dafür würde man aber zwei Linearantriebe mehr benötigen. Dies war aber im Rahmen des Budgets dieses Projektes nicht möglich.
* Eine andere Erweritung wäre, dass die Box mit Wettersensoren ausgestattet ist und dem Piloten je nach Wetterbedingungen Empfehlungen abgibt, ob er fliegen sollte oder nicht.
* Ebenso könnte man die Box durch Solarpanels erweitern, sodass sie autark ist und sich bei gutem Wetter selbst wieder aufladen.
* Man könnte aber auch die Station aus Metall herstellen und die elektronsichen Verbindungen isolieren, sodass sie vor Nässe besser geschützt sind.
* Eine weitere Erweiterung könnte die Installierung eines GPS sein, damit auch sicheres Landen ohne Sichtkontakt möglich ist, die schnellste Route zwischen Drohne und Ladestation angezeigt werden kann oder wenn die Station geklaut wurde, eine Nachverfolgung stattfinden kann.
# Code
