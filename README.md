# typora_basic_theme_revise
Instructions for revising typora basic themes (MacOS)




## config file location

* for general configuration: `/Applications/Typora.app/Contents/Resources/TypeMark/style/base.css`
* for user specific configuration: `~/Library/Application Support/abnerworks.Typora/themes/github.css`



## revise alert note block color

There are five types of alert:

1. note
2. caution
3. tip
4. important
5. warning

<img width="603" height="754" alt="image" src="https://github.com/user-attachments/assets/bd3e49fc-d026-457d-8b7e-419ee41d791b" />


In `base.css` file, we see the colors

```css
.md-alert.md-alert-note{border-left-color:#0969da}
.md-alert.md-alert-important{border-left-color:#8250df}
.md-alert.md-alert-warning{border-left-color:#9a6700}
.md-alert.md-alert-tip{border-left-color:#1f883d}
.md-alert.md-alert-caution{border-left-color:#cf222e}
```

We revise `github.css` so that the background of these blocks.

```css
.md-alert.md-alert-note {background: rgba(9, 105, 218, 0.06);color: #0969da;}
.md-alert.md-alert-important {background: rgba(130, 80, 223, 0.06);color: #8250df;}
.md-alert.md-alert-warning {background: rgba(154, 103, 0, 0.06);color: #9a6700;}
.md-alert.md-alert-tip {background: rgba(31, 136, 61, 0.06);color: #1f883d;}
.md-alert.md-alert-caution {background: rgba(207, 34, 46, 0.06);color: #cf222e;}
```
