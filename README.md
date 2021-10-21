# Nohello

This is the source of [this](https://felixnext.github.io/doresearch/) website.

## Build

There is a Github Action in place to deploy any changes to `index.md` to the
`index.html` site when pushing to `master` branch.

To generate the HTML file from Markdown manually,
[pandoc](https://github.com/jgm/pandoc) is used:

```
pandoc --standalone --metadata pagetitle="doresearch" --css "assets/css/pandoc.css" --output=index.html index.md
```

## Acknowledgements

This website was inspired by the original at
[nohello.com](https://www.nohello.com/) and [sbmueller.nohello](https://sbmueller.github.io/nohello). Acknowledgements go to the original
anonymous author and sbmueller.
[Stylesheet](https://gist.github.com/forivall/7d5a304a8c3c809f0ba96884a7cf9d7e#file-gh-pandoc-css)
licensed under MIT license, Copyright (c) 2016-2017 Emily M Klassen.
