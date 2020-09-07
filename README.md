# ess-r-insert-obj

Utilities to help inserting variable (column) names or values in ESS-R

## Installation

Clone this repository, or install from MELPA. Add the following to your `.emacs`:

``` elisp
(require 'ess-r-insert-obj)
```

## Usage

Data.frame-like object:

- [x] ess-r-insert-obj-dt-name

Column/Variable name: with `C-u C-u`, it prompt for the dt name for search in.

- [x] ess-r-insert-obj-col-name
- [x] ess-r-insert-obj-col-name-all

Column/Variable name: with `C-u C-u`, it prompt for the dt name for search in, or
with `C-u`, it prompt for column/variable name to search in.

- [x] ess-r-insert-obj-value
- [x] ess-r-insert-obj-value-all

## Customization

### ess-r-insert-obj-complete-backend-list

- jsonlite

### ess-r-insert-obj-read-string

- ess-completing-read (default)
- completing-read
- ido-completing-read
- ivy-completing-read
