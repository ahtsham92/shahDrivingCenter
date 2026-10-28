# Shah Driving Center website

Static site (HTML, CSS, JavaScript). No build step, no dependencies.

## Structure
- index.html: page markup
- css/style.css: styles (light and dark themes)
- js/main.js: data and behaviour

## Customise
Open js/main.js. The block marked "EDIT THESE" holds branches (address, phone, WhatsApp number in international format without +), courses and prices, instructors and reviews.
Also edit in index.html: licence fee table, FAQ answers, quiz questions, offer popup text, social links and the footer.

## Run locally
Open index.html in a browser, or run: python3 -m http.server 8000

## Deploy (upload the folder contents)
- Netlify: drag and drop the folder at app.netlify.com/drop
- Vercel: run "vercel" inside the folder, framework "Other"
- GitHub Pages: push to a repo, Settings > Pages > deploy from branch
- Cloudflare Pages: connect the repo, build command empty, output directory /
- Any shared hosting or VPS (cPanel, Nginx, Apache): upload the files to the web root (public_html)

## Notes
Forms have no backend: they open WhatsApp with the details pre-filled. To store submissions, connect the forms to a service such as Formspree or your own API.
