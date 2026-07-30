# أنقذني في آخر لحظة — Last-Minute Exam Rescue

An AI-powered emergency exam study planner supporting Arabic and English. Students enter their subject, remaining time, and level; the app generates a personalized study plan, smart summary, predicted questions, and Pomodoro timer — all powered by Google Gemini.

## Stack

- **Frontend:** React 19 + TypeScript + Vite + Tailwind CSS v4
- **Backend:** Express (TypeScript) served via `tsx` in dev, compiled with `esbuild` for prod
- **AI:** Google Gemini 2.5 Flash (`@google/genai`)
- **Auth/Data:** Firebase
- **Charts:** Recharts
- **Animation:** Motion (Framer Motion)

## Running the app

```bash
npm run dev
```

The Express server starts on port **5000** and serves the Vite dev middleware in development. The workflow `Start application` runs this automatically.

## Required secrets

| Secret | Description |
|---|---|
| `GEMINI_API_KEY` | Google Gemini API key — get one free at https://aistudio.google.com/apikey |

## Firebase

Firebase is integrated but requires configuration. Set the Firebase project credentials (API key, auth domain, project ID, etc.) as secrets or environment variables if you want auth and data persistence to work.

## Build for production

```bash
npm run build   # builds frontend to dist/ and server to dist/server.cjs
npm start       # runs the compiled server
```

## User preferences

- Keep the existing project structure and Arabic/English bilingual support.
