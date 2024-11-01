# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Installs

* Skipping Conda / whichever package manager you choose to use

``` py
pip install mkdocs
pip install pymdown-extensions
```

``` bash
cd ~/Downloads/MoBI_Docs
mkdocs serve
```

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Other Useful Markdown tools:

### Lists

Magnique moenia Herculis Daedalon amnis humus limen, dent cum tenent arbiter:
nulli. Quodque [saepes](http://versatnon.net/pictispartes), quas gestu
alimentaque ulvae postquam **fata sonumque**! Ima **prius**, est ardere summo,
et longa caelum occumbere in dixerat trementi.

#### Unordered Lists

- Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur
  accumsan nibh eu mattis. Vivamus tempus velit eros, porttitor placerat nibh
  lacinia sed. Aenean in finibus diam.

    * Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    * Nam vulputate tincidunt fringilla.
    * Nullam dignissim ultrices urna non auctor.

#### Ordered Lists

1.  Vivamus id mi enim. Integer id turpis sapien. Ut condimentum lobortis
    sagittis. Aliquam purus tellus, faucibus eget urna at, iaculis venenatis
    nulla. Vivamus a pharetra leo.

    1.  Vivamus venenatis porttitor tortor sit amet rutrum. Pellentesque aliquet
        quam enim, eu volutpat urna rutrum a. Nam vehicula nunc mauris, a
        ultricies libero efficitur sed.

    2.  Morbi eget dapibus felis. Vivamus venenatis porttitor tortor sit amet
        rutrum. Pellentesque aliquet quam enim, eu volutpat urna rutrum a.

        1.  Mauris dictum mi lacus
        2.  Ut sit amet placerat ante
        3.  Suspendisse ac eros arcu

#### Definition Lists

`Lorem ipsum dolor sit amet`

:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus
    tellus non sem sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`

:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin
    ut eros sed sapien ullamcorper consequat. Nunc ligula ante.

#### Task Lists

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque

### Quotes and Codeblocks

Illos in cupidine avidi. Sub albus claro **nitidum sidere nitentia** irascere,
**silva omnes** terrebit. At Thracum virgae dicta. Auras ferventibus vestis
pervenientia detrahat Baucis, cervice sit mentoque, virtus? Exhortor palmite
poposcit, non aetas stratosque licet Nereides: nacta inpatiens modo nihil deorum
vilibus.

> Nec Procne erit proelia, umeris quem, petunt, **est positis erat**. Per
> dominum tractata. Sustinet quo; virilem cognoscere visa, in imago.

Per visus Lycaoniae cortice. Dixit in despecta umbra. Me tulit flumine imas
dicor aetatis orbam insula ultra sua densetur; ille. Lacteus orbis sed breve,
cara, e tortum tepido ferrum, *dolet* oblivia Hyries equidem saevior usus
**ventis**. Videre motasse, cum tela lyncum, servabunt mansit Arcadiae et
extemplo longa.

Lorem markdownum situsque ut ligari voluptas dummodo moras fata vela lecti
fecere parentis saxea. Primordia quia timentem suadent Heliades, Tonantis aves
nunc tenditur. Latuere volenti solita et inprudens feras. Vidi Lichan at Aeson
et **lapis reluxit**. Viri medio tamen thalami tinguet, clausas, in ambit mille,
ego invadunt Dauno illi!

``` py
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```



### Colored Text (in-line html)

Orange words incoming: <span style="color:orange;">Word up</span>.


### Sub & Superscript

29^th^ H~2~O

### Emojis & Keyboard Keys

:dog: :cat: :) 😀 🫔  💀[find emojis here](https://emojipedia.org/)

++ctrl+alt+del++ [link to all the keys](https://facelessuser.github.io/pymdown-extensions/extensions/keys/#extendingmodifying-key-map-index)


### Marked Text & Footnotes

==Hello Everyone (highlight + bold)==

^^Hello Everyone (highlight)^^

~~Hello Everyone (strikethrough)~~

Footnote 1[^1].

Footnote 2[^2].


[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
[^2]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.

### Abbreviations and Tooltips

#### Text with abbreviations

The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language
*[W3C]: World Wide Web Consortium

#### Link with tooltip, inline syntax

[Hover me](https://example.com "I'm a tooltip!")

#### Link with tooltip, reference syntax

[Hover me][example]

  [example]: https://example.com "I'm a tooltip!"
