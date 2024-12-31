# Markdown Mode for Emacs Pocessor

Markdown processor to be used with [Markdown Mode for Emacs](https://jblevins.org/projects/markdown-mode).

Converts Markdown to HTML via Pandoc and tweaks the output a bit so it looks good in the
[Emacs Web Wowser](https://www.gnu.org/software/emacs/manual/html_mono/eww.html) (EWW).

## Configuration

Add the following to Emacs `init.el`:

```
(setq markdown-command "<projects-home>/emacs-markdown-mode-processor/md2html")
```

## Requirements

- Tcl
- Pandoc
