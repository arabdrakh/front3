# Assignment #3: Responsive Web Design (Media Queries + Bootstrap Grid)

**Course:** Web Technologies Front-End Development  
**Student Name:** Aruzhan Abdrakhmanova  
**Group:** IT-2501  
**University:** Astana IT University  

---

## 📌 Project Overview

The objective of this assignment is to master responsive web design principles using both **pure CSS Media Queries** and the **Bootstrap 5 12-Column Grid System**. The project demonstrates how layouts and typography dynamically adapt to mobile, tablet, and desktop viewports.

### 📁 File Structure

```text
front3/
├── index.html          # Task 4: Responsive Portfolio Page
├── style.css           # Task 4: Custom CSS with custom media queries
├── task0.html          # Task 0: Responsive Typography (Pure CSS)
├── task1.html          # Task 1: Responsive 3-Box Layout (Pure CSS Grid & Media Queries)
├── task2.html          # Task 2: Bootstrap 12-Column Responsive Grid
├── task3.html          # Task 3: Bootstrap Responsive Navigation Bar
├── screenshots/        # Captured screenshots for all tasks across viewports
└── README.md           # Assignment Report
```

---

## Part 1. Media Queries

### Task 0. Responsive Typography

- **Description:**  
  A webpage created with semantic headings (`h1`, `h2`) and paragraphs (`p`). Pure CSS media queries adapt the font sizes across mobile, tablet, and desktop viewports without any external CSS framework.
  - **Mobile (< 768px):** `h1`: 20px, `h2`: 16px, `p`: 14px
  - **Tablet (768px – 1023px):** `h1`: 28px, `h2`: 20px, `p`: 16px
  - **Desktop (≥ 1024px):** `h1`: 36px, `h2`: 24px, `p`: 18px

#### Task 0 Screenshots

**Desktop View (≥ 1024px):**
![Task 0 Desktop](screenshots/task0-desktop.png)

**Tablet View (768px - 1023px):**
![Task 0 Tablet](screenshots/task0-tablet.png)

**Mobile View (< 768px):**
![Task 0 Mobile](screenshots/task0-mobile.png)

---

### Task 1. Responsive Layout with Media Queries

- **Description:**  
  A responsive layout with three content boxes built strictly using pure CSS Grid and Media Queries (no Bootstrap).
  - **Desktop (≥ 900px):** All 3 boxes are displayed side by side (`grid-template-columns: 1fr 1fr 1fr`).
  - **Tablet (600px – 899px):** 2 boxes on the first row, and the third box wraps to the second row (`grid-template-columns: 1fr 1fr`).
  - **Mobile (< 600px):** All boxes are stacked vertically at full width (`grid-template-columns: 1fr`).

#### Task 1 Screenshots

**Desktop View (≥ 900px) — 3 side by side:**
![Task 1 Desktop](screenshots/task1-desktop.png)

**Tablet View (600px - 899px) — 2 in first row, 1 in second row:**
![Task 1 Tablet](screenshots/task1-tablet.png)

**Mobile View (< 600px) — Stacked vertically:**
![Task 1 Mobile](screenshots/task1-mobile.png)

---

## Part 2. Bootstrap Grid System

### Task 2. Bootstrap Responsive Columns

- **Description:**  
  A responsive layout utilizing Bootstrap’s 12-column grid system (`row` and `col-*` classes).
  - Each column uses the class `col-12 col-md-6 col-lg-4`.
  - **Desktop (`lg` ≥ 992px):** Each card occupies 4 columns (4 + 4 + 4 = 12 columns, 3 equal parts side by side).
  - **Tablet (`md` 768px – 991px):** Each card occupies 6 columns, resulting in 2 columns on the first row (6 + 6 = 12) and the third column wrapping to the second row.
  - **Mobile (< 768px):** Each card takes 12 columns (`col-12`), stacking all cards vertically.

#### Task 2 Screenshots

**Desktop View (3 equal columns):**
![Task 2 Desktop](screenshots/task2-desktop.png)

