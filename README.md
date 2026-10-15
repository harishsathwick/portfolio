# Harish Sathwick — Portfolio

Static site: plain HTML/CSS/JS, no build step. Content lives in the data arrays near the top of the `<script>` in `index.html` (`SKILLS`, `PROJECTS`, `EXPERIENCE`, `EDUCATION`, `CERTS`, `CONTACT_LINKS`).

## Deploy (pick one)
- **Netlify:** drag this folder onto https://app.netlify.com/drop
- **Vercel:** `npx vercel --prod` inside this folder
- **GitHub Pages:** push this folder to a repo, then Settings → Pages → deploy from `main` / root

## After deploying
1. In `index.html`, change `og:image` and `twitter:image` from `assets/og-image.jpg` to the full URL, e.g. `https://yourname.netlify.app/assets/og-image.jpg` (link previews on LinkedIn/WhatsApp need an absolute URL).
2. Optionally add `<link rel="canonical" href="https://your-domain/">` in `<head>`.

## Updating content
- **Resume:** replace `assets/Harish_Sathwick_Resume.pdf` (keep the filename).
- **Projects:** add a `github` and/or `demo` URL to a project in `PROJECTS`. Buttons appear only when a URL is set.
- **Contact form:** posts to FormSubmit, which forwards each message to your Gmail. See the section below. To use a different provider, change `FORM_ENDPOINT` in the `CONTACT FORM` block of `index.html`.

## Contact form: make sure messages reach you (do this once)
The form delivers to harishjakkamsetty76@gmail.com. Pick ONE of these:

**Option A (recommended, most reliable): Web3Forms, about 1 minute**
1. Go to https://web3forms.com, enter harishjakkamsetty76@gmail.com and get your free **access key** by email.
2. In `index.html`, find `web3formsKey: ''` (search for `CONTACT FORM`) and paste the key between the quotes.
3. Re-deploy. Done: no activation click is needed.

**Option B (default, no key): FormSubmit**
1. Deploy the site (it does not work reliably from a local file or a preview).
2. Send yourself one test message through the live form.
3. FormSubmit emails you an **activation link**. Click it once (check Spam/Promotions).

If sending ever fails, the visitor sees the exact reason plus a link to send the same message from their own email app, so no enquiry is lost.

## Where to edit the content
Everything lives in the data lists near the top of the `<script>`: `SERVICES`, `PROCESS`, `SKILLS`, `PROJECTS`, `EXPERIENCE`, `EDUCATION`, `CERTS`. The hero and About text are plain HTML near the top of `<body>`.
