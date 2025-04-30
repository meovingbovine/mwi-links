# Meowing Bovine Useful Link List

This repository contains the source code for the Meowing Bovine Useful Link List, a simple static site built with [Hugo](https://gohugo.io/). It serves as a curated collection of useful links related to MWI *[Define MWI if possible, e.g., Milky Way Idle]*, covering categories like Combat, Enhancing, Skilling, Leaderboards, Market tools, and more.

**Live Site:** [https://meowingbovine.github.io/mwi-links/](https://meowingbovine.github.io/mwi-links/)

## ✨ Features

*   **Fast & Simple:** Built with Hugo, known for its speed and simplicity.
*   **Minimalist Design:** Uses the clean and responsive [Risotto](https://github.com/joeroe/risotto) theme.
*   **No JavaScript:** Pure HTML and CSS for a lightweight experience (thanks to the Risotto theme).
*   **Tool Management:** Uses [Mise](https://mise.jdx.dev/) to manage the correct Hugo version.
*   **Automated Deployment:** Deployed automatically to GitHub Pages via GitHub Actions.

## 🛠️ Development

### Prerequisites

*   [Git](https://git-scm.com/)
*   [Mise](https://mise.jdx.dev/) (for managing the Hugo version specified in `mise.toml`)

### Getting Started

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/meowingbovine/mwi-links.git 
    cd mwi-links
    ```

2.  **Install Hugo using Mise:**
    Mise should automatically prompt you to install the required Hugo version when you `cd` into the directory (if you have the shell integration set up) or when you first run a `mise` command. If not, you can install it manually:
    ```bash
    mise install
    ```
    *Note: The `mise.toml` specifies `hugo = "latest"`, so Mise will install the latest available version.*

3.  **Run the Hugo development server:**
    ```bash
    mise exec hugo -- server
    # Or, if mise is integrated into your shell:
    # hugo server
    ```
    This will start a local server, typically at `http://localhost:1313/`. The site will automatically reload when you make changes to the content or configuration.

### Adding Content

*   The main list of links is managed in the `content/_index.md` file.
*   Use standard Markdown syntax (headings for categories, bullet points for links) to add or modify content.

## 🏗️ Building

To build the static site files for deployment:

```bash
mise exec hugo
# Or, if mise is integrated into your shell:
# hugo