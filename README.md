[![License GPL 3](https://img.shields.io/badge/license-GPL_3-green.svg)](http://www.gnu.org/licenses/gpl-3.0.txt)
[![GitHub
Release](https://img.shields.io/github/v/release/jethrokuan/company-org-roam)](https://img.shields.io/github/v/release/jethrokuan/company-org-roam)
[![MELPA](https://melpa.org/packages/company-org-roam-badge.svg)](https://melpa.org/#/company-org-roam)

## Synopsis

`company-org-roam` is a [company][company] backend for use with [org-roam]. In
Org-roam buffers, it provides completion for Org-roam files using its title.

![company-org-roam-gif](screenshot/company-org-roam.gif)

## Installation

You can install it using `use-package`:

```emacs-lisp
(use-package company-org-roam
  :ensure t
  ;; You may want to pin in case the version from stable.melpa.org is not working 
  ; :pin melpa
  :config
  (push 'company-org-roam company-backends))
```

Or in case you're using `use-package` with `straight.el`:

```emacs-lisp
(use-package company-org-roam
  :straight (:host github :repo "org-roam/company-org-roam")
  :config
  (push 'company-org-roam company-backends))
```

Or make sure `company-org-roam` is in your load path, and:

```emacs-lisp
(require 'company-org-roam)
(push 'company-org-roam company-backends)
```

[company]: https://company-mode.github.io/
[org-roam]: https://github.com/jethrokuan/org-roam
