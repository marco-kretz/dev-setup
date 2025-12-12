# Personal PHP Web-Development Setup

These are my minimum requirements for an elegant and easy-to-use development environment with **VS Code**.

## Machine

-   **OS**: [`Omarchy`](https://omarchy.org/) - _Beautiful, Modern & Opinionated Linux by DHH_
-   **Hardware**:
    -   **Mainboard**: [`ASUS ROG STRIX B550-F GAMING WIFI II`](https://rog.asus.com/de/motherboards/rog-strix/rog-strix-b550-f-gaming-wifi-ii-model/)
    -   **CPU**: [`AMD Ryzen 7 5800X3D`](https://www.amd.com/de/products/processors/desktops/ryzen/5000-series/amd-ryzen-7-5800x3d.html)
    -   **GPU**: [`Hellhound AMD Radeon™ RX 7900 XT`](https://www.powercolor.com/product-detail120.htm)
-   **Screens**:
    -   1x [`DELL G3223Q (32", 4K)`](https://www.dell.com/de-de/shop/dell-32-4k-uhd-gamingmonitor-g3223q/apd/210-bdxs/monitore-und-monitorzubeh%C3%B6r)
    -   1x Samsung S27AG524NU (27", 1440p)

## Editor

For the longest time, I used **Visual Studio Code** as my main editor. It is fine.
Throughout 2025, I experimented with various ways to integrate AI perfectly into my workflow:

-   VS Code + Copilot / Claude Code / OpenCode
-   Cursor
-   Zed
-   etc.

I'm not 100% satisfied yet, but right now **Cursor** offers the best overall experience. You are somewhat locked into the editor, which I dislike, so I am still exploring alternatives. **Zed** is very promising—super fast and "zen"—but not quite ready for my daily needs. Maybe I can tweak it to perfection over the holidays. :)

**CLI Agents vs. Integration**
CLI agent tools are great but often lack tight editor integration. While plugins exist (e.g., for Claude and OpenCode) to show diffs, I found them unreliable—often breaking after terminal restarts. **Zed** has the best concept here with their _Agent Client Protocol_, where the chat lives in the sidebar as if native. It's a cool idea, but it wasn't reliable for me yet.

Full-blown IDEs like PHPStorm are not my cup of tea. I need my editor to be fast.

### Verdict

I use **Cursor** as my main editor. It offers superior edit predictions and better project understanding than Copilot.

When I want to conserve Cursor usage or face a heavy, non-code-specific problem, I fallback to usage-based CLI agents:

-   [`OpenCode`](https://opencode.ai/) - Using [their API](https://opencode.ai/zen) and/or [OpenRouter](https://openrouter.ai/)
-   [`Claude Code`](https://github.com/anthropics/claude-code) - Using [OpenRouter](https://openrouter.ai/) API via [y-router](https://github.com/luohy15/y-router) (running locally)
-   [`Mistral Vibe`](https://github.com/mistralai/mistral-vibe) - Currently playing around with it _\*EU copium\*_

## VS Code / Cursor Extensions

### General

-   [`EditorConfig for VS Code`](https://open-vsx.org/extension/EditorConfig/EditorConfig) - _EditorConfig Support_
-   [`Prettier - Code formatter`](https://open-vsx.org/extension/esbenp/prettier-vscode) - _Opinionated code formatter_
-   [`Error Lens`](https://open-vsx.org/extension/usernamehw/errorlens) - _Improve highlighting of errors and diagnostics_
-   [`GitLens — Git supercharged`](https://open-vsx.org/extension/eamodio/gitlens) - _Supercharge Git within VS Code_

### PHP

-   [`PHP Intelephense`](https://open-vsx.org/extension/bmewburn/vscode-intelephense-client) - _PHP code intelligence_
-   [`PHP Debug`](https://open-vsx.org/extension/felixfbecker/php-debug) - _Debug support with XDebug_
-   [`php cs fixer`](https://open-vsx.org/extension/junstyle/php-cs-fixer) - _PHP formatter and beautifier_
-   [`Twig Language 2`](https://open-vsx.org/extension/mblode/twig-language-2) - _Snippets, syntax highlighting, and formatting for Twig_

### JavaScript / ECMAScript

-   [`ESLint`](https://open-vsx.org/extension/dbaeumer/vscode-eslint) - _Integrates ESLint into VS Code_
-   [`Vue (Official)`](https://open-vsx.org/extension/Vue/volar) - _Language Support for Vue_

## Appearance

### Themes

-   [`Monokai Pro (Filter Ristretto)`](https://open-vsx.org/extension/monokai/theme-monokai-pro-vscode) - _Icon Theme_
-   [`Monokai Pro (Filter Ristretto)`](https://open-vsx.org/extension/monokai/theme-monokai-pro-vscode) - _Color Scheme_

_I bought the license. It's 100% worth it :)_

### Font

I always use [Nerd Fonts](https://www.nerdfonts.com/) variants since I use them in the terminal as well.

-   [`JetBrainsMono`](https://www.jetbrains.com/de-de/lp/mono/) - _A typeface for developers_

### Misc

-   [`Sync Settings`](https://open-vsx.org/extension/zokugun/sync-settings) - _Easily synchronize your settings_
-   [`YAML`](https://open-vsx.org/extension/redhat/vscode-yaml) - _YAML Language Support by Red Hat_
-   [`Rainbow CSV`](https://open-vsx.org/extension/mechatroner/rainbow-csv) - _Highlight CSV/TSV files and run SQL-like queries_
-   [`Thunder Client`](https://open-vsx.org/extension/rangav/vscode-thunder-client) - _Lightweight Rest API Client_

## Screenshot

![Screenshot](https://github.com/marco-kretz/dev-setup/blob/master/screenshot.png)
