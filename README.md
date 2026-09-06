# StormOps Field

Public field/crew client for StormOps, hosted on GitHub Pages.

This is a **cloud-only** client: it talks directly to Firebase (Auth + Realtime
Database). It contains no server code, no passwords, and no customer names or
addresses. Crews sign in with their Firebase field account and see only
sanitised incident data (network details, suburb, coordinates) plus the scoping
they submit.

## Deploy
GitHub Pages serves `index.html` from the default branch. No build step.

## Notes
- The Firebase `apiKey` in `index.html` is public by design; access is enforced
  by Firebase Authentication and Realtime Database security rules.
- The full ops/admin side runs separately and privately; it is not part of this
  repository.
