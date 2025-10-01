# Resume Update Checklist

1. **Edit resume.json**
   Open `resume.json` in VS Code.
   Update experience, skills, links, etc.

2. **Preview locally (optional)**
   npx resume serve --theme elegant --port 4001
   Open http://localhost:4001 to check layout and links.

3. **Rebuild the site**
   mkdir -p dist
   npx resume export dist/index.html --theme elegant --format html
   cp public/\* dist/ 2>/dev/null || true
   cp docs/CNAME dist/ 2>/dev/null || true #<-- preserve custom domain
   rm -rf docs && mv dist docs

4. **Commit changes**
   git add resume.json docs
   git commit -m "Update resume content"

5. **Push to GitHub**
   git push origin main
6. **Verify live site**
   Go to https://deanhattenhauer.dev
   Hard refresh (Shift+Reload) or test in incognito.
   Confirm updates appear.

✅ Done! Your updated résumé is live with the new content.
