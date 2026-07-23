# JIF Cookbook: Setup & Deployment Guide

This site is built with Docsify and hosted on GitHub Pages. Here's how to set it up and deploy.

## Local Setup (For Development)

### Prerequisites
- GitHub account
- Git installed locally
- Node.js (optional, for running a local server)

### Steps

1. **Clone the repository**
```bash
git clone https://github.com/ANyashina-LLC/jif-cookbook.git
cd jif-cookbook
```

2. **Serve locally (optional, for testing)**
```bash
# Install docsify CLI
npm install -g docsify-cli

# Run local server
docsify serve docs

# Visit http://localhost:3000 in your browser
```

3. **Edit files**
- All content is in the `docs/` folder as markdown (.md) files
- Edit any markdown file using your preferred text editor
- Changes appear immediately in the browser (if using docsify serve)

4. **Push to GitHub**
```bash
git add .
git commit -m "Update: describe your changes"
git push origin main
```

The site will automatically rebuild and deploy to `https://jif-cookbook.github.io` within 1-2 minutes.

---

## Directory Structure

```
jif-cookbook/
├── docs/                          # All content (source of truth)
│   ├── index.html                 # Docsify configuration
│   ├── home.md                    # Landing page
│   ├── _sidebar.md                # Navigation sidebar
│   ├── _coverpage.md              # Cover page
│   ├── cookbook/                  # The five sections
│   │   ├── 01-timeline.md
│   │   ├── 02-kitchen-notes.md
│   │   ├── 03-recipes.md
│   │   ├── 04-network.md
│   │   └── 05-vision.md
│   ├── financial-operations/      # Budgets & playbooks
│   │   ├── playbook.md
│   │   ├── materials-inventory.md
│   │   └── templates.md
│   ├── supporting-documents/      # Org docs, timelines, evaluations
│   │   ├── org-chart.md
│   │   ├── startup-timeline.md
│   │   ├── decision-matrix.md
│   │   ├── 2022-evaluation.md
│   │   ├── 2014-strategic-plan.md
│   │   ├── mailchimp-voice.md
│   │   └── press.md
│   ├── for-replicators/           # Guidance for new cities
│   │   ├── budgets.md
│   │   ├── staffing.md
│   │   ├── host-org-vetting.md
│   │   ├── selection-process.md
│   │   └── methodology.md
│   └── archive/                   # Historical materials
├── README.md                       # GitHub repo landing
├── QUICKSTART.md                   # This file
└── .gitignore
```

---

## Editing Guide

### Adding New Content

1. **Create a new markdown file** in the appropriate folder
2. **Add it to `_sidebar.md`** so it appears in navigation
3. **Use markdown formatting** (headers, bold, links, code blocks)
4. **Commit and push** to GitHub

### Markdown Syntax

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*

- Bullet list
- Another item
  - Nested item

1. Numbered list
2. Another item

[Link text](url)

> Blockquote

`inline code`

\`\`\`python
code block
\`\`\`

| Column 1 | Column 2 |
|----------|----------|
| Cell 1   | Cell 2   |
```

### Linking Between Sections

```markdown
[Section 1: Timeline](/docs/cookbook/01-timeline.md)
[Financial Playbook](/docs/financial-operations/playbook.md)
[Read more](#heading-in-same-file)
```

---

## Deployment

### Automatic (Recommended)

GitHub Pages automatically builds and deploys the site whenever you push to the `main` branch.

1. Push changes to GitHub
2. GitHub Actions (if enabled) or GitHub Pages automatically rebuilds the site
3. Site updates at `https://jif-cookbook.github.io` (usually within 1-2 minutes)

### Manual

If automatic deployment isn't working:

1. Go to repository Settings → Pages
2. Ensure Source is set to `main` branch, `/docs` folder
3. Click Save
4. GitHub will rebuild and deploy

---

## Custom Domain (Optional)

To use `jerusaleminternationalfellows.com` or a custom domain:

1. **Register domain** (GoDaddy, Namecheap, etc.)
2. **Update DNS settings** to point to GitHub Pages:
   - Add CNAME record: `jif-cookbook.github.io`
   - Or add A records with GitHub's IP addresses (check GitHub docs)
3. **Create CNAME file** in the `docs/` folder containing your domain name:
   ```
   jerusaleminternationalfellows.com
   ```
4. **Commit and push**
5. **Verify in GitHub Settings** → Pages → Custom Domain
6. **Enable HTTPS** (automatic, usually)

---

## Access & Permissions

### GitHub Team Access

To give someone edit access:

1. Go to repository Settings → Collaborators
2. Invite them as a Collaborator
3. They can now push changes directly

### Making It Read-Only for Viewers

The site is automatically read-only for visitors. Only people with GitHub access can edit.

---

## Troubleshooting

**Site not updating after push:**
- Wait 1-2 minutes for GitHub to rebuild
- Clear your browser cache (Ctrl+Shift+Delete or Cmd+Shift+Delete)
- Check GitHub Actions for build errors (if enabled)

**Sidebar not showing:**
- Ensure `_sidebar.md` exists in `docs/` folder
- Check that paths in sidebar are correct
- Refresh the page

**Links not working:**
- Use full paths starting with `/`: `/docs/cookbook/01-timeline.md`
- Don't use relative paths like `../cookbook/`
- Ensure markdown files exist at the path you're linking to

**Search not working:**
- Search index may need time to update (up to 24 hours for large sites)
- Try refreshing after a few minutes

---

## Docsify Documentation

For more advanced customization, see official Docsify docs:
- https://docsify.js.org/
- https://docsify.js.org/#/configuration

---

## Questions?

- **Technical issues:** Check Docsify docs or GitHub Issues
- **Content questions:** Contact the Cookbook maintainer
- **GitHub Pages issues:** See GitHub's official documentation

---

**Setup completed:** July 19, 2026  
**Maintainer:** Alexandra Nyashina, ANyashina LLC  
**Future Owner:** Elise Bernhardt
