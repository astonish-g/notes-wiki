---
{"dg-publish":true,"permalink":"/obsidian/obsidian/neon-css-snippet/","noteIcon":""}
---

Here below, you can find the **Neon CSS Snippet** that was sent to me by the kind reddit user: ==4I3xBB==. I am still trying the snippets to see which parts of it I can add and adapt to my existing set-up. 

```css
/* Colors Variables */

body {
    --accent-1: #C1FDFF;
    --accent-2: #F3CBFF;
    --accent-3: #00FFFF;
    --accent-4: #FF0000;
    --accent-5: #FF0000;
    --accent-6: #BD93F9;
    --accent-7: #FFBDAD; /* HEADING 4 COLOR ON MINIMAL THEME */

    --accent-1-muted: #ff79c6;
    --accent-2-muted: #8be9fd;
    --accent-3-muted: #50fa7b;
    --accent-4-muted: #ffb86c;
    --accent-5-muted: #ff5555;
    --accent-6-muted: #bd93f9;
}
h1, h2, h3, h4, h5, h6 {
    font-weight: 600;
    overflow: visible;
}

/* Apply Neon Color on Reading View */

h1 {
    text-shadow: 0 0 0.5em var(--accent-1) !important;
}
h2 {
    text-shadow: 0 0 0.5em var(--accent-2);
}
h3 {
    text-shadow: 0 0 0.5em var(--accent-3);
}
h4 {
    text-shadow: 0 0 0.75em var(--accent-4);
}
h5 {
    text-shadow: 0 0 0.75em var(--accent-5);
}
h6 {
    text-shadow: 0 0 0.75em var(--accent-6);
}

/* Apply Neon Color on Source Mode and Live Preview View */

span.cm-header.cm-header-1 {
    text-shadow: 0 0 0.5em var(--accent-1);
}
span.cm-header.cm-header-2 {
    text-shadow: 0 0 0.5em var(--accent-2);
}
span.cm-header.cm-header-3 {
    text-shadow: 0 0 0.5em var(--accent-3);
}
span.cm-header.cm-header-4 {
    text-shadow: 0 0 0.75em var(--accent-4);
}
span.cm-header.cm-header-5 {
    text-shadow: 0 0 0.75em var(--accent-5);
}
span.cm-header.cm-header-6 {
    text-shadow: 0 0 0.75em var(--accent-6);
}

/* Apply Neon on Markdown Elements */
/* HEADERS' HASHTAGS # */

span.cm-formatting.cm-formatting-header.cm-formatting-header-1.cm-header.cm-header-1 {
    color: var(--accent-1);
}
span.cm-formatting.cm-formatting-header.cm-formatting-header-2.cm-header.cm-header-2 {
    color: var(--accent-2);
}
span.cm-formatting.cm-formatting-header.cm-formatting-header-3.cm-header.cm-header-3 {
    color: var(--accent-3);
}
span.cm-formatting.cm-formatting-header.cm-formatting-header-4.cm-header.cm-header-4 {
    color: var(--accent-4);
}
span.cm-formatting.cm-formatting-header.cm-formatting-header-5.cm-header.cm-header-5 {
    color: var(--accent-5);
}
span.cm-formatting.cm-formatting-header.cm-formatting-header-6.cm-header.cm-header-6 {
    color: var(--accent-6);
}

/* OPEN AND CLOSE BRACKETS [] */

span.cm-formatting-link.cm-formatting-link-start {
    color: var(--accent-3);
}
span.cm-formatting-link.cm-formatting-link-end {
    color: var(--accent-3);
}

/* SINGLE QUOTATION MARKS '' */

span.cm-formatting.cm-formatting-code.cm-inline-code{
    color: var(--accent-3);
}

/* [[ WIKILINKS FONT ]] */

span.cm-hmd-internal-link, .internal-link {
    font-weight: 650;
    color: var(--accent-2) !important;
}

.internal-link.is-unresolved {
    font-weight: 650 !important;
    color: var(--accent-2) !important;
}
span.is-unresolved {
    color: var(--accent-2) !important;
    opacity: 1 !important;
}

/* MINIMAL CARDS */

div.block-language-dataview.node-insert-event { /* AVOID LEFT SHADOW ON CARDS WITHOUT CUT IT */
    padding-left: 0.4em; 
}
.dataview.table-view-table .table-view-tbody tr { /* CARDS BORDER AND SHADOW */
    border-color: var(--accent-1);
    border-width: 0.15em;
    box-shadow: 0 0 0.7em var(--accent-1);
}

/* INTERNAL LINKS ON MINIMAL CARDS */

div.block-language-dataview.node-insert-event a.internal-link {
    color: var(--accent-2);
    font-weight: 800;
    margin-top: 1em !important;
}
div.block-language-dataview.node-insert-event .table-view-tbody td {
    text-align: center !important;
    padding-bottom: 0.4em !important;
}

/* ** BOLD FONT ** */

span.cm-hr, span.cm-formatting.cm-formatting-strong.cm-strong {
    color: var(--accent-3);
}

/* INLINE CODE FONT WEIGHT */

span.cm-inline-code, .is-loaded.language-bash, .is-loaded.language-php, .is-loaded.language-python, .is-loaded.language-javascript {
    font-weight: 700;
}

/* CALENDAR EXTENSION */

span.month.svelte-1vwr9dd {
    font-size: 2.50em !important;
    font-weight: 1000 !important;
}
span.year.svelte-1vwr9dd {
    font-size: 2.00em !important;
    font-weight: 1000 !important;
}
div.day.today.svelte-q3wqg9 {
    color: var(--accent-2) !important;
    text-shadow: 0 0 0.5em var(--accent-2) !important;
    font-size: 1.5em !important;
}
.svelte-156w7na {
    color: var(--accent-2) !important;
    filter: drop-shadow(0 0 0.3em var(--accent-2));
}

.reset-button.svelte-1vwr9dd {
    color: var(--accent-2) !important;
    text-shadow: 0 0 1em var(--accent-2) !important;
    font-size: 1em !important;
    text-transform: uppercase !important;
}

svg.svg-icon.lucide-calendar-check {
    color: var(--accent-2) !important;
    filter: drop-shadow(0 0 0.3em var(--accent-2));
}

/* FRONTMATTER DATAVIEW - SOURCE MODE */

.cm-atom.cm-hmd-frontmatter {
    color: var(--accent-2-muted);
    font-weight: bolder;
}

/* FRONTMATTER DATAVIEW - LIVE MODE */

.metadata-properties-title {
    color: var(--accent-2);
    text-shadow: 0 0 1em var(--accent-2);
    font-size: 1.35em;
}
input.metadata-property-key-input {
    color: var(--accent-1) !important;
    text-shadow: 0 0 1em var(--accent-1) !important;
    font-weight: 500;
 }
div.metadata-link-inner.external-link, div.metadata-link-inner.internal-link {
    color: var(--accent-6);
    font-weight: 500;
}
div.multi-select-pill {
    border: 0.2em solid #F3CBFF !important;
    padding-left: 0.8em;
    padding-bottom: 0.3em;
    padding-right: 0.4em;
    margin-bottom: 0.25em;
}
div.multi-select-pill-content {
    font-weight: 500 !important;
    color: var(--accent-1);
    text-shadow: 0 0 1em var(--accent-1);
}
.svg-icon.lucide-x {
    color: var(--accent-2);  
    margin-top: 0.3em;
}

/* INLINE TITLE */

.inline-title {
    text-shadow: 0 0 0.5em var(--accent-1);
}

/* LEFT PANEL TOP */

div.tree-item-inner.nav-folder-title-content {
    color: var(--accent-2);
    text-shadow: 0 0 0.1em var(--accent-2);
    
}

/* RIGHT PANEL TOP */

.view-content.node-insert-event .tree-item-inner-text {
    color: var(--accent-2);
    text-shadow: 0 0 0.1em var(--accent-2);
}

.view-content.node-insert-event 
.svg-icon.lucide-tags,
.svg-icon.lucide-binary,
.svg-icon.lucide-text,
.svg-icon.lucide-list,
.svg-icon.lucide-forward,
.tree-item-flair
{
    color: var(--accent-1);
    filter: drop-shadow(0 0 0.1em var(--accent-1));
}

.clickable-icon.nav-action-button {
    color: var(--accent-2) !important;
    filter: drop-shadow(0 0 0.1em var(--accent-2));
}


/* CUSTOM CSS CLASES FRONTMATTER DATAVIEW - CARDS STYLE COLOR AND BOX SHADOW */

.red-style .dataview.table-view-table .table-view-tbody tr { /* CARDS BORDER AND SHADOW */
    border-color: var(--accent-7);
    border-width: 0.15em;
    box-shadow: 0 0 0.7em var(--accent-4);
}

.purple-style .dataview.table-view-table .table-view-tbody tr { /* CARDS BORDER AND SHADOW */
    border-color: var(--accent-2);
    border-width: 0.15em;
    box-shadow: 0 0 0.7em var(--accent-2);
}
```
