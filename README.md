
# Gripetime — Full Stack (E)
React + Firebase Hosting + Cloud Functions + Firestore + Clean URLs + CI

## Quick Start
```bash
npm i -g firebase-tools
# Web
cd web && npm i && cp .env.example .env  # paste Firebase web config
npm run dev
# In another shell: Firebase emulators
cd ..
firebase emulators:start
```

## Deploy (via GitHub Actions)
1. Update `.firebaserc` project id.
2. Add repo secrets (Settings → Secrets and variables → Actions):
   - FIREBASE_SERVICE_ACCOUNT = JSON for a service account (Editor)
   - VITE_API_KEY, VITE_AUTH_DOMAIN, VITE_PROJECT_ID, VITE_STORAGE_BUCKET, VITE_MESSAGING_SENDER_ID, VITE_APP_ID
3. Push to `main`.

## Admin
Create a document in `admins/{uid}` for your UID (from Firebase Auth → Users) to grant admin rights.
