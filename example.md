---
backaddress: Absender Name, Absender Straße 42, 1337 Absenderstadt
fromname: Absender Name
fromaddress: |
  Absender Straße 42  
  1337 Absenderstadt
place: Absenderstadt
#fromemail: mail@absender.de	# It is generally not advised to set these, as it clutters the letterhead.
#fromurl: absender.de			# It is generally not advised to set these, as it clutters the letterhead.
to: |
  Musterfirma GmbH  
  Max Mustermann  
  Musterstraße 2  
  12345 Musterstadt
date: \today{}
yourref: "yourref123"
yourmail: "01.01.2001"
subject: "Beispielhafter privater Brief zur Preview des DIN 5008-Template"
signature: Flowinho
opening: "Guten Tag liebe Entwickler:innen,"
closing: "Ich hoffe dieses Template ist euch eine gute Grundlage,"
lang: de-DE
firstfoot: "username@emailprovider.com | abcd efgh ijkl mnop qrstu vwxy | absender.de"
---

Ich habe dieses Template geschrieben um mittels [pandoc]() auf einfache Art und Weise[^1] Briefe schreiben zu können.
Dieses Template basiert auf der \LaTeX{} Klasse `scrletter` und erweitert das DIN5008-Template von Benedict Budel[^2].

Das Ziel war es, eine DIN5008 konforme Briefvorlage zu erzeugen, die visuell ein bisschen "aufgefrischt" wurde, um den daraus resultierenden
Brief etwas ansprechender gestalten zu können. Da DIN5008 sehr streng vorgibt, welche Elemente verändert werden dürfen, habe ich mich auf die Veränderung
einzelner Schriftarten und -farben beschränkt.

Ich habe das Template um folgende Dinge erweitert bzw. geändert:

- Hinzufügen des Tex-Package `xcolor` ermöglicht die Einfärbung mehrerer Elemente des Briefes, in diesem Fall: `fromname`, `fromadress`, `subject`, `place`, `date`, `backadress` und `firstfoot`. Weitere Änderungen können selbstverständlich vorgenommen werden.
- Die optische Erscheinung von `longtable` weicht nun vom bisherigen Standard ab und erlaubt das Einfärben der Tabellenzeilen.
- Einführung von _sans-serif_ Schriftarten um relevante Elemente entsprechend hervorzuheben.

Dinge die ich explizit **nicht** hinzugefügt bzw. geändert habe:

- Syntax-Highlight, das hat in einem Brief nun wirklich keinen Platz.

Hier erscheint nun eine beispielhafte Tabelle.

|Tabellüberschrift 1|Tabellenüberschrift 2|Tabellenüberschrift 3
|:--|:--|:--|
|Zeile 1 A|Zeile 1 B|Zeile 1 C|
|Zeile 2 A|Zeile 2 B|Zeile 2 C|
|Zeile 3 A| Zeile 3 B|Zeile 3 C|
||
|Leerzeile|||
|||Andere Seite|

Und hier geht es mit Text weiter.

[^1]: Durch die Nutzung von Markdown.
[^2]: https://github.com/benedictdudel/pandoc-letter-din5008
