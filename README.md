# HTML-IDE

A self-contained, single-file HTML IDE that runs entirely in the browser — no server, no install, no build step. 
Built for teaching (KS2 / KS3 computing style exercises).

Inspired by https://github.com/milesberry/pyde and created using copilot.

## Features

- **Syntax highlighting** - CodeMirror 5. Copying a selection also writes a colour-highlighted text/html version to the clipboard alongside the plain text, matching the current theme, so pasting into Word/OneNote/Google Docs keeps the syntax colours instead of landing as flat text.

- **Undo / Redo** - undo/redo last edits
- **Add page / Remove page** - starts with add and remove pages

- **NavBar** - separate tab for the nav bar which is injected into each page. <div id="navbar-slot"></div>
Pages are stored as page1, page2, page3 etc. this is also used to in linking.
Tabs in the edior pick up the text used in the navbar.

- **styles.css** - separate tab for the CSS styles which are applied when rendering each page

- **script.js** - separate tab for scripts which is referenced in the normal way 
(add <script type="text/javascript" src="script.js"></script> to the page header)

- **Reset Page** - resets the current page back to a default state (a heading and some text)
- **Reset All Pages** - resets the entire website back to a very simple 5 page template with basic css and no js

- **Live Preview On/Off** - the preview pane can automatically update, but this adds a additional processing overhead (default = Off)
- **Update preview** - updates the current preview

- **Update URL & Copy** - the whole site is LZ-compressed into the page's URL hash, so a link fully reproduces it with no backend

- **A+ / A-** - quickly increase / decrease displayed font size in editor (bigger is good for projecting) 
- **Light/Dark mode** - switch the code editor between light mode (good for projecting) and dark mode (good for coding)

## Running it locally

There's nothing to install. Open "index.html" directly in a browser, or serve the folder with any static file server if you prefer.

## License

[MIT](LICENSE) — use it, modify it, teach with it, no strings attached.
