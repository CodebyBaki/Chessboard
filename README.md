# Chessboard → Full Chess Game

A browser-based chess game built in plain HTML/CSS/JavaScript.

## Features

- Complete 8×8 board with coordinates
- Piece selection + legal move highlights
- Full turn-based play for White and Black
- Rule enforcement:
  - Check detection
  - Checkmate detection
  - Stalemate detection
  - Castling (both sides)
  - En passant
  - Pawn promotion (auto-promotes to queen)
- New Game reset button

## Run locally

Open `index.html` in any modern browser.

## GitHub Pages hosting

This repo now includes a GitHub Actions workflow that deploys the app to GitHub Pages whenever `main` is updated.

### One-time setup

1. Push this repository to GitHub.
2. In GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Source: GitHub Actions**.
4. Push to `main` (or trigger the workflow manually from the **Actions** tab).

After deployment, your site will be available at:

- `https://<your-username>.github.io/<repo-name>/`

## CI/CD pipeline

Workflow file: `.github/workflows/pages.yml`

- `validate` job confirms the app entrypoint exists and includes the board container.
- `deploy` job publishes the repository contents to GitHub Pages.

## VS Code direct changes flow

You can make direct edits from VS Code and have them deployed automatically:

1. Clone the repository in VS Code.
2. Edit files (`index.html`, `README.md`, etc.).
3. Commit and push from VS Code Source Control.
4. GitHub Actions runs automatically and redeploys the site.

Recommended VS Code extensions are listed in `.vscode/extensions.json`.
