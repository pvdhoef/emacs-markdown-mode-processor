# Markdown Mode for Emacs Processor

Markdown processor to be used with [Markdown Mode for Emacs](https://jblevins.org/projects/markdown-mode).

Converts Markdown to HTML via Pandoc and includes additional formatting adjustments to enhance the appearance of
the output in [Emacs Web Wowser (EWW)](https://www.gnu.org/software/emacs/manual/html_mono/eww.html).

## Requirements

The following tools must be installed and accessible from the command line:

- [Tcl](https://www.tcl-lang.org/)
- [Pandoc](https://pandoc.org/)

## Installation

Issue the following command:

```sh
git clone https://github.com/pvdhoef/emacs-markdown-mode-processor /path/to/emacs-markdown-mode-processor
```

Add the following to the Emacs configuration file `init.el`:

```lisp
(setq markdown-command "/path/to/emacs-markdown-mode-processor/md2html")
```

Make sure that the full path to `md2html` is specified.
The tool uses a number of other files in the same directory and should be able to find them.

## Configuration

The script includes several configurable variables:

- `INDENT_PRE`: Adjusts indentation for `<pre>` blocks.
- `EXTRA_BREATHING_SPACE_FOR_PRE`: Adds extra spacing around `<pre>` blocks.
- `HR_BEFORE_AND_AFTER_PRE`: Inserts `<hr>` before and after `<pre>` blocks.
- `BR_AFTER_TABLE`: Adds line breaks after tables.

These can be modified within the script to suit your preferences.

The tool uses a template (`template.html`) and style sheet (`template.css`)
that can also be customized to your own liking.
