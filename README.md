# Daniel Mercer — book landing page

Static site, no build step, no framework, no dependencies.

## Deploy to Vercel
1. Create a new GitHub repo (e.g. `daniel-mercer-books`) and push these files as-is
   (index.html, style.css, images/ folder).
2. Go to vercel.com -> Add New Project -> import that repo.
3. Framework preset: "Other" (it's plain static HTML, no build command needed).
4. Deploy. Vercel will give you a `.vercel.app` URL immediately.
5. In the Vercel project -> Settings -> Domains, add danielmercerbooks.com
   (or whichever domain you register), then point its DNS at Vercel
   per the instructions Vercel shows you.

## Anchors for Pinterest deep-linking
Each book section has an id you can link straight to from a pin:
- yourdomain.com/#why-self-help-fails
- yourdomain.com/#manifestation-from-awareness
- yourdomain.com/#why-cant-i-manifest
- yourdomain.com/#living-from-awareness

## Updating a book's link or cover later
Everything lives in index.html as plain HTML -- find the <section class="book" id="...">
block for that title, swap the href or image file, redeploy (Vercel redeploys
automatically on every push to the connected branch).
