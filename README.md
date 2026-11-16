# PRAVEENRAJ E — Portfolio

React + Vite + Tailwind CSS + Framer Motion + Lucide + tsParticles. All content comes from your resume.

## Run locally
```bash
npm install
npm run dev
```
Build: `npm run build` (output in `dist/`).

## Where to edit
- **Everything personal** (name, summary, skills, experience, projects, education, certifications, links): `src/data/site.js`
- **Resume PDF:** replace `public/resume.pdf`
- **Photo:** replace `public/images/photo.jpeg`
- **Add a project:** add an object to `projects` in `src/data/site.js` (`categories` can be Web, IoT or Embedded; set `image: '/images/x.png'` for a screenshot and `demo: 'https://...'` to show a Live Demo button). Per-project GitHub links currently point to your GitHub profile; change them to the repo URLs.
- **Social links:** `socialLinks` in `src/data/site.js`. Instagram was not in the resume, so it is not shown. Add an `instagram` link and a `<SocialIcon name="Instagram" />` if you want it.
- **Theme colors:** CSS variables at the top of `src/index.css` (`:root` = light, `.dark` = dark).
- **Contact form:** it validates input, then (because no email service is connected) opens the visitor's email app. To send for real, edit `src/services/sendMessage.js` (EmailJS, Formspree or your API) and set `EMAIL_SERVICE_CONFIGURED = true`.

## Deploy
Push to GitHub, import the repo in Vercel or Netlify. Build command `npm run build`, output directory `dist`.
