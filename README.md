# Markdown Mode for Emacs Processor

Markdown processor to be used with [Markdown Mode for Emacs](https://jblevins.org/projects/markdown-mode).

Converts Markdown to HTML via Pandoc and tweaks the output a bit so it looks good in the
[Emacs Web Wowser (EWW)](https://www.gnu.org/software/emacs/manual/html_mono/eww.html).

## Configuration

Add the following to the Emacs configuration file `init.el`:

```
(setq markdown-command "<projects-home>/emacs-markdown-mode-processor/md2html")
```

## Requirements

- Tcl
- Pandoc
