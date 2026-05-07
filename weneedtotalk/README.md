# We Need to Talk — Site

## Folder structure

```
weneedtotalk/
├── index.html          ← Main gallery page
├── about.html          ← About page
├── notes-data.js       ← Your notes list (edit this to add notes)
├── netlify.toml        ← Netlify config
├── admin/
│   ├── index.html      ← Decap CMS admin UI
│   └── config.yml      ← CMS field definitions
└── images/
    └── notes/          ← Drop your note images here
```

---

## Deploying to Netlify (free)

1. **Create a GitHub account** at github.com if you don't have one.

2. **Create a new repository** — go to github.com/new, name it `weneedtotalk`, set it to Public.

3. **Upload these files** — drag the whole folder into the GitHub repo via the web UI, or use GitHub Desktop.

4. **Create a Netlify account** at netlify.com (free tier is plenty).

5. **Import your repo** — in Netlify: Add new site → Import an existing project → GitHub → select your repo. Build settings can be left blank. Click Deploy.

6. **Connect your domain** — in Netlify: Domain management → Add custom domain → follow the DNS instructions.

7. **Enable Netlify Identity + Git Gateway** (this powers the CMS):
   - In Netlify: Site settings → Identity → Enable Identity
   - Under Registration: set to "Invite only"
   - Scroll to Services → Git Gateway → Enable Git Gateway
   - Go to Identity tab → Invite users → invite yourself

8. **Access the CMS** at `yoursite.com/admin` — log in with your invite.

---

## Adding notes without the CMS

Open `notes-data.js` in any text editor. Copy an existing entry, paste it at the top of the array, and update the fields. Drop the image into `images/notes/`.

---

## Image tips

- JPG or PNG both work
- Recommended size: 1200 × 1600px (portrait, 3:4 ratio)
- Keep file sizes under 500kb for fast loading (use squoosh.app to compress)
