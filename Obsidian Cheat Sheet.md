[Obsidian Help](https://help.obsidian.md)
[Obsidian.md Markdown Cheat Sheet](https://obsidian-school.com/obsidian-basics/obsidian-cheat-sheet/)

# Block Quote

>  Sample Text

# Footnote
This is a simple footnote[^1]. Here is another one [^2]. 


[^1]: This is the referenced text. 
[^2]: Add 2 spaces at the start of each new line. This lets you write footnotes that span multiple lines.

Page Break (three underscores)
___
# Styling text

| Style                  | Syntax                 | Example                                  | Output                                 |
| ---------------------- | ---------------------- | ---------------------------------------- | -------------------------------------- |
| Bold                   | `** **` or `__ __`     | `**Bold text**`                          | **Bold text**                          |
| Italic                 | `* *` or `_ _`         | `*Italic text*`                          | _Italic text_                          |
| Strikethrough          | `~~ ~~`                | `~~Striked out text~~`                   | ~~Striked out text~~                   |
| Highlight              | `== ==`                | `==Highlighted text==`                   | ==Highlighted text==                   |
| Bold and nested italic | `** **` and `_ _`      | `**Bold text and _nested italic_ text**` | **Bold text and _nested italic_ text** |
| Bold and italic        | `*** ***` or `___ ___` | `***Bold and italic text***`             | **_Bold and italic text_**             |
# Links
## Link to another note
`[[Page to link to]]`
[[Test]]
## Link to a block of text inside a note
`[[Page Link^block to link to]]`
[[Test#^739e21]]
[[Test#^a9b655]]
## Link to a page heading
`[[Page Link#The Heading]]`
[[Test#Test 1]]
[[Test#Test 2]]
## Link Aliases
`[[Page Link|Alias]]`
[[Test|Alias]]

# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6

# Lists

## Ordered List
1. This
2. is an
3. Ordered list
  1. Indent by pressing tab

## Unordered List
- This
- is an
- Unordered list
  - Indent by pressing tab

## Task List
- [ ] This
- [ ] is a
- [ ] Task list
  - [ ] Indent by pressing tab

# Code Blocks

## HTML
```html
some code here
```

## Javascript
```javascript
some code here
```

## Markdown
```md
some code here
```

## Python
```python
some code here
```

# Tables
Recommended to install and enable the Table Plugin

'| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |'

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

(Shift+Enter to finish table)

# External links

If you want to link to an external URL, you can create an inline link by surrounding the link text in brackets (`[ ]`), and then the URL in parentheses (`( )`).

```md
[Obsidian Help](https://help.obsidian.md)
```

[Obsidian Help](https://help.obsidian.md)

You can also create external links to files in other vaults, by linking to an [Obsidian URI](https://help.obsidian.md/Concepts/Obsidian+URI).

```md
[Note](obsidian://open?vault=MainVault&file=Note.md)
```

## External images

You can add images with external URLs, by adding a `!` symbol before an [external link](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#External%20links).

```md
![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

![Engelbart](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)

You can change the image dimensions, by adding `|640x480` to the link destination, where 640 is the width and 480 is the height.

```md
![Engelbart|640x480](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```


![Engelbart|640x480](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)

If you only specify the width, the image scales according to its original aspect ratio.

```md
![Engelbart.jpg|100](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)
```

![Engelbart.jpg|100](https://history-computer.com/ModernComputer/Basis/images/Engelbart.jpg)

# Embedding web pages

Learn how to use the [iframe](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/iframe) HTML element to embed web pages in your notes.

To embed a web page, add the following in your note and replace the placeholder text with the URL of the web page you want to embed:

```html
<iframe src="INSERT YOUR URL HERE"></iframe>
```

> [!Note]
> Some websites don't allow you to embed them. Instead, they may provide URLs that are meant for embedding them. If the website doesn't support embedding, try searching for the name of the website followed by "embed iframe". For example, "youtube embed iframe".

>[!Tip]
>If you're using [Canvas](https://help.obsidian.md/Plugins/Canvas), you can embed a web page in a card. For more information, refer to [Canvas > Add cards from web pages](https://help.obsidian.md/Plugins/Canvas#Add%20cards%20from%20web%20pages).

## Embed a YouTube video

To embed a YouTube video, use the same Markdown syntax as [external images](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#External%20images):

```md
![](https://www.youtube.com/watch?v=NnTvZWp5Q7o)
```

![](https://www.youtube.com/watch?v=NnTvZWp5Q7o)
## Embed a tweet

To embed a tweet, use the same Markdown syntax as [external images](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#External%20images):

```md
![](https://twitter.com/obsdmd/status/1580548874246443010)
```

![](https://twitter.com/obsdmd/status/1580548874246443010)

# Comments

You can add comments by wrapping text with `%%`. Comments are only visible in Editing view.

```md
This is an %%inline%% comment.

%%
This is a block comment.

Block comments can span multiple lines.
%%
```

This is an %%inline%% comment.

%%
This is a block comment.

Block comments can span multiple lines.
%%

# Math

You can add math expressions to your notes using [MathJax](http://docs.mathjax.org/en/latest/basic/mathjax.html) and the LaTeX notation.

To add a MathJax expression to your note, surround it with double dollar signs (`$$`).

```md
$$
\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc
$$
```

$$
\begin{vmatrix}a & b\\
c & d
\end{vmatrix}=ad-bc
$$

You can also inline math expressions by wrapping it in `$` symbols.

```md
This is an inline math expression $e^{2i\pi} = 1$.
```

This is an inline math expression $e^{2i\pi} = 1$.

>For more information about the syntax, refer to [MathJax basic tutorial and quick reference](https://math.meta.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference).
>For a list of supported MathJax packages, refer to [The TeX/LaTeX Extension List](http://docs.mathjax.org/en/latest/input/tex/extensions/index.html).


# Callouts

Use callouts to include additional content without breaking the flow of your notes.

To create a callout, add `[!info]` to the first line of a blockquote, where `info` is the _type identifier_. The type identifier determines how the callout looks and feels. To see all available types, refer to [Supported types](https://help.obsidian.md/Editing+and+formatting/Callouts#Supported%20types).

```markdown
> [!info]
> Here's a callout block.
> It supports **Markdown**, [[Internal link|Wikilinks]], and [[Embed files|embeds]]!
> ![[og-image.png]]
```

> [!info]
> Here's a callout block.
> It supports **Markdown**, [[Internal link|Wikilinks]], and [[Embed files|embeds]]!

Callouts are also supported natively on [Obsidian Publish](https://help.obsidian.md/Obsidian+Publish/Introduction+to+Obsidian+Publish).

>[!Note]
>If you're also using the Admonitions plugin, you should update it to at least version 8.0.0 to avoid problems with the new callout feature.

### Change the title

By default, the title of the callout is its type identifier in title case. You can change it by adding text after the type identifier:

```markdown
> [!tip] Callouts can have custom titles
> Like this one.
```

> [!tip] Callouts can have custom titles
> Like this one.

You can even omit the body to create title-only callouts:

```markdown
> [!tip] Title-only callout
```

> [!tip] Title-only callout

## Foldable callouts

You can make a callout foldable by adding a plus (+) or a minus (-) directly after the type identifier.

A plus sign expands the callout by default, and a minus sign collapses it instead.

```markdown
> [!faq]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden when the callout is collapsed.
```

> [!faq]- Are callouts foldable?
> Yes! In a foldable callout, the contents are hidden when the callout is collapsed.

## Nested callouts

You can nest callouts in multiple levels.

```markdown
> [!question] Can callouts be nested?
> > [!todo] Yes!, they can.
> > > [!example]  You can even use multiple layers of nesting.
```

> [!question] Can callouts be nested?
> > [!todo] Yes!, they can.
> > > [!example]  You can even use multiple layers of nesting.

## Customize callouts

[CSS snippets](https://help.obsidian.md/Extending+Obsidian/CSS+snippets) and [Community plugins](https://help.obsidian.md/Extending+Obsidian/Community+plugins) can define custom callouts, or even overwrite the default configuration.

To define a custom callout, create the following CSS block:

```css
.callout[data-callout="custom-question-type"] {
    --callout-color: 0, 0, 0;
    --callout-icon: lucide-alert-circle;
}
```

The value of the `data-callout` attribute is the type identifier you want to use, for example `[!custom-question-type]`.

- `--callout-color` defines the background color using numbers (0–255) for red, green, and blue.
- `--callout-icon` can be an icon ID from [lucide.dev](https://lucide.dev/), or an SVG element.
  
Note about lucide icon versions

Obsidian updates Lucide icons periodically. The current version included is shown below; use these or earlier icons in custom callouts.  

Version `0.268.0`  
ISC License  
Copyright (c) 2020, Lucide Contributors

SVG icons

Instead of using a Lucide icon, you can also use a SVG element as the callout icon.

```css
--callout-icon: '<svg>...custom svg...</svg>';
```

### Supported types

You can use several callout types and aliases. Each type comes with a different background color and icon.

To use these default styles, replace `info` in the examples with any of these types, such as `[!tip]` or `[!warning]`.

Unless you [Customize callouts](https://help.obsidian.md/Editing+and+formatting/Callouts#Customize%20callouts), any unsupported type defaults to the `note` type. The type identifier is case-insensitive.

> [!note]
```md
> [!note]
> Lorem ipsum dolor sit amet
```

---

> [!abstract]
```md
> [!abstract]
> Lorem ipsum dolor sit amet
```

Aliases: `summary`, `tldr`

---

> [!info]
```md
> [!info]
> Lorem ipsum dolor sit amet
```

---

> [!todo]
```md
> [!todo]
> Lorem ipsum dolor sit amet
```

---

> [!tip]
```md
> [!tip]
> Lorem ipsum dolor sit amet
```

Aliases: `hint`, `important`

---

> [!success]
```md
> [!success]
> Lorem ipsum dolor sit amet
```

Aliases: `check`, `done`

---

> [!question]
```md
> [!question]
> Lorem ipsum dolor sit amet
```

Aliases: `help`, `faq`

---

> [!warning]
```md
> [!warning]
> Lorem ipsum dolor sit amet
```

Aliases: `caution`, `attention`

---

> [!failure]
```md
> [!failure]
> Lorem ipsum dolor sit amet
```

Aliases: `fail`, `missing`

---

> [!danger]
```md
> [!danger]
> Lorem ipsum dolor sit amet
```

Alias: `error`

---

> [!bug]
```md
> [!bug]
> Lorem ipsum dolor sit amet
```

---

> [!example]
```md
> [!example]
> Lorem ipsum dolor sit amet
```

---

> [!quote]
```md
> [!quote]
> Lorem ipsum dolor sit amet
```

Alias: `cite`

# Multiple cursors

Obsidian lets you edit text in multiple places at the same time using multiple cursors. You can add additional cursors by holding `Alt` (or `Option` on macOS) and selecting another position in the note.

To remove a selection along with all additional cursors, click anywhere in the note without holding a key. You can also remove the selection by pressing `Escape`.

## Rectangular selection

If you want to edit consecutive lines of text—for example, to turn paragraphs into list items—you can hold `Shift+Alt` (or `Shift+Option` on macOS) while dragging. You can also hold the middle mouse button while dragging.




