# academic-page

Academic homepage for Peiyang Ni (bonjour-npy), built with Jekyll (AcademicPages / Minimal Mistakes).

- Live site: `https://bonjour-npy.github.io/academic-page/`
- Edit content:
  - Home: `_pages/about.md`
  - Publications list page: `_pages/publications.html`
  - CV page: `_pages/cv.md`
  - Publications entries: `_publications/*.md`
- Local rendering:
  - `bundle install` (first time only, to install dependencies)
  - `bundle exec jekyll serve`
  - Open `http://localhost:4000/academic-page/` in a web browser to view the site locally.
- Deployment:
  - `git add . && git commit -m "Update content" && git push`
  - GitHub Pages will automatically build and deploy the site after pushing to the repository.
