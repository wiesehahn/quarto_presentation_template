
# Presentation Template

This template repository is meant as personal starting point to create [RevealJS](https://revealjs.com/) presentations from Markdown via [Quarto](https://quarto.org/). It should provide a skeleton for a quick entry, using a concise style between presentations and automatic rendering via Github workflows (only works in Public Repositories).


### Get startet

The following files contain sample code (including variables such as website), please edit / replace the content:
- `presentation.qmd` (main file to add content for presentation) 
- `references.bib` (optionally, add references to be included)
- `_quarto.yml` (main file to change presentation settings)
- `_variables.yml` (optionally, add variables to be added in .qmd)


Informtion about Quarto Markdown syntax and options for RevealJS presentations can be found at https://quarto.org/docs/presentations/revealjs/.

#### References

References can be manually inserted in the `references.bib` file and cited via their key (e.g. `[@Wiesehahn_2023]`. 

Alternatively references can be managed within Zotero and synchronized with the `references.bib`,  plugins such as the *Citation Picker for Zotero* in VS Code help to insert citations (e.g. via `alt`+`shift`+`z`).

https://quarto.org/docs/authoring/footnotes-and-citations.html


### Pre-installed extensions

#### [Quarto social embeds](https://github.com/sellorm/quarto-social-embeds)

Use to embed GitHub gists, Twitter, Youtube, Vimeo, Mastodon, e.g.:
`{{< gist wiesehahn 6b6c215c227341f4faab03ff96fa7f1b >}}`

#### [Attribution](https://github.com/quarto-ext/attribution)

Use to display attribution text sideways, e.g.:
```r
::: {.attribution}
by [@Jens Wiesehahn](https://wiesehahn.github.io/)
:::
```

#### [Lightbox](https://github.com/quarto-ext/lightbox)

Use to add lightbox styling and behavior to images in HTML documents, e.g.:

`![logo](images/triangle_logo.png){.lightbox}`

#### [Verticator](https://github.com/Martinomagnifico/quarto-verticator)

Adds indicators to show the amount of slides in a vertical stack.

#### [Qrcode Extension for Quarto](https://github.com/jmbuhr/quarto-qrcode)

Provides shortcodes for qrcodejs in quarto, e.g.:

`{{< qrcode https://github.com/jmbuhr/quarto-qrcode >}}`