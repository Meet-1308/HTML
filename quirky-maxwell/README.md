# CinePulse - Movie Information Portal

### Web Technology–I (2301CS363) - Phase-1 Static UI
**Darshan Institute of Engineering & Technology**  
Department of Computer Engineering

---

## 1. Academic Evaluation Scope: Phase-1 (Weeks 1 to 3)

This project codebase is specifically scoped to fulfill the **Phase-1 Evaluation (Weeks 1 to 3)** of the Web Technology–I syllabus:

| Week | Dates | Unit / Technology | Major Work & Deliverables |
| :--- | :--- | :--- | :--- |
| **Week 1** | 24/08/2026 to 30/08/2026 | **HTML** | Project folder structure, Home, Movies, Movie Details, Forms. (Static HTML Portal) |
| **Week 2** | 31/08/2026 to 06/09/2026 | **CSS** | Page styling, layouts, movie cards, CSS3 design. (Designed Portal) |
| **Week 3** | 07/09/2026 to 13/09/2026 | **HTML + CSS** | Remaining pages, responsive CSS using media queries, complete UI. (Complete Static UI) |
| **Phase-1** | **14/09/2026 to 19/09/2026** | **Phase-1 Evaluation** | **• All major pages completed<br>• Navigation implemented<br>• Movie cards & movie details created<br>• Forms created<br>• CSS design completed<br>• Responsive design implemented<br>Expected Output: Complete Static UI** |

> [!NOTE]
> All subsequent phases (Weeks 4-6 JavaScript/DOM, Week 7 jQuery, Week 8 Bootstrap) have been deliberately excluded as per the Phase-1 evaluation requirements. The portal is built purely with **HTML5 and CSS3**.

---

## 2. Implemented Pages & Functional Requirements

| Page | File | SRS Functional Requirements Covered |
| :--- | :--- | :--- |
| **Home** | `index.html` | **FR-01**: Website logo, navigation menu, featured hero banner, curated statistics bar, genre exploration cards, featured & popular movie grids, semantic footer. |
| **Movie Listing** | `movies.html` | **FR-02, FR-04, FR-05, FR-06**: Collection of 12 complete movie cards, search keyword input, multi-filter dropdowns (genre, language, year, rating), and sorting controls. |
| **Movie Details** | `movie-details.html` | **FR-03**: Cinematic hero backdrop, floating poster card, complete storyline, director & cast list, film specifications, embedded YouTube HD trailer, community critiques, and "More Like This" recommended cards. |
| **Favorites / Watchlist** | `favorites.html` | **FR-07, FR-08**: Watchlist dashboard displaying 4 saved movie cards, summary metrics (total saved, average rating, top genre), and clear/remove action controls. |
| **Reviews & Ratings** | `reviews.html` | **FR-09, FR-10, FR-11, FR-13**: Client-side validated review submission form (name, email, movie dropdown, rating stars, comment textarea) and static community review cards with avatars. |
| **Contact & Feedback** | `contact.html` | **FR-12, FR-13**: Department contact details (campus address, email, phone, lab hours), HTML5 validated contact form, competencies list, and pure HTML5/CSS3 collapsible FAQ accordion. |

---

## 3. Modular CSS Architecture

As requested, each HTML page links to a shared base stylesheet (`css/style.css`) plus its own dedicated page stylesheet:

```
quirky-maxwell/
├── index.html               # Home page (Hero banner, stats, featured/popular movie cards)
├── movies.html              # Movie listing (12 movie cards, search & filter controls)
├── movie-details.html       # Movie details (Storyline, cast, trailer embed, reviews, specs)
├── favorites.html           # Watchlist dashboard (Saved movie cards, metrics)
├── reviews.html             # Reviews & ratings (Review form, community review cards)
├── contact.html             # Contact & feedback (Department info, contact form, FAQ)
├── css/
│   ├── style.css            # Base stylesheet: CSS variables, reset, navbar, footer, cards, buttons, forms
│   ├── home.css             # index.html: Hero banner, stats grid, genre cards, CTA box
│   ├── movies.css           # movies.html: Filter toolbar layout, active filter tags, sort container
│   ├── movie-details.css    # movie-details.html: Cinematic hero, poster box, 16:9 trailer, cast layout
│   ├── favorites.css        # favorites.html: Watchlist metrics grid, remove button layout
│   ├── reviews.css          # reviews.html: Two-column review grid, rating stars, review card items
│   └── contact.css          # contact.html: Department info cards, form grid, pure CSS FAQ accordion
└── README.md                # Project documentation and Phase-1 submission reference
```

---

## 4. Key Technologies & Design Highlights

- **Pure HTML5 Semantics**: Structured using `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<details>`, `<summary>`, and `<footer>`.
- **Pure CSS3 Layouts**:
  - **CSS Flexbox**: Responsive navigation bar, filter tag chips, metadata badges, and review header items.
  - **CSS Grid**: Responsive multi-column movie cards (`repeat(4, 1fr)` adapting to `3`, `2`, and `1` columns), stats dashboard, genre grid, and two-column page layouts.
- **Custom CSS Variables**: Dark theme palette (`--bg-primary`, `--bg-secondary`, `--text-primary`, `--accent-color`, `--accent-gold`, etc.).
- **Responsive Media Queries**: Breakpoints at `1024px`, `768px`, and `480px` for mobile, tablet, and desktop display.
- **Native HTML5 Form Validation**: `required`, `type="email"`, `minlength`, `maxlength`, and `pattern="[A-Za-z\s]+"`.
- **Font Awesome 6 Icons & Web-Safe Fonts**: Uses clean web-safe system fonts (`Segoe UI, Arial, sans-serif`) and high-fidelity Font Awesome 6 icons (`<i class="fa-solid ..."></i>`), replacing all raw emojis across the entire UI.
- **Pure HTML5 & CSS3 Architecture**: Complete static UI with zero JavaScript runtime errors or script dependencies.

---

## 5. How to Run & Verify

1. Open `index.html` directly in any web browser (Google Chrome, Microsoft Edge, Mozilla Firefox).
2. Open Browser Developer Tools (`F12` -> Console tab) to verify:
   - **Zero JavaScript errors**
   - **Zero script requests**
3. Navigate across all 6 pages using the top navigation bar.
4. Resize the browser window or use Device Emulation to observe native CSS media queries adapting the layout across mobile (375px), tablet (768px), and desktop (1200px) screens.
