
# Presentation Template

This template repository is meant as personal starting point to create [RevealJS](https://revealjs.com/) presentations from Markdown via [Quarto](https://quarto.org/). It should provide a skeleton for a quick entry, using a concise style between presentations and automatic rendering via Github workflows (only works in Public Repositories).

## The Readme

This file (README.md) is the entry point to the repository on Github. There are several ways to make it visually appealing. 

Ideally add an **Abstract**, in case it is in German also add a **Zusammenfassung**.

Use badges if appropriate, they can be created via https://shields.io/badges/static-badge and optionally contain logos from https://simpleicons.org. 

E.g. 
[![video recording](https://img.shields.io/badge/Video%20Recording-373b38?logo=youtube)](https://youtube.com)  [![presentation slides](https://img.shields.io/badge/Presentation%20Slides-373b38?logo=revealdotjs&logoColor=white)](https://wiesehahn.github.io/quarto_presentation_template/presentation.html)

```markdown

# Title

*(Presented at X)*

##### Keywords:
**Keyword1**, **Keyword2**

[![video recording](https://img.shields.io/badge/Video%20Recording-373b38?logo=youtube)](https://youtube.com)  [![presentation slides](https://img.shields.io/badge/Presentation%20Slides-373b38?logo=revealdotjs&logoColor=white)](https://wiesehahn.github.io/quarto_presentation_template/presentation.html)



#### Abstract

Template repository to help creating a presentation in Quarto which is rendered to RevealJS via Github Actions.

--- 

#### Description

This template repository is meant as personal starting point to create [RevealJS](https://revealjs.com/) presentations from Markdown via [Quarto](https://quarto.org/). It should provide a skeleton for a quick entry, using a concise style between presentations and automatic rendering via Github workflows (only works in Public Repositories).
```


### Get startet

The following files contain sample code (including variables such as website), please edit / replace the content:
- `presentation.qmd` (main file to add content for presentation) 
- `references.bib` (optionally, add references to be included)
- `_quarto.yml` (main file to change presentation settings)
- `_variables.yml` (optionally, add variables to be added in .qmd)

Informtion about Quarto Markdown syntax and options for RevealJS presentations can be found at https://quarto.org/docs/presentations/revealjs/.

#### Citation
The repository comes with a `CITATION.cff` file, which provides information about the correct citation. It is supported by Github, Zenodo and Zotero. 
Change fields to desired variables or delete completely. A file can also be created or updated using a [UI](https://citation-file-format.github.io/cff-initializer-javascript/#/).

To create a DOI for the repository you have to [connect to Zenodo](https://docs.github.com/de/repositories/archiving-a-github-repository/referencing-and-citing-content).

1. [toggle switch for repository](https://zenodo.org/account/settings/github/)
2. [ publish a release](https://docs.github.com/de/repositories/releasing-projects-on-github/managing-releases-in-a-repository)
3. (optionally) add DOI to `CITATION.cff` and as badge in `README.md`


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

#### [Iconify](https://github.com/mcanouil/quarto-iconify)

provides support to free and open source icons provided by [Iconify](https://icon-sets.iconify.design/), e.g.:
`{{< iconify typcn plus >}}`