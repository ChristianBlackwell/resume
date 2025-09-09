# ===============================

# Resume Project Workflow Checklist

# ===============================

#

# 1) Edit your resume

# - Open resume.json in VS Code

# - Make changes to experience, skills, etc.

#

# 2) Preview while editing

# - ATS-safe look (no icons):

# npx resume serve --theme spartan

# - Pretty web look (with icons/layout):

# npx resume serve --theme elegant

#

# 3) Rebuild outputs (PDF + Web HTML)

# - One command to regenerate everything:

# npm run build:all

#

# This will create/update:

# - dist/resume.pdf (ATS-safe Spartan theme)

# - dist/index.html (Elegant web version)

#

# 4) Open / share the results

# - Open the PDF locally:

# open dist/resume.pdf

# - Open the web version locally:

# npm run serve:web

# # then go to http://localhost:4000

#

# 5) (Optional) Hosting the web version

# - Commit and push the dist/ folder to GitHub

# - Enable GitHub Pages or deploy with Netlify

# - Share the link (this uses the Elegant theme)

#

# 6) Version control (optional but recommended)

# - Commit changes to git

# - Tag releases so you can roll back:

# git add .

# git commit -m "Update resume for Sept 2025"

# git tag resume-2025-09

# git push && git push --tags

#

# ===============================

# Notes:

# - Use Spartan (or Paper/Flat) for ATS-safe PDFs.

# - Use Elegant for stylish web versions.

# - The build scripts in package.json bake in the

# correct Chrome path so PDF export always works.

# ===============================
# resume
