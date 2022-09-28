# Notes about Beamer's themes

The idea of this document is to compile information about how a Beamer theme works and is created.

## Themes - Five Flavors of Themes

Themes make it easy to chenge the appearance of a presentation. The BEAMER class uses five different kinds of themes:

- **Presentation Themes** Conceptually, a presentation theme dictates for single detail of a presentation what i look like. Thus, choosing a particular presentation theme will setup for, say the numbers in enumeration what color they have, what color their background has, what font is used to render them, whether a circle or ball or rectangle or whatever is drawn behind them, and so forth. Thus, when you choose a presentation theme, your presentation will look the way someone (the creator of the theme) thought that a presentation should look like. Presentation themes typically only choose a particular color theme, font theme, inner theme, and outer theme that go well together.
- **Color Themes** A color theme only dictates which colors are used in a presentation. If you have chosen a particular presentation theme and then choose a color theme, only the colors of your presentation will change. A color theme can specify colors in a very detailed way: For example, a color theme can specifically change the colors used to render, say, the border of a button, the brackground of a button, and the text on a button.
- **Font Theme** A font theme dictates which fonts of font attributes are used in a presentation. As for colors, the font of all text elements used in a presentation can be specified independently.
- **Inner Theme** An inner theme specifies how certain elements of a presentation are typeset. This includes all elements that are at the "inside" of the frame, that is, that are not part of the headline, footline, or sidebars. This includes all enumerations, itemize environments, block environments, theorem enviroments, or the table of contents. For example, an inner theme might specify that in an enumeration the should be typqeset without a dot and that a small circle should be shown behind it. The inner theme would not specify what color should be used (this is the job of the color theme) nor which font should be used (this is the job of the font theme).
- **Outer Themes** An outer theme specifies what the "outside" or "border" of the presentation slides should look like. it specifies whether there are head- and footlines, what is shoen in them, whether there is a sidebar, where the logo goes, where the navigation symbols and bars go, and so on. It also specifies where the frametitle is put and how it is typeset.

## Como se distribuye la informacion

    \usetheme[options]{XXX}

Los temas de Beamer se componen de un archivo principal que la da el nombre al tema, la sintaxis para nombrarlo es:

    beamerthemeXXX.sty

donde `XXX` es el nombre del tema. Este archivo contiene todas las definiciones y opciones que construiran el tema.


El archivo:

    beamercolorthemeXXX.sty

incluye todas las definiciones de color del tema.