# Einleitung

*Einleitung...*

# Wissenschaftliches Publizieren

*Allgemeines zu wissenschaftlichem Publizieren (aktueller Stand)...*

Die Landschaft des wissenschaftlichen Publizierens ist sehr heterogen. Die Publikationspraxis ist sehr unterschiedlich

* in der Publikationsfrequenz
* in der Publikationserstellung
* in dem Publikationszugang.

Diese hängen stark von der Fachdisziplin oder dem ab. Informatiker, Naturwissenschaftler und Mathematiker
benutzen i.d.R. Latex zur Publikationserstellung. In anderen Fachgebieten wird Word bevorzugt. Zudem haben
Verlage ihre eigenen Vorlagen, mit denen die Publikationen zu erstellen sind. Es muss betont werden, dass diese Techniken auf ein druckfertiges Manuskript abzielen. Eine parallele Publikation in einem anderen 
Format (wie z.b. HTML) wird kaum praktiziert.

Weiterhin besteht und wächst die Notwendigkeit zur kollaborativen Erstellung
von Manuskripten. Hierfür sind ein Versionierungssystem und ein einfaches Textformat besonders hilfreich, z.B. __git__ und __Markdown__. Mit 
diesen Tools lassen sich Textänderungen des Koautors sehr leicht nachvollziehen.

Einige Wissenschaftler haben diese Möglichkeiten zu schätzen gelernt und daher eine Initiative gestartet, um Markdown um "wissenschaftliche Elemente" anzureichern, __Scholarly Markdown__.

* Verlage verlangen in der Regel druckfertiges Manuskript
* In vielen Naturwissenschaften ist LaTeX de-facto Standard.
* Nachteile der aktuellen Situation
* Markdown als Alternative
    * Artikel und Vortragsfolien
    * Vereinzelt schon Dissertationen und Bücher in Markdown
    * Initiative zur Entwicklung von "Scholarly Markdown"

# Markdown

Markdown ist eine Auszeichnungsprache für einfache Textdokumente, die mit dem
Ziel entwickelt wurde, so einfach wie möglich lesbar und schreibbar zu sein.
Verglichen mit anderen Auszeichnungssprachen kommt die Markdown-Syntax mit
wenigen Sonderzeichen aus und folgt in der Regel üblichen Gepflogenheiten
(siehe Tabelle 1 und das folgende Kapitel). Da Markdown-Dokumente
ausschließlich aus (Unicode-)Zeichen bestehen reicht zur Bearbeitung ein
beliebiger Texteditor.

| HTML        | TEI                      | LaTeX         | Markdown |
|-------------|--------------------------|---------------|----------|
|`<b>fett</b>`|`<hi rend="bold">fett</b>`|`\textbf{fett}`|`**fett**`|

:Hervorhebung eines Wortes als **fett** in verschiedenen Auszeichnungsprachen

