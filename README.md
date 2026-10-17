# PRIMELA — Admin & Creative Support Portfolio

A responsive portfolio website for **PRIMELA**, based on the supplied branding guide.

## Brand direction
- **Plum:** `#301934`
- **Gold:** `#E5C158`
- Warm cream backgrounds and editorial typography
- The guide names **Glacial Indifference**. This starter uses DM Sans as a convenient web font and a local fallback stack; replace it with a licensed/hosted Glacial Indifference font if you have the font files and rights to use them.

## Included
- About / professional bio
- Portfolio with category filters
- Services offered
- Certificates section with image placeholders
- Two testimonial placeholders
- Contact details and a contact form that opens the visitor's email app
- Responsive mobile navigation
- Plain HTML, CSS, and JavaScript — no build tools required

## Run locally
Open `index.html` in a browser. For a local server, you can use the VS Code Live Server extension.

## Publish on GitHub Pages
1. Create a new GitHub repository, for example `primela-portfolio`.
2. Upload `index.html`, `style.css`, `script.js`, and this `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. GitHub will provide your public website URL after deployment finishes.

## Personalize before publishing
1. In `index.html`, replace `your.email@example.com` with your real email address.
2. Update the social profile link in the Contact section.
3. Replace the photo, workspace, project, and certificate placeholder blocks with your own images.
4. Replace both testimonial placeholders with genuine, approved testimonials. Do not publish invented endorsements.
5. Add real dates, tools, project goals, and outcomes to your work samples.
6. Review the bio and services to ensure they accurately represent your experience and current offerings.

## Add your own images
Create folders such as `assets/images/` and `assets/certificates/`, then add image files. Replace a placeholder `<div>` with an image element, for example:

```html
<img
  class="portrait"
  src="assets/images/princess-portrait.jpg"
  alt="Portrait of Princess De Casa"
>
```

For project thumbnails, keep the existing `.project-image` wrapper and put the `<img>` inside it. Add this CSS if you want images to crop consistently:

```css
.project-image img,
.portrait {
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}
```

## Contact form note
This static website does not store or send messages itself. The form uses a `mailto:` link to prepare an email in the visitor's email app. If you want submissions without an email app, connect a form backend/service and update the JavaScript accordingly.
