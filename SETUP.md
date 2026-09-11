# FlipBook — Setup

## Prerequisites (system-level, not installed via npm)
- Node.js (v18+ recommended)
- **ffmpeg** — required by the backend for video trimming/frame extraction
  - Mac: `brew install ffmpeg`
  - Windows: `choco install ffmpeg` (or download from ffmpeg.org and add to PATH)
  - Linux: `apt install ffmpeg`
  - Verify install: `ffmpeg -version`

## Install project dependencies

```bash
cd client
npm install

cd ../server
npm install
```

All npm dependencies are tracked in each folder's `package.json` — no manual list needed, `npm install` reads it automatically.

## Run

```bash
# terminal 1
cd server
npm run dev   # (add this script once nodemon is configured)

# terminal 2
cd client
npm run dev
```