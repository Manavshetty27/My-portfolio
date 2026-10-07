# Deployment

This is a static HTML/CSS/JavaScript site. It has no build step and can be published directly with GitHub Pages.

## Before publishing

- The contact email and phone open the visitor's default mail or calling app. The contact form opens a prefilled email draft; it does not send mail by itself. For in-page submissions, connect a form service or your own server endpoint.
- Replace the X and Dev.to URLs in the footer with the owner's actual profiles if those links are used.
- Review the portfolio's biography, skills, project descriptions, education, certificate details, dates, and metrics for accuracy.
- Keep `index.html`, `style.css`, `background.jpeg`, the profile photo, project thumbnails, resume PDF, and highlight MP4 in the published site. Preserve the filenames and capitalization used in the HTML.
- The chat currently uses local JavaScript responses. For a real AI assistant, call a server-side endpoint; never put an OpenAI or other provider secret in browser JavaScript.
- Test the local MP4 and resume from the published URL, not only from a `file://` page.

## Publish with GitHub Pages

1. Create a GitHub repository and add the site files and assets to the repository root.
2. Push the files to the `main` branch.
3. Open the repository's **Settings > Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, select `main` and `/(root)`, then save.
5. Wait for the Pages deployment to finish. The published address appears in the Pages settings. A user or organization repository named `OWNER.github.io` uses `https://OWNER.github.io/`; other repositories use `https://OWNER.github.io/REPOSITORY/`.
6. Open the published address on a phone and desktop. Check navigation, media and image loading, the chat responses, the contact email draft, and the resume download. GitHub Pages serves relative asset paths from either repository URL form.

No build command or package installation is needed. Add a custom domain through the same Pages settings only after the default Pages URL works.