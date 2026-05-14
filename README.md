# Marine Estate Connected Communities — muiz.co.za

Website for the Marine Estate Connected Communities (CCME) in Muizenberg, Cape Town.

## Stack

- **[Hugo](https://gohugo.io/)** — static site generator
- **[Netlify](https://netlify.com/)** — hosting (free tier)
- **[DecapCMS](https://decapcms.org/)** — browser-based content editor for non-technical admins
- **GitHub** — content and code storage

## Content Structure

```
content/
├── _index.md          # Homepage content
├── groups/            # One .md file per WhatsApp group
├── events/            # Events and announcements
└── resources/         # Community resources (can span multiple groups)
```

## For Group Admins

To update your group's content, events, or resources:

1. Go to [muiz.co.za/admin](https://muiz.co.za/admin)
2. Log in with your Netlify Identity account
3. Edit your group's page, add events, or add resources
4. Click **Publish** — changes go live within ~1 minute

## Local Development

```bash
# Install Hugo (macOS)
brew install hugo

# Clone the repo
git clone https://github.com/Greenpill-Cape-Town/muiz.co.za
cd muiz.co.za

# Run locally
hugo server -D

# Open http://localhost:1313
```

## Deployment

Connected to Netlify. Every push to `main` triggers a new build and deploy automatically.

## Setup Checklist

- [ ] Replace `whatsapp_community_link` in `config.toml` with real community link
- [ ] Add real WhatsApp invite links to each group's `.md` file
- [ ] Add QR code images to `static/images/` and reference in group front matter
- [ ] Enable Netlify Identity in Netlify dashboard
- [ ] Invite group admins via Netlify Identity
- [ ] Point muiz.co.za DNS to Netlify

---

Supported by [Greenpill Cape Town](https://greenpill.network) · Built with 🌊 in Muizenberg
