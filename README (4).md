# Flat Duty Roster – Winter

A single-page duty roster site. Everything (HTML, CSS, JS and the background images) lives in `index.html`, so there is no build step.

## Deploy on GitHub Pages

1. Create a new repository on GitHub and upload all files from this folder (including the hidden `.nojekyll`).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose **main** and **/ (root)**, then **Save**.
4. After about a minute the site is live at `https://<your-username>.github.io/<repo-name>/`.

## Firebase setup

`index.html` still contains the placeholder Firebase config (`PASTE_API_KEY`, etc.). Paste your real values into `firebaseConfig` in `index.html`.

Firebase web API keys are meant to be public, so it is safe to commit them. Access is controlled by your Firestore security rules.

Then, in the Firebase console, go to **Authentication → Settings → Authorized domains** and add `<your-username>.github.io`. Otherwise email/password sign-in will be blocked on the deployed site.