Ursprünglich wurde Markdown 2004 von John Gruber und Aaron Swartz als einfache
Alternative zur Erstellung von HTML-Texten entwickelt [@Swartz2004]. Dazu
lassen sich Dokumente in Markdown-Syntax mit einem Script nach HTML
konvertiert. Ein solches Konvertierungsskript stellte Gruber zusammen mit der
Spezifikation der Markdown-Syntax Ende 2004 bereit [@Gruber2004]. Auf dieser
Basis wurden in den folgenden Jahren zahlreiche Anwendungen entwickelt, die zur
Popularität von Markdown beitrugen. Zu den größten Webseiten, bei denen Nutzer
Kommentare und andere Inhalte in Markdown-Syntax verfassen können, zählen
[GitHub](http://github.com), [Stack Exchange](http://stackexchange.com/) 
und [reddit](http://www.reddit.com/).

Da Gruber eine Weiterentwicklung von Markdown ablehnt und sein Standard einige
Uneindeutigkeiten enthält, gibt es inzwischen verschiedene Markdown-Dialekte,
die die Syntax um zusätzliche Elemente erweitern. Zur Vereinheitlichung wurde
Ende 2014 der CommonMark-Standard geschaffen [@MacFarlane2014].

## Bestandteile und Syntax

Markdown abstrahiert weitgehend von visuellen Eigenschaften wie Schriftart,
Zeilenabstand und Blocksatz. Stattdessen konzentriert sich die Syntax auf die
wesentlichen Bestandteile eines Textdokumentes.

*Übersicht der Markdown-Syntax...*

### Block-Elemente

* Absätze
* Überschriften
* Listen
* Code-Abschnitte
* Zitat-Abschnitte
* Horizontale Linie

### Inline-Auszeichnung 

Textformatierung u.A.

* Fett
* Kursiv
* Code
* Links und URLs
* Zeilenumbrüche
* Bilder (können auch als Block-Elemente verwendet werden)
* strike/Hoch/tiefstellung (erweiterung)
* Link-Referenzen
* Sonstige Elemente
    * Entities
    * Escape
    * HTML

## Erweiterungen für wissenschaftliches Publizieren

*Zusätzliche Bestandteile...*

* Fußnoten
* Interne Verweise
* Tabellen
* Abbildungs- und Tabellentitel
* Mathematische Formeln
* Zitationen und Literaturverzeichnis
* Dynamische Elemente (IPhyonNotebook, Kramdown...)

### Mathematische Formeln

In vielen ingenieur- und naturwissenschaften, in der Mathematik und in der Informatik ist die
Darstellung mathematischer Formeln von essentieller Bedeutung. Daher werden diese Aspekte und hier näher beleuchtet. [@Kr

Es lassen sich die üblichen Latex-Befehle verwenden. Gekennzeichnet wird ein Latex-Befehl mit . So wird der Befehl

$$\int_0^{\infty}f(x)dx$$

$$x=x+1*\zeta$$

so lassen sich math. Elemente in Markdown darstellen.


# Markdown-Werkzeuge

*Einleitung dieses Kapitels...*

## Markdown-Editoren

Zur Bearbeitung von Markdown-Dokumenten reicht ein beliebiger
Texteditor wie zum Beispiel TextPad oder Notepad++ unter Windows und
vim unter Linux.  Darüber hinaus gibt es inzwischen zahlreiche
spezialisierte Markdown-Editoren mit zusätzlichen Funktionen wie
Syntax-Highlighting, HTML-Preview und Synchronisierung mit
Cloud-Diensten. Einige dieser Editoren müssen nicht erst installiert
werden sondern laufen direkt im Browser, sei es als eigenständige
Webanwendung^[Beispiele für webbasierte Markdown-Editoren: http://dillinger.io/, http://prose.io/, https://notex.ch/, http://markable.in/, http://slhck.info/markdown/, https://jgm.github.io/stmd/js/, https://jbt.github.io/markdown-editor/, http://markdown.pioul.fr/ uva.]
oder durch die Bereicherung von bestehenden Webseiten um
Markdown-Funktionalität.

Welcher Markdown-Editor am Besten geeignet ist, hängt von den eigenen
Anforderungen ab und lässt sich angesichts der raschen Entwicklung angebotener
Software nicht abschließend beantworten. Der Wechsel zwischen verschiedenen
Programmen ist allerdings relativ einfach möglich, da die Markdown-Syntax nicht
an eine Software gebunden ist.

*Weitere Editoren speziell für wissenschaftliches Schreiben ...*

* Authorea
* IPhytonNotebook, RStudio
* notex.ch
* ...?

## Pandoc

*Pandoc zur Konvertierung zwischen verschiedenen Dokumentformaten...*

* Ausgangsformate: HTML, PDF, ePUB...
* Templates für Layout-Anpassungen zur einheitlichen Gestaltung von Dokumenten

Neben der Erstellung von Dokumenten in verschiedenen Ausgabeformaten  kann
Pandoc auch vorhandene Dokumente nach Markdown-Syntax konvertieren. Seit
Version 1.13 bietet das Programm neben HTML, LaTeX und MediaWiki-Syntax auch
Das DOCX als Importformat an.

Beispiele für Bücher, die mit Markdown und Pandoc erstellt wurden:
@Kofler2013, @Voss2014, ...

# Stand der wissenschaftlichen Markdown-Nutzung

* Zunehmend als Alternative zu LaTeX, allerdings noch eher einzelne Autoren
* Wie Knuth bei TeX hat der MacFarlane Pandoc auch als Wissenschaftler für 
  seine eigene Publikationstätigkeit entwickelt
* LIBREAS & Informationspraxis (geplant) nutzen Markdown, um Artikel
  medienneutral bereitzustellen (gibt es weitere?!)
* Markdown-for-Science / Scholarly Markdown Workshop
* BeyondPDF-Initiativen, um von der Fokussierung auf die Druckversion
  wegzukommen
* ...

# Zusammenfassung & Ausblick

*Zusammenfassung, Bewertung, Ausblick...*

Markdown als Ausgangsformat für wissenschaftliche Publikationen, 
Medienneutrales Publizieren mit Scholarly Markdown...

* Scholarly Markdown
* Trend: Reproduzierbare Forschung
    * Quelltext und Beschreibung in einem Dokument 
      (z.B. Berechnungen in einem Fachartikel)
    * Beispiel: R markdown mit knitr [@Xie2014; @Baumer2014; @Gandrud2013]
* Nachteile von Markdown (u.A. kein WYSIWYG)
* Verweise auf Beispiele und andere Tutorials
* ...

Abbildung:\
Markdown\
&#8594; Konvertierungsprogramm\
&#8594; Druckfertiges Ausgabeformat oder HTML

# Literatur {.unnumbered}
