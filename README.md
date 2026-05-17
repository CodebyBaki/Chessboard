# Chess Social React App

A React-based chess web app with:

- Play vs local player
- Play vs computer (basic AI: random legal responses)
- Account name + local save/load progress
- Social invite links for Twitter/X, Facebook, and WhatsApp
- GitHub Pages CI/CD deployment workflow

## Run

Open `index.html` in a modern browser with internet access (React is loaded from ESM CDN).

## Play modes

- **2 Players (Local)**: both players on same device.
- **Play vs Computer**: computer controls Black and responds automatically.

## Accounts and progress

- Enter a username in **Account & Progress**.
- Click **Save** to store current game state in browser localStorage.
- Click **Load** to continue from saved progress.

## Invite friends

Use built-in links to share the page:

- Twitter/X invite
- Facebook share
- WhatsApp invite

> Note: this is link-based sharing. Real-time online multiplayer (chess.com-style live matches) requires backend services (rooms, sockets, auth, persistence).

## Deployment

GitHub Actions workflow: `.github/workflows/pages.yml`

- Deploys to GitHub Pages on `main` updates.
- Includes a lightweight validation step.
