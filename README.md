# szczepienia-privacy — manual GH Pages deployment

Deployment when gh CLI is authenticated:

```bash
cd ~/Desktop/Projects/Szczepienia/privacy-policy
gh auth login   # if not done
gh repo create MacSiem/szczepienia-privacy --public --source . --push
# In GitHub repo Settings → Pages → Source: main branch / root
# After ~30s: https://macsiem.github.io/szczepienia-privacy/ live (200 OK)
```

Files in this folder ready for `git init && git push`:
- `index.html` — main privacy policy (PL+EN)
- `delete-data.html` — required Play Console "Account deletion request URL"
- `README.md` — this file