**Tablet View (2 on row 1, 1 on row 2):**
![Task 2 Tablet](screenshots/task2-tablet.png)

**Mobile View (Stacked columns):**
![Task 2 Mobile](screenshots/task2-mobile.png)

---

### Task 3. Bootstrap Navigation Bar

- **Description:**  
  A responsive navbar built using Bootstrap 5 components:
  - **Logo on the left:** Brand name (`Aruzhan`) aligned using `.navbar-brand`.
  - **Links on the right:** Navigation links right-aligned using Bootstrap's `ms-auto` class.
  - **Collapsible menu:** When the viewport width is below the `md` breakpoint (< 768px), navigation links collapse into an accessible hamburger menu (`navbar-toggler`) that opens and closes via Bootstrap JS.

#### Task 3 Screenshots

**Desktop View (Logo left, links right):**
![Task 3 Desktop](screenshots/task3-desktop.png)

**Mobile View (Collapsed into hamburger menu button):**
![Task 3 Mobile](screenshots/task3-mobile.png)

---

## Part 3. Combined Project

### Task 4. Responsive Portfolio Page (`index.html` & `style.css`)

- **Description:**  
  A complete personal portfolio page combining both Bootstrap 5 Grid and custom CSS Media Queries in `style.css`:
  1. **Header:** Responsive Bootstrap navbar with logo on the left, collapsible hamburger toggler, and navigation links.
  2. **Main Section:**
     - **Left Side (`col-lg-8`):** Portfolio project cards arranged using Bootstrap grid (`col-md-6`).
     - **Right Side (`col-lg-4`):** Sidebar containing personal information, student bio, and contact details.
  3. **Footer:** Bottom footer with copyright and university affiliation.
  4. **Custom Media Queries (`style.css`):**
     - Adjusts typography (`h1` scales from 24px to 30px and 36px).
     - Controls spacing (`main` padding scales from 15px to 25px and 35px).
     - Element visibility: `.extra-info` is hidden on mobile (`display: none;`) and shown on tablet/desktop via `display: block;`.

#### Task 4 Screenshots

**Desktop View:**
![Task 4 Desktop](screenshots/task4-desktop.png)

**Tablet View:**
![Task 4 Tablet](screenshots/task4-tablet.png)

**Mobile View:**
![Task 4 Mobile](screenshots/task4-mobile.png)

---

## 📝 Brief Summary of Work Process

1. **Part 1 — Pure Media Queries:**  
   - Built `task0.html` to demonstrate responsive typography across mobile, tablet, and desktop viewports using CSS media queries.
   - Built `task1.html` using CSS Grid (`1fr`, `1fr 1fr`, `1fr 1fr 1fr`) to implement the 3-box responsive layout without any framework.

2. **Part 2 — Bootstrap 5 Grid & Navbar:**  
   - Implemented `task2.html` using Bootstrap’s 12-column grid (`col-12 col-md-6 col-lg-4`) to satisfy responsive column wrapping requirements.
   - Implemented `task3.html` using the Bootstrap navbar component with logo on the left, `ms-auto` links on the right, and hamburger toggler for smaller viewports.

3. **Part 3 — Combined Portfolio Page:**  
   - Created `index.html` and `style.css` combining Bootstrap's grid structure for projects with custom media queries for font scaling, spacing, and element visibility (`display: block` on `.extra-info`).
   - Styled the site with a clean, distinctive color theme suitable for front-end student coursework.

4. **Testing & Version Control:**  
   - Tested each page across multiple screen dimensions (Mobile: 420px, Tablet: 750px–800px, Desktop: 1100px).
   - Captured screenshots across all breakpoints and updated the report.
   - Maintained clean, step-by-step Git commits.

---

## 📚 References & Resources

1. Abitova G.A., *Web technologies Front-End Development. Part 1*, 2022.
2. [Bootstrap 5.3 Documentation](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
3. [MDN Web Docs - Responsive Design](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design)
4. [W3Schools - CSS Media Queries](https://www.w3schools.com/css/css_rwd_mediaqueries.asp)
