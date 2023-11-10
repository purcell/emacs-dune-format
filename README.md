[![Melpa Status](http://melpa.org/packages/dune-format-badge.svg)](http://melpa.org/#/dune-format)
[![Melpa Stable Status](http://stable.melpa.org/packages/dune-format-badge.svg)](http://stable.melpa.org/#/dune-format)
[![Build Status](https://github.com/purcell/emacs-dune-format/actions/workflows/test.yml/badge.svg)](https://github.com/purcell/emacs-dune-format/actions/workflows/test.yml)
<a href="https://www.patreon.com/sanityinc"><img alt="Support me" src="https://img.shields.io/badge/Support%20Me-%F0%9F%92%97-ff69b4.svg"></a>

dune-format.el
============

This Emacs library provides commands and a minor mode for easily reformatting
dune files using dune's built-in format command.

Installation
=============

If you choose not to use one of the convenient
packages in [MELPA][melpa], you'll need to
add the directory containing `dune-format.el` to your `load-path`, and
then `(require 'dune-format)`.

Usage
=====

Call `dune-format`, `dune-format-buffer` or `dune-format-region` as convenient.

Enable `dune-format-on-save-mode` in `dune-mode` buffers like this:

```el
(add-hook 'dune-mode-hook 'dune-format-on-save-mode)
```

or locally to your project with a form in your .dir-locals.el like
this:

```el
((dune-mode
   (mode . dune-format-on-save)))
```

You might like to bind `dune-format` or `dune-format-buffer` to a key,
e.g. with:

```el
(define-key dune-mode-map (kbd "C-c C-f") 'dune-format)
```

[melpa]: http://melpa.org

<hr>

[💝 Support this project and my other Open Source work](https://www.patreon.com/sanityinc)

[💼 LinkedIn profile](https://uk.linkedin.com/in/stevepurcell)

[✍ sanityinc.com](http://www.sanityinc.com/)

[🐦 @sanityinc](https://twitter.com/sanityinc)
