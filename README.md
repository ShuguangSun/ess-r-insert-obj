# ess-r-insert-obj

Utilities to help inserting variable (column) names or values in ESS-R.

ESS-R has it own completing system, e.g., `ess-r-complete-object-name` and
`ess-r-get-rcompletions`. For example, if `dt` is a data.frame, after the `$`
(`dt$|`), the completing list of variables in the data.frame will be prompted.

However, if we works with tidyverse, the completing system is not so helpful.
This package provide the utilities to help completing names of data frame or
variable values in a semi-automatic way.

## Installation

Clone this repository, or install from MELPA. Add the following to your `.emacs`:

``` elisp
(require 'ess-r-insert-obj)
```

## Usage

Data.frame-like object:

- M-x ess-r-insert-obj-dt-name

Variable (Column) name: with `C-u C-u`, it prompt for the dt name for search in.

- M-x ess-r-insert-obj-col-name
- M-x ess-r-insert-obj-col-name-all

Variable (Column) value: with `C-u C-u`, it prompt for the dt name for search in, or
with `C-u`, it prompt for column/variable name to search in.

- M-x ess-r-insert-obj-value
- M-x ess-r-insert-obj-value-all

## Customization

### ess-r-insert-obj-complete-backend-list

- jsonlite

### ess-r-insert-obj-read-string

- ess-completing-read (default)
- completing-read
- ido-completing-read
- ivy-completing-read
