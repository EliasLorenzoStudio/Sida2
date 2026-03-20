# Sida2

A responsive test site — works on desktop (web) and mobile.

## Development in Visual Studio Code

### Prerequisites

- [Visual Studio Code](https://code.visualstudio.com/)
- [Node.js](https://nodejs.org/) (for the `npm start` script)

### Recommended VS Code extensions

Open the project in VS Code — you will be prompted to install the recommended extensions from `.vscode/extensions.json`:

| Extension | Purpose |
|---|---|
| **Live Server** (`ritwickdey.LiveServer`) | Auto-refresh dev server |
| **Edge DevTools** (`ms-edgedevtools.vscode-edge-devtools`) | In-editor browser & mobile DevTools |
| **Prettier** (`esbenp.prettier-vscode`) | Code formatting |
| **ESLint** (`dbaeumer.vscode-eslint`) | JavaScript linting |

### Run the dev server

**Option A – npm script**

```bash
npm start
```

This launches `live-server` on <http://localhost:5500>.

**Option B – Live Server extension**

Right-click `index.html` → **Open with Live Server**.

### Test for web and mobile

#### Desktop browser
Use the **Run & Debug** panel (`Ctrl+Shift+D` / `⌘⇧D`) and select:

- **Open in Chrome (Desktop)** — standard desktop viewport
- **Open in Edge (Desktop)** — Microsoft Edge

#### Mobile browser emulation
Select **Open in Chrome (Mobile – iPhone 12)** from the Run & Debug panel.  
This launches Chrome with a 390 × 844 px window and a mobile user-agent string.

For full device emulation (touch events, pixel ratio, etc.) open Chrome DevTools
(`F12`) → **Toggle device toolbar** (`Ctrl+Shift+M` / `⌘⇧M`) after the page loads.

## Project structure

```
Sida2/
├── index.html        # Main page
├── styles.css        # Responsive styles (desktop + mobile breakpoints)
├── app.js            # Navigation toggle & form handling
├── package.json      # npm start script
└── .vscode/
    ├── extensions.json   # Recommended extensions
    ├── settings.json     # Editor & Live Server settings
    ├── launch.json       # Debug launch configurations
    └── tasks.json        # Background server task
```
