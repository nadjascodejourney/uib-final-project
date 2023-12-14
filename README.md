## **ToDo Liste und Herangehensweise**

- Vorbereitung und Layout-Design in Figma => [click-here-to-see-my-figma-layout](https://www.figma.com/file/GoQ6UQWA03ZMIMtr9AgxCT/uib_final_project-portfolio?type=design&node-id=0-1&mode=design&t=QItJQimTzGYWFR4J-0)

- Ordnerstruktur anlegen: images, etc. in entsprechende Unterordner sortieren
- indexdatei erstellen, .scss dateien erstellen (lokal im Projekt, nicht global, nicht über Extension)
- grober Aufbau (vorerst One-Pager, Unterseiten ggf. später) => zunächst noch nicht um Details wie Animationen oder perfekte Bordereigenschaften, usw. kümmern
- dann Schriften, Farben und wiederkehrende Elemente wie z. B. Buttons, etc. in SCSS gestalten
- Responsives Design und Barrierefreiheit nicht vergessen
- Animations etc. erst nachdem alles andere fertig ist (nicht verzetteln), responsives Verhalten berücksichtigen
- Website testen, auch von anderen Personen
- wenn noch Zeit ist, Lighthousereport und ggf. Optimierungen vornehmen

## Besonderheiten/Herausforderungen

- **Projektplan** mit Figjam von Figma

- Skizze mit Stift und Papier, **Layout mit Figma** erstellt

- **Ordnerstruktur** vor Beginn mit Code angelegt (gab später Probleme bzgl. Veröffentlichung über github pages, da hier nur bestimmte Ordnerstruktur funktioniert, was ich vorher nicht wusste)

- Zunächst Schwierigkeiten, mich in mein Design aus Code-Perspektive hineinzudenken (wo genau anfangen, wie hängt alles zusammen (parent, children, etc.))

- Tägliches Meeting mit Drita um sich gegenseitig auf dem Laufenden zu halten (hat mir geholfen, mich an meinen Plan zu halten und mich nicht zu sehr zu verzetteln)

- Mit **SASS** gearbeitet; dabei sind mir Unregelmäßigkeiten bei der Nestingstruktur aufgefallen:
  Insbesondere in Verbindung mit den media queries hat Nesting manchmal nicht funktioniert und ich musste das jeweilige Child-Element doch außerhalb des Nests schreiben, damit der Style angenommen wird => liegt das an den media queries oder hätte ich es anders aufziehen müssen?
  Die Möglichkeit mit Mixins und Variablen zu arbeiten, fand ich aber sehr nützlich. Irgendwann habe ich zwar dann doch wieder alle Styles normal geschrieben, aber im Nachhinein würde ich bspw. auch für das Buttonstyling ein Mixin schreiben. Ich vermute, dass es dann auch weniger Probleme bei den mediaqueries gäbe.

- **Responsive**: Gerade bei den Details sehr kleinteilige Arbeit; scheint mir noch viel Arbeit zu sein, bis meine Seite sich auf möglichst vielen Geräten gut darstellen lässt (habe es neben meinen Geräten auch mit mobile und desktop von Freunden getestet)

- **Grid**: Mit Grid bin ich gut zurecht gekommen, das fällt mir schon relativ leicht und macht Spaß

- **Keyframe Animationen**: Hatte auf der landing page zunächst eine "getippter-Text Animation", bei dir mir aufgefallen ist, dass die Animation nur auf das jeweilige Wort angewendetet wird, wenn es in einem div container steht und nicht in einem span element, span wurde bei mir nicht akzeptiert und ich habe lange nach dem Fehler gesucht, warum die Animation nicht klappt; Letzlich habe ich die Animation dann aber geändert, um mehrere Verben nacheinander durchloopen zu lassen.

- **Sprungmarken**: Zunächst Problem, dass beim Klick auf Menüpunkt der Sprung immer zu weit nach unten ging. Ich habe dann im Netz eine Lösung gefunden, bei der man eine leere Div mit der jeweiligen sprung ID versieht und der Sprung dann quasi an die Stelle dieser div box erfolgt und nicht auf die jeweilige Kapitelüberschrift. Vermute aber, dass es dafür eine "professionellere" Lösung gibt und recherchiere weiter.

- Bei diesem Projekt im Rahmen meiner Ausbildung beim DCI sollte **explizit kein Javascript** etc. verwendet werden. Ich würde JS jedoch künftig bei folgenden Elementen meiner Seite einsetzen: Bildergalerie (nicht mehr mit CSS transition: scale), Ausklappmenü für mobile Geräte (nicht mehr CSS checkbox trick)

## (Offene)Fragen

- Klären, ob man bei einem Onepager auch einen Bereich einbauen kann, wo man neben hoch und runter auch noch nach links und rechts scrollen kann, wie so eine Art "Nebentür" => mir ist bei anderen Seiten aufgefallen, dass der body für so eine Lösung display flex und flex direction row erhalten hat; hat bei mir aber nicht richtig funktioniert

- Responsive Design mit SASS: mehrere .scss dateien erstellen und dann in eine gemeinsame Datei importieren oder lieber alles in einer Datei?

- ineinander übergehende Bilder über backgroundimage in CSS oder wie lösen? => ja mit cross-fade (habe ich aber dann vorerst weggelassen, da github pages damit Probleme hat)

## Weitere ToDos (nach Präsentation)

- SCSS "aufräumen": Insbesondere bei den mediaqueries könnte man manches noch kürzen und zusammenfassen, damit es nicht doppelt vorkommt; zudem schauen, was man ggf. als mixin in der extra scss file zusammenfassen kann

- Styling weiter ausbauen: Formular (so gut wie gar nicht gestyled bisher), Unterseiten (Vita, Impressum, Webportfolio)

- Responsive Ansichten verbessern, erweitern

- Barrierefreiheit und UX verbessern: Kapitelüberschriften zu hell; Alternativtexte, Bilddateien verkleinern (aktuell noch zu groß => kleinere Ansichten für Vorschau und bei Klick auf jeweiliges Bild größere File mit besserer Qualität laden (später mit JS)); Buttons mit Inhalt sind teilweise zu klein bzw. Inhalt darin zu dicht aufeinander => überarbeiten!

- Kapitelhöhen nochmal so anpassen, dass Sprung auf das jeweilige Kapitel den jeweiligen Header etwas mehr abdeckt;

- Feedback aus meiner Weiterbildungsklasse einbauen, wo möglich
