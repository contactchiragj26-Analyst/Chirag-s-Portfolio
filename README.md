# Chirag Jain | Data Analyst Portfolio

A responsive, static portfolio website for showcasing data analytics skills, selected projects, and contact details.

## Features

- Professional data analyst portfolio layout
- Responsive desktop and mobile design
- About, toolkit, selected work, and contact sections
- Email contact link
- WhatsApp contact link generated from the phone number
- LinkedIn and GitHub profile links
- Built-in **Edit profile** panel
- Profile details stored in browser `localStorage`
- No backend or build process required

## Project Files

```text
.
├── index.html   # Portfolio content, contact links, and editor logic
├── style.css    # Responsive layout, colors, typography, and animations
└── README.md    # Project documentation
```

## Run Locally

Because this is a static website, it can be opened directly:

1. Open `index.html` in a browser.
2. Click **Edit profile** in the top navigation.
3. Enter your name, email address, phone number, and LinkedIn URL.
4. Click **Save details**.

You can also use the VS Code Live Server extension for a local preview.

## Editing Contact Details Permanently

The editor saves changes in the current browser only. To update the default values for everyone who visits the deployed website, edit the `defaults` object near the bottom of `index.html`:

```js
const defaults = {
    name: 'Chirag Jain',
    email: 'your-email@example.com',
    phone: '+91 99999 99999',
    whatsapp: '919999999999',
    linkedin: 'https://www.linkedin.com/in/your-linkedin-username'
};
```

Use the WhatsApp number in international format without `+`, spaces, or brackets. For example:

```text
+91 98765 43210  ->  919876543210
```

You can also update the GitHub URL, project descriptions, skills, and headings directly in `index.html`.

## Deploy with GitHub Pages

1. Create or open a GitHub repository.
2. Upload `index.html`, `style.css`, and `README.md` to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select the `main` branch and the `/ (root)` folder.
6. Click **Save**.

GitHub will provide a public URL similar to:

```text
https://your-github-username.github.io/repository-name/
```

### Important

This project currently sits inside a nested `contactchiragj26-Analyst-main` folder. When uploading to GitHub Pages, upload the files from the inner project folder so that `index.html` is at the repository root.

## Customization

- Replace the GitHub profile URL in `index.html`.
- Replace the LinkedIn URL and contact details.
- Update the profile image URL if needed.
- Edit project cards and tool labels to reflect your real work.
- Change colors and spacing through the CSS variables at the top of `style.css`.

## Technologies

- HTML5
- CSS3
- Vanilla JavaScript
- Google Fonts
- Browser `localStorage`

## License

This portfolio is intended for personal use and customization.
