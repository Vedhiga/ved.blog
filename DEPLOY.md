# Deploy checklist (do this part — I can't push to your GitHub/Vercel/Firebase for you)

1. **Firebase config** — open `index.html`, find `firebaseConfig` near the top of the `<script>` block, and paste in the same config object from your current site (Firebase Console → Project Settings → General → Your apps).
2. **Replace files in your repo** — copy `index.html`, `vercel.json`, and `firestore.rules` into the root of `Vedhiga/personal-blog` (your repo currently has `backend/` and `frontend/` folders from the fork — this plan assumes a single static root, so move/delete those or point Vercel's root directory at wherever you place these three files).
3. **Deploy Firestore rules**: `firebase deploy --only firestore:rules` (or paste `firestore.rules` into Firebase Console → Firestore → Rules).
4. **Push to GitHub** — commit and push; Vercel will auto-deploy if it's connected to this repo.
5. **Create your admin login** — Firebase Console → Authentication → Add user (email/password).
6. **Visit `/studio`** on your deployed site and log in.

## Still open (from the plan)
- **Admin URL**: defaulted to `/studio` since none was specified — easy to rename, just change the `isAdminRoute()` check in the script and update `vercel.json` if you add explicit rewrites.
- **About Me content**: I put in placeholder bio/tags/LinkedIn — edit the `#tab-about` section directly, or add an "Edit About" feature in Studio later if you want it CMS-driven too.
- **Backend/frontend folders**: your repo has these from the fork; the plan itself calls for no backend, so decide whether to delete `backend/` or repurpose the repo root.
