# Abstract
In diesem Projekt baue ich eine automatische Ladevorrichtung für Drohnen. Sobald die Drohne vom Piloten auf einer Plattform gelandet wurde, wird ein Mechanismus aktiviert, der die Drohne in die richtige Position bringt und den Ladevorgang startet. Nach Abschluss des Ladevorgangs ist die Drohne wieder abflugbereit.
# Projekt im Detail
Der Pilot landet auf einer Landeplattform. Die Landeplattform verfügt an zwei Seiten über Wände, an denen zwei Ultraschallsensoren angebracht sind. An den anderen beiden Seiten ist jeweils ein Linearantrieb mit einem Schieber angebracht. Sobald die Ultraschallsensoren eine Drohne auf der Landeplattform erfassen, bewegen die Linearantriebe die Drohne so weit in die Ecke, bis sie sich in der richtigen Position befindet. Unterhalb der Landeplattform ist ein wireless charging Sender montiert, während sich unterhalb der Drohne der entsprechende wireless charging Empfänger befindet. Sobald die Ultraschallsesonren erkennen, dass sich die Drohne in der Ecke befindet, fließt Strom von einem Netzteil zum wireless charging Sender. Der Empfänger an der Drohne wandelt die Wechselspannung in Gleichstrom um, der dann in den Akku der Drohne fließt, der über ein Kabel mit dem wireless charging Empfänger verbunden ist. Sobald der Ladevorgang abgeschlossen ist, kann die Drohne wieder abheben.
## Welche Features wurden umgesetzt?
## Beschreibung der Hardware
## Beschreibung der Software
## Benützung
Ein Netzteil mit 5V kann in die Power-Öffnung gesteckt werden.
## Demonstration
Ich habe ein <a href="https://kantonsschuleromanshorn-my.sharepoint.com/:v:/g/personal/jostoelz_ksr_ch/EYghmAxh7fZNp1EXa3LVJkMBQi_qL3hC4DV3Lf5EdQMKvw?e=Lkv3ng ">Video</a> aufgenommen, welches die ganze Station in Aktion demonstriert. Um nachzuweisen, dass tatsächlich die Drohne geladen wird, biete ich gerne an, dies auch nach Abgabe des Projektes physisch zu zeigen.
# Entwicklung
# Diskussion & Reflexion
## Was hat gut geklappt, was weniger?
## Was würde ich anders machen?
## Erweiterungen
Eine bedeutende Verbesserung der Ladestation wäre, dass das Aufladen der Drohne nicht mehr wie bis anhin nur funktioniert, wenn die Drohne in einer speziellen Ausrichtung landet, sondern 
# Code
