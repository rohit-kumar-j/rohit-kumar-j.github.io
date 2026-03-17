# 🚧 Rohit Jakkula — Academic Website (Under Construction)

Personal website → [rohit-kumar-j.github.io](https://rohit-kumar-j.github.io)

---

## TODO — Content

- [ ] Add profile photo → `files/me.jpg`
- [ ] Add CV → `files/cv.pdf`
- [ ] Add Syracuse University logo → `files/logo-syr.png` (for Experience section)
- [ ] Confirm and update Google Scholar link in `index.html` (search for `scholar.google.com/TODO`)
- [ ] Uncomment and fill in LinkedIn link if desired
- [ ] Uncomment and fill in Twitter/X link if desired
- [ ] Add MS degree start/end dates in Experience section
- [ ] Add previous education / undergrad entry in Experience
- [ ] Add publication thumbnail images → `files/paperN.png` (for future papers)
- [ ] Verify IROS 2025 acceptance for the Transformable Modular Robots paper (currently listed as IROS 2025)
- [ ] Add more publications when available (use the commented template in `index.html`)
- [ ] Add more specializations/certifications (use the commented template in the Specializations section)
- [ ] Remove the "Under Construction" banner when ready (`<div class="under-construction">` in `index.html`)

---

## TODO — Technical

- [ ] Set up GitHub repository named `rohit-kumar-j.github.io`
- [ ] Push to `main` branch and enable GitHub Pages

---

## How to Go Live on GitHub Pages

1. Create a repo on GitHub named exactly **`rohit-kumar-j.github.io`**
2. From this folder, run:
   ```bash
   git init
   git add .
   git commit -m "initial site"
   git remote add origin https://github.com/rohit-kumar-j/rohit-kumar-j.github.io.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Source → Deploy from branch → `main` / `/ (root)`**
4. Site goes live at `https://rohit-kumar-j.github.io` within ~1 minute

> **Your CV is automatically hosted** at `https://rohit-kumar-j.github.io/files/cv.pdf` once you push `files/cv.pdf`.

---

## Adding a New Publication

Copy this block inside `<div id="pub-list">` in `index.html`:

```html
<article class="publication"
    data-title="lowercase paper title"
    data-authors="lowercase author names"
    data-venue="conference-shortname (iros / icra / arxiv / neurips / cvpr / etc.)"
    data-year="202X">
    <div class="row">
        <div class="row-media" style="background-image: url(files/paperN.png);"></div>
        <div class="row-text">
            <a class="publication-title" href="PAPER_URL">Paper Title</a>
            <div class="publication-authors"><span class="bold">Rohit Jakkula</span>, Co-author</div>
            <div class="publication-venue"><span class="italic" style="color:#C4956A">Venue Year</span></div>
            <div class="publication-links">
                <a class="btn btn-red" href="#">PDF</a>
                <a class="btn btn-dark" href="#">Code</a>
            </div>
        </div>
    </div>
</article>
```

Also add a new **filter button** if the venue isn't already covered — find `<div class="pub-filters">` and add:
```html
<button class="pub-filter" data-filter="icra">ICRA</button>
```

---

## Design Credit

Inspired by [Xinyue Wei's website](https://sarahweiii.github.io/)
