# Markdown Mode for Emacs Processor

Markdown processor to be used with [Markdown Mode for Emacs](https://jblevins.org/projects/markdown-mode).

Converts Markdown to HTML via Pandoc and tweaks the output a bit so it looks good in the
[Emacs Web Wowser (EWW)](https://www.gnu.org/software/emacs/manual/html_mono/eww.html).

## Requirements

- Tcl
- Pandoc

## Installation

Open a terminal, change the current working directory to the desired location for this project,
and issue the following command:

```
git clone https://github.com/pvdhoef/emacs-markdown-mode-processor
```

## Configuration

Add the following to the Emacs configuration file `init.el`:

```
(setq markdown-command "<projects>/emacs-markdown-mode-processor/md2html")
```

Where `<projects>` is a placeholder for the full path to the folder containing the project.
