tex-presentation
================

Template for starting a new latex beamer presentation.
Also defines some useful patterns which are described under [Built in features](#Built in features).

## How to use

1. Copy example.tex somewhere to use it as the base for your new presentation
2. adjust the `\featurePath` command definition to the relative path where features are located

## Built in features

To include all features, use

```tex
\input{features/all}
```

### TikZ overlay

```tex
\input{features/overlays/def}
```

Simple putting text or images in a relative positioned overlay.

```tex
\tikzoverlay at (-1cm,-5cm) (name) {%
	content
};%
```

There are 3 types of overlays:
- `tikzoverlay` overlay with white background
- `tikzboverlay` overlay with bordered background
- `tikztoverlay` overlay with transparent background

### Speech bubbles

```tex
\input{features/bubbles/def}
```

TODO

### Colored tables

```tex
\input{features/tablecolors/def}
```

TODO
