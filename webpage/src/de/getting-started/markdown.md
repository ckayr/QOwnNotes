# Markdown

Dieses Markdown-Cheatsheet dient als Kurzreferenz und Beispiel für die Markdown-Syntax in QOwnNotes.

## Überschriften

Verwenden Sie Überschriften, um Ihre Texte zu strukturieren.

```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```

::: tip
Das **Navigation panel** zeigt die Struktur Ihrer Überschriften.
:::

Alternativ für H1 und H2; eine unterstrichene Schriftweise:

```markdown
Alt-H1
======

Alt-H2
------
```

::: tip
Standardmäßig erstellt QOwnNotes den **Dateinamen einer Notiz** aus der **Überschrift 1** (h1).
:::

## Hervorhebung

```markdown
Hervorhebung durch "Kursivschrift", mit *Sternchen*.

Starke Hervorhebung, auch: "fett", mit **Sternchen**.
```

::: tip
Sie können die [Tastenkombination](./shortcuts.md) <kbd>Strg + B</kbd> verwenden, um Text fett hervorzuheben, und <kbd>Strg + I</kbd>, um ihn kursiv hervorzuheben.
:::

## Unterstreichen

Es gibt auch eine optionale Einstellung zum Aktivieren des Unterstreichungs-Hervorhebung in den *Preview settings*.

```markdown
_unterstreichen_
```

::: tip
Sie können den [shortcut](./shortcuts.md) <kbd>Ctrl + U</kbd> verwenden, um einen Text zu unterstreichen.
:::

## Durchstreichen

```markdown
~~durchstreichen~~
```

::: tip
Sie können den [shortcut](./shortcuts.md) <kbd>Alt + Shift + S</kbd> verwenden, um einen Text durchzustreichen.
:::

## Listen

Es gibt viele Möglichkeiten, Listen zu erstellen.

```markdown
1. Als Erstes bestimmter Listeneintrag
2. Ein weiterer Eintrag
   * Ungeordnete Unterliste.
1. Tatsächliche Zahlen spielen keine Rolle, nur dass es eine Zahl ist!
   1. Geordnete Unterliste (funktioniert nur im Editor, nicht in der Vorschau)
4. Und noch ein Eintrag.

* Ungeordnete Liste kann Sternchen verwenden
- Oder Minusse
+ Oder Plusse
```

::: tip
Wenn Sie am Ende einer Liste die <kbd>Enter</kbd> -Taste drücken, wird ein neues Listenelement erstellt.
:::

## Links

Es gibt mehrere Möglichkeiten, Links zu erstellen.

```markdown
[Ich bin ein Inline-Link] (https://www.google.com)

[Ich bin ein Inline-Link mit Titel] (https://www.google.com "Googles Homepage")

[Sie können Zahlen für Referenzdefinitionen im Referenzstil verwenden] [1]

URLs und URLs in spitzen Klammern werden in der Vorschau automatisch in Links umgewandelt. 
http://www.example.com oder <http://www.example.com>

[1]: https://www.qownnotes.org
```

::: tip
Sie können den [shortcut](./shortcuts.md) <kbd>Ctrl + L</kbd> verwenden: **Erstellen Sie Links zu Webseiten oder anderen Notizen**.

Wenn Sie <kbd>Strg + Umschalt + X</kbd> verwenden, wird ein Dialogfeld angezeigt, durch den Sie in Ihre Notiz **Anhänge einfügen** können.

Sie können <kbd>Strg + Leertaste</kbd> drücken, während sich der Cursor auf einem Link in der Notizbearbeitung befindet, um dem Link zu folgen.
:::

### Lesezeichen

Die von der [QOwnNotes Web Companion-Browsererweiterung](./browser-extension.md) verwendeten Lesezeichen verwenden Links in Listen.

```markdown
- [Name der Webseite] (https://www.example.com) #tag1 #tag2 einige Beschreibungen und Tags
```

## Bilder

Bilder können in QOwnNotes eingebettet werden. Sie werden in der Vorschau angezeigt.

```markdown
![alt text](media/my-image.jpg)
```

::: tip
Sie können die [Tastenkombination](./shortcuts.md) <kbd>Strg + Umschalt + I</kbd> verwenden, um ein Bild in eine Notiz einzufügen. Das Bild kann sich auch in der Zwischenablage befinden. Das Dialogfeld erkennt es und zeigt eine Vorschau an.

Sie können ein Bild auch direkt aus der Zwischenablage mit <kbd>Strg + Umschalt + V</kbd> in Ihre Notiz einfügen.
:::


## Inline-Code und Code-Blöcke

```markdown
Inline-`Code` hat `Back-Ticks`.
```

Sie können die [Verknüpfung](./shortcuts.md) <kbd>Strg + Umschalt + C</kbd> für ausgewählten Inline-Text oder nur innerhalb von Text verwenden, um einen Inline-Codeblock zu erstellen.
:::

Codeblöcke werden entweder durch Zeilen mit drei Back-Ticks eingezäunt oder mit vier Leerzeichen eingerückt.

### Code-Blöcke mit vier führenden Leerzeichen

Fügen Sie vier Leerzeichen vor Ihrem Code hinzu, um ihn als Codeblock zu markieren.

```markdown
    s = "Code mit Leerzeicheneinzug"
     drucken s
```

### Code-Blöcke mit Backticks

