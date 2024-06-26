---
{"dg-publish":true,"permalink":"/obsidian/obsidian/general-css-snippets/","noteIcon":""}
---

>[!tip] Below are the snippets that I am using right now:
>- Hides minimize/maximize and close buttons.
>- Frees up the space reserved for the minimize/maximize and close buttons.
>- Increases the radius of the callout.
>- Changes code and code block backgrounds and borders.
>- Changes sidebar toggle button background.
>- Changes file explorer background color.
>- Changes the tab bar and top bar background color.
>- Hides left bar.
>- Justifies text to on both sides.
>- Disables text wrapping on code blocks.
>- Changes font properties for bold, italic and highlight.
>- Changes font strike-through to underline in Catppuccin yellow.

```css
/* Hide title bar minimize, maximize and close buttons*/
.mod-linux .titlebar-button-container, .mod-windows .titlebar-button-container {
  display: none;
}

/* Free up the space that was reserved for he minimize, maximize and close buttons*/
.is-hidden-frameless:not(.is-fullscreen) .workspace-tabs.mod-top-right-space .workspace-tab-header-container {
  padding-right: 10px;
}

/* Hide bottom status bar */
/* .status-bar {
  display: none !important;
}*/

/* Callout border radius */
.callout {
  border-radius: 10px;
}

/* Code Block background colour and border */
.markdown-rendered pre {
  border-radius: 10px !important;
  background-color: #2b2c3e !important;
  border: 1px solid #89b4fa;
}

/* Code background colour, font colour, border radius and padding*/
.markdown-rendered code {
  background-color: #484b69;
  padding: 0.15em 0.25em;
  color: #cdd6f4;
  border-radius: 7px;
}

/* Sidebar Toggle button background */
.sidebar-toggle-button {
  background: #1e1e2e !important;
}

/* File explorer background colour */
.workspace-tabs .workspace-leaf {
  background: #1e1e2e !important;
}

/* Tab bar and top bar background colour */
.workspace-tab-header-container {
  background-color: #1e1e2e;
}

/* Left bar hidden - press alt+b to reveal it */
body > div.app-container > div.horizontal-main-container > div > div.workspace-ribbon.side-dock-ribbon.mod-left.is-collapsed {
  display: none;
}

/*Text justify */
/* reading mode */
.markdown-preview-view p {
	text-align: justify;
	text-justify: inter-word;	
}

/* Text Justify */
/* source view and live preview */
.markdown-source-view.mod-cm6 .cm-line {
	text-align: justify;
	text-justify: inter-word;	
}

/* Center Mermaid Content */
.mermaid {
  display: flex !important;
  justify-content: center;
}

/* Disable wrapping on code blocks in preview mode */
.markdown-rendered :not(.print) code,
body :not(.print) code {
  word-break: normal;
  word-wrap: break-word;
  white-space: pre;
}

/* Font Properties for bold, italic and highlight */
/* Highlight properties */
.markdown-rendered mark, .cm-s-obsidian span.cm-formatting-highlight, .cm-s-obsidian span.cm-highlight {
  background-color: transparent !important;
  font-weight: 700 !important;
  color: #fab387 !important;
}

/* bold properties */
strong, .cm-strong {
  color: #cdd6f4 !important;
  font-weight: 700 !important;
}

/* italic properties */
em, .cm-em {
  color: #cdd6f4 !important;
  font-style: italic;
}

/* Strike through properties ~~strike~~ */
del, .cm-strikethrough {
  text-decoration: underline;
  font-weight: 700;
  color: #f9e2af;
}
```
