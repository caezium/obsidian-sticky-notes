# obsidian-sticky-notes

> Sticky Notes for Obsidian

<img src="https://github.com/dhniceday/obsidian-sticky-notes/blob/main/images/sticky-notes-readme1.png" alt="Sticky Notes in Obsidian" />

## Metadata

- different sizes [s-20, s-25, s-30 … s-95 in steps of 5 - default is 30%]

- different colors [yellow, green, red, blue, purple, aqua, orange, pink, brown, turquoise, salmon, indigo, magenta, violet - default is yellow]

- align left, right and center [left, right, center - default is center]
    - `left` / `right` **float** the sticky inside the text column and the paragraph wraps around it

- define if the first row should be bold [title - default is no title]

- use sticky notes as an **aside** (`aside left` or `aside right`) to place them in the margin, Cornell-cue style

- make a sticky **collapsible** by adding `+` (open) or `-` (closed) after the metadata, e.g. `> [!sticky]- My note`

<img src="https://github.com/dhniceday/obsidian-sticky-notes/blob/main/images/sticky-notes-aside.png" alt="Sticky Notes in Obsidian" />

## In the sticky notes

- text decoration for bold and italic is deactivated

- link color is aligned with sticky note's normal text color

- highlight color is adapted to the sticky note's color

## Options in style settings

- Sticky notes colors

- Choose the font 
    - Fonts are incorporated
    - All fonts are from Google Fonts

- Text size

- Offset for asides

- Zoom on hover (still experimental and not that pretty)

CSS is a bit rough (I'm not an expert). I have created that for myself. It blends into my own Gruvbox color scheme for the Minimal theme. But all of that can be easily modified in the css.

## Examples

```
> [!STICKY]
> The default sticky 
> (takes default color from Style Settings).
```

```
> [!STICKY|yellow left]
> Sticky Note
> This one floats left
```

```
> [!STICKY|green right title]
> Sticky Note
> This one floats right and has its first line bold
```

```
> [!STICKY|blue center s-45]
> Sticky Note
> This one is centered and a bit larger
```

```
> [!STICKY|aside left purple title]
> Sticky Note
> This one is put aside, purple with its first line bold
```

```
> [!STICKY|aside right blue]
> Sticky Note
> This one sits in the right margin
```

```
> [!STICKY|left green]
> Sticky Note
> This floats inside the column; the paragraph wraps around it
```

```
> [!STICKY|s-40 pink]- Reminder
> Sticky Note
> This one is collapsible and starts closed (note the trailing `-`)
```

> **Note on asides:** asides sit in the page margin, so they need room beside
> the text — keep **Settings → Editor → Readable line length** on. They render
> in Reading view; in Live Preview they stay visible but dimmed so you can edit
> them. If you don't use readable line length, use `left` / `right` float
> instead (the sticky stays in the column and the text wraps around it).