Sie können auch drei Backticks verwenden, um einen Codeblock zu erstellen.
~~~markdown
```
Code wird hierhin geschrieben
Code wird hierhin geschrieben
```
~~~

::: tip
Sie können die Verknüpfung [shortcut](./shortcuts.md) <kbd>Strg + Umschalt + C</kbd> in mehreren ausgewählten Textzeilen oder in einer leeren Zeile verwenden, um einen Codeblock zu erstellen.
 
:::

### Backtick-Zaun mit Code-Hervorhebung

Es gibt auch einige Syntaxhervorhebungen mit Codeblöcken in QOwnNotes.

~~~markdown
```bash
# Ich bin ein Kommentar
cd Notes
```
~~~

Currently, supported languages (and code block identifiers) are:

* BASh scripting, `bash`
* C, `c`
* C++, `cpp`
* C++, `cxx`
* C++, `c++`
* C#, `c#`
* CMake, `cmake`
* C#, `csharp`
* CSS, `css`
* Go, `go`
* HTML, `html`
* INI, `ini`
* Java, `java`
* JavaScript, `javascript`
* JavaScript, `js`
* JSON, `json`
* Makefile, `make`
* PHP, `php`
* Python, `py`
* Python, `python`
* QML, `qml`
* Rust, `rust`
* Shell scripting, `sh`
* SQL, `sql`
* TypeScript, `ts`
* TypeScript, `typescript`
* V, `v`
* Vex, `vex`
* XML, `xml`
* YAML, `yml`
* YAML, `yaml`

## Tables

Tables aren't part of the core Markdown spec, but the QOwnNotes preview supports them. 

~~~markdown
Doppelpunkte können zum Ausrichten von Spalten verwendet werden.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

Es müssen mindestens 3 Striche vorhanden sein, die jede Kopfzelle trennen.

Sie können auch Inline-Markdown verwenden.

| Abschlag | Weniger | Hübsch |
| --- | --- | --- |
| `Rendert` | *immer noch* | **schön** |
| 1 | 2 | 3 |
~~~

::: tip
Press <kbd>Alt + Shift + T</kbd> to activate a dialog that can help you to create tables. In diesem Dialog können Sie sogar CSV-Dateien importieren!

Verwenden Sie <kbd>Strg + Leertaste</kbd> in einer Markdown-Tabelle, um sie automatisch zu formatieren.
:::

## Zitat-Blöcke

```markdown
> Blockzitate sind in E-Mails sehr praktisch, um sich in Antworttexten auf einen zitierten Textteil zu beziehen.
> Diese Zeile ist Teil desselben Zitats.

Zitatpause.

> Dies ist eine sehr lange Zeile, die beim Umbruch immer noch richtig zitiert wird. Oh Mann, lass uns weiter schreiben, um sicherzustellen, dass dies lang genug ist, um tatsächlich für alle umgebrochen zu werden. Oh, du kannst **Markdown** in ein Blockquote *setzen*. 
```

::: tip
Sie können QOwnNotes anweisen, Blockzitate oder nur das Blockzitatzeichen in den *Editoreinstellungen* vollständig hervorzuheben

Sie können die [ Verknüpfung ](./shortcuts.md) <kbd> Strg + Umschalt + B </kbd> verwenden, um Text als Blockzitat zu markieren.
:::

## Horizontale Linie

Es gibt drei Möglichkeiten, um eine horizontale Regel zu erhalten: Bindestriche, Sternchen oder Unterstriche.

```markdown
Drei oder mehr ...

Bindestriche

---

Sternchen

***

Unterstriche

___
```

## Zeilenumbrüche

- You can break a paragraph into more than a single line for easier editing, they still render as a single paragraph with no breaks.
- You can force a line break inside a paragraph by ending a line with two spaces.
- You can make a separate paragraph by delimiting it by empty lines.

::: tip
You can enter two spaces and a newline with <kbd>⇧ Shift</kbd> + <kbd>Return</kbd>.
:::

```markdown
Hier ist eine Zeile, mit der wir beginnen sollten.

Diese Zeile ist durch zwei Zeilenumbrüche von der obigen getrennt, sodass es sich um einen *separaten Absatz* handelt.

Diese Zeile beginnt auch einen separaten Absatz, aber ...
Diese Zeile wird nur durch zwei nachgestellte Leerzeichen und eine einzelne neue Zeile getrennt, sodass es sich um eine separate Zeile im *gleichen Absatz* handelt.
```

::: tip
Trailing spaces are highlighted by default in the editor.
:::

## Kommentare

Comments are not shown in the preview.

```markdown
[Kommentar]: # (Dieser Kommentar wird nicht in der Vorschau angezeigt.)

<! - HTML-Kommentare sind ebenfalls ausgeblendet - >
```

::: tip
A leading html comment block in a note will also be ignored in the automatic note filename generation.
:::

## Kontrollkästchenlisten

You can create simple todo lists with checkbox lists.

```markdown
- [x] done
- [ ] todo
```

::: tip
You can check/un-check checkboxes in the preview.
:::

## Inhaltsübersicht

In QOwnNotes you can use a frontmatter (e.g. YAML) to add some extra meta information. It will **not be shown in the preview** and will **not disturb the the automatic note filename generation**.

```markdown
---
Titel: Ein Name
Beschreibung: Ein wenig Beschreibung
---

# Notiz Überschrift beginnt hier

Etwas Text
```

The filename of this example note would be `Note headline starts here.md`.
