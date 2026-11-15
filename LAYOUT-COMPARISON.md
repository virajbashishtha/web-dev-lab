# Practical P13: Flexbox vs. CSS Grid Analysis

**Student:** Viraj Bhashishtha  
**College:** Bosscoder School of Technology  
**Assignment:** Module 3 (CSS Layout Systems)

---

## 1. Core Structural Differences

| Characteristic | CSS Flexbox | CSS Grid |
| :--- | :--- | :--- |
| **Dimensions** | **1D (One-Dimensional)**: Arranges items along a row OR a column. | **2D (Two-Dimensional)**: Controls rows AND columns simultaneously. |
| **Philosophy** | **Content-First**: Item size dictates the space allocation. | **Layout-First**: The container defines tracks, items slot into places. |
| **Grid Lines** | Items wrap to next line independently without column alignment. | Strict column alignment maintained across all rows. |
| **Best Used For** | Navigation menus, action buttons, card tags. | Main page structure, newspaper columns, auto-fit card grids. |

---

## 2. Flexbox Usage in This Portfolio
- **Sticky Navbar (`.navbar`):** Used `display: flex; justify-content: space-between; align-items: center;` to distribute the brand on the left and navigation links on the right.
- **Hero Section (`.hero-section`):** Arranged the introductory text and student profile badge horizontally with flexbox.
- **Footer Columns (`.footer-rows`):** Created a multi-column responsive footer using `flex-wrap: wrap;` and `flex: 1 1 200px;`.

---

## 3. CSS Grid Usage in This Portfolio
- **Projects Grid (`.showcase-grid`):** Implemented `grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));` to auto-fit cards without media queries.
- **Featured Card Span:** Applied `grid-column: span 2` to highlight the primary project on wider screens.
- **Newspaper Layout (`.news-layout-grid`):** Utilized `grid-template-areas` with fractional units (`2.2fr 1.2fr 1fr`) for an editorial front page.

---

## 4. Final Recommendation
Modern web layouts combine both: **CSS Grid is best for the macro page skeleton**, while **Flexbox is best for the micro components** inside each grid area.
