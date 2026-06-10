# Day 03 — CSS Foundation + GitHub Introduction

**Course:** Web Development, AI Chatbots, Agentic AI Workflows & Automation  
**Class Duration:** 2 Hours  
**Session Type:** Practical Coding + GitHub Introduction  
**Main Focus:** Styling the Portfolio Website with CSS + Understanding GitHub  

---

## 🎯 Day 03 Goal

The goal of Day 03 is to style the HTML portfolio website created in Day 02 using CSS and introduce students to GitHub as a platform for saving, organizing, and showcasing code projects.

By the end of this class, students should understand:

- How CSS connects with HTML
- How CSS changes the look and feel of a website
- How to style sections, buttons, navigation, forms, and footer
- What GitHub is and why developers use it
- What a repository is
- Why a `README.md` file matters

---

## ✅ Day 03 Learning Outcomes

By the end of Day 03, students should be able to:

1. Connect `style.css` with `index.html`
2. Understand the role of CSS in web development
3. Use basic CSS selectors
4. Apply colors, fonts, spacing, borders, and backgrounds
5. Understand margin, padding, and the box model
6. Style headings, sections, buttons, cards, and navigation
7. Improve their portfolio website visually
8. Understand what GitHub is
9. Understand what a GitHub repository is
10. Prepare their project for future deployment

---

## ⏱️ Day 03 Class Flow

| Time | Section | Focus |
|---|---|---|
| 0–10 min | Quick Recap | HTML structure, semantic tags, project folder |
| 10–20 min | What is CSS? | CSS role in web design |
| 20–30 min | Connect CSS | Link `style.css` with `index.html` |
| 30–45 min | CSS Selectors | `body`, `header`, `section`, `button` |
| 45–75 min | Portfolio Styling | Header, navbar, sections, hero, buttons |
| 75–90 min | Form + Footer Styling | Contact form and footer |
| 90–105 min | Student Customization | Colors, spacing, personal design |
| 105–115 min | GitHub Introduction | What GitHub is and why developers use it |
| 115–120 min | Recap + Homework | CSS polish + GitHub preparation |

---

# 1. Quick Recap of Day 02

Ask students:

```text
1. What is index.html?
2. What is HTML used for?
3. What does <header> mean?
4. What does <section> mean?
5. What does <nav> mean?
6. What is the purpose of a form?
7. What did we build yesterday?
```

Teacher line:

> Yesterday we created the structure of our portfolio website using HTML. Today we will use CSS to make it look modern, clean, and professional.

---

# 2. What is CSS?

CSS stands for **Cascading Style Sheets**.

CSS controls how a website looks.

CSS controls:

- Colors
- Fonts
- Spacing
- Layout
- Backgrounds
- Borders
- Buttons
- Cards
- Section design
- Mobile responsiveness later

---

## HTML vs CSS

| HTML | CSS |
|---|---|
| Structure | Design |
| Skeleton | Clothes and styling |
| Content | Presentation |
| Creates sections | Makes sections beautiful |

Teacher line:

> HTML creates the website structure. CSS gives it style, spacing, colors, and personality.

---

# 3. Connect CSS to HTML

Open `index.html`.

Inside the `<head>` section, add this line:

```html
<link rel="stylesheet" href="style.css">
```

The full `<head>` should look like this:

```html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio Website</title>
  <link rel="stylesheet" href="style.css">
</head>
```

Explanation:

```text
rel="stylesheet" means this file is a CSS design file.
href="style.css" tells HTML where the CSS file is located.
```

Now open `style.css` and write:

```css
body {
  background-color: lightyellow;
}
```

Save the file and refresh the browser.

Ask students:

> What changed on the website?

Then change it to:

```css
body {
  background-color: #f4f7f5;
}
```

This proves the CSS file is connected successfully.

---

# 4. CSS Selectors

A CSS selector tells the browser which HTML element we want to style.

## Basic Selectors

```css
body {
  background-color: #f4f7f5;
}

h1 {
  color: green;
}

p {
  color: #333333;
}
```

| Selector | Meaning |
|---|---|
| `body` | Styles the full page |
| `h1` | Styles all main headings |
| `p` | Styles all paragraphs |
| `header` | Styles the top website area |
| `section` | Styles all sections |
| `button` | Styles buttons |

---

## ID Selector

Example:

```css
#hero {
  background-color: white;
}
```

This targets this HTML section:

```html
<section id="hero">
```

Teacher line:

> IDs are used when we want to style one specific section.

---

# 5. Start Styling the Website

Open `style.css`.

Write the CSS step by step.

## Step 1: Reset Basic Spacing

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
```

Explanation:

```text
* targets everything.
margin: 0 removes outside spacing.
padding: 0 removes inside spacing.
box-sizing helps control element size properly.
```

## Step 2: Style the Body

```css
body {
  font-family: Arial, sans-serif;
  background-color: #f4f7f5;
  color: #1f2933;
  line-height: 1.6;
}
```

Explanation:

| Property | Meaning |
|---|---|
| `font-family` | Changes text style |
| `background-color` | Changes page background |
| `color` | Changes default text color |
| `line-height` | Improves readability |

## Step 3: Style the Header

```css
header {
  background-color: #064e3b;
  color: white;
  padding: 24px;
  text-align: center;
}
```

Ask students:

> What changed in the header?

---

# 6. Style Navigation

Add:

```css
nav {
  margin-top: 15px;
}

nav a {
  color: white;
  text-decoration: none;
  margin: 0 12px;
  font-weight: bold;
}
```

Explanation:

```text
nav styles the navigation area.
nav a styles the links inside the navigation.
text-decoration: none removes underline.
margin creates spacing between links.
```

Add hover effect:

```css
nav a:hover {
  text-decoration: underline;
}
```

Explanation:

> Hover means the style changes when the mouse goes over the link.

---

# 7. Style Sections as Cards

Add:

```css
section {
  background-color: white;
  margin: 24px auto;
  padding: 28px;
  width: 85%;
  max-width: 900px;
  border-radius: 16px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
}
```

| CSS Property | Meaning |
|---|---|
| `background-color` | Section background |
| `margin` | Space outside the section |
| `padding` | Space inside the section |
| `width` | Section width |
| `max-width` | Prevents section from becoming too wide |
| `border-radius` | Rounded corners |
| `box-shadow` | Soft shadow |

Teacher line:

> This is how simple HTML sections start looking like professional cards.

---

# 8. Style the Hero Section

Add:

```css
#hero {
  text-align: center;
  background: linear-gradient(135deg, #064e3b, #10b981);
  color: white;
}
```

Style hero heading:

```css
#hero h2 {
  font-size: 36px;
  margin-bottom: 12px;
}
```

Style hero paragraph:

```css
#hero p {
  font-size: 18px;
  margin-bottom: 20px;
}
```

Teacher line:

> The hero section is the first impression of the website, so it should look strong and clean.

---

# 9. Style Buttons

Add:

```css
button {
  background-color: #10b981;
  color: white;
  border: none;
  padding: 12px 22px;
  border-radius: 30px;
  cursor: pointer;
  font-weight: bold;
}
```

Add hover effect:

```css
button:hover {
  background-color: #059669;
}
```

| Property | Meaning |
|---|---|
| `background-color` | Button color |
| `border: none` | Removes default border |
| `padding` | Button size |
| `border-radius` | Rounded button |
| `cursor: pointer` | Shows hand cursor |
| `:hover` | Style when mouse moves over button |

---

# 10. Style Skills List and Projects

Add:

```css
ul {
  margin-top: 12px;
  padding-left: 24px;
}

li {
  margin-bottom: 8px;
}
```

Style project headings:

```css
h3 {
  color: #064e3b;
  margin-top: 18px;
}
```

Style section headings:

```css
h2 {
  color: #064e3b;
  margin-bottom: 12px;
}
```

---

# 11. Style Contact Form

Add:

```css
form {
  margin-top: 18px;
}

input,
textarea {
  width: 100%;
  padding: 12px;
  margin-top: 8px;
  border: 1px solid #cbd5e1;
  border-radius: 10px;
  font-size: 16px;
}

textarea {
  height: 100px;
}
```

Teacher line:

> Forms are used to collect user information. CSS makes them clean and easy to use.

---

# 12. Style Footer

Add:

```css
footer {
  text-align: center;
  background-color: #064e3b;
  color: white;
  padding: 18px;
  margin-top: 30px;
}
```

At this point, the website should have:

- Styled header
- Navigation links
- Hero section
- White content cards
- Styled button
- Styled form
- Footer

---

# 13. Final CSS Code for Day 03

At the end of class, `style.css` should look like this:

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  background-color: #f4f7f5;
  color: #1f2933;
  line-height: 1.6;
}

header {
  background-color: #064e3b;
  color: white;
  padding: 24px;
  text-align: center;
}

nav {
  margin-top: 15px;
}

nav a {
  color: white;
  text-decoration: none;
  margin: 0 12px;
  font-weight: bold;
}

nav a:hover {
  text-decoration: underline;
}

section {
  background-color: white;
  margin: 24px auto;
  padding: 28px;
  width: 85%;
  max-width: 900px;
  border-radius: 16px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
}

#hero {
  text-align: center;
  background: linear-gradient(135deg, #064e3b, #10b981);
  color: white;
}

#hero h2 {
  font-size: 36px;
  margin-bottom: 12px;
}

#hero p {
  font-size: 18px;
  margin-bottom: 20px;
}

h2 {
  color: #064e3b;
  margin-bottom: 12px;
}

h3 {
  color: #064e3b;
  margin-top: 18px;
}

ul {
  margin-top: 12px;
  padding-left: 24px;
}

li {
  margin-bottom: 8px;
}

button {
  background-color: #10b981;
  color: white;
  border: none;
  padding: 12px 22px;
  border-radius: 30px;
  cursor: pointer;
  font-weight: bold;
}

button:hover {
  background-color: #059669;
}

form {
  margin-top: 18px;
}

input,
textarea {
  width: 100%;
  padding: 12px;
  margin-top: 8px;
  border: 1px solid #cbd5e1;
  border-radius: 10px;
  font-size: 16px;
}

textarea {
  height: 100px;
}

footer {
  text-align: center;
  background-color: #064e3b;
  color: white;
  padding: 18px;
  margin-top: 30px;
}
```

---

# 14. Student Customization

Ask students to change:

```text
1. Website background color
2. Header color
3. Button color
4. Hero text
5. Skills list
6. About section text
7. Project section content
```

Teacher line:

> A developer does not only write code. A developer improves, tests, and customizes.

---

# 15. GitHub Introduction

## What is GitHub?

GitHub is an online platform where developers save, organize, and showcase their code projects.

Simple explanation:

```text
GitHub = online home for your code projects
```

Students should understand that GitHub is like a **developer portfolio**.

---

## What GitHub Is Used For

| GitHub Feature | Simple Meaning |
|---|---|
| Repository | A project folder stored online |
| Commit | A saved version of your work |
| README | A project explanation file |
| GitHub Profile | A place to showcase your projects |
| Deployment connection | Later we can connect GitHub with Vercel |

---

## What to Tell Students

> Today we are not going deep into Git commands. First, we need to understand why GitHub matters. GitHub helps us save our website project online, show our progress, and later connect it with Vercel to publish the website.

---

## GitHub Practical Option 1: If Students Have GitHub Accounts

Students create a new repository:

```text
portfolio-website
```

Repository description:

```text
My first portfolio website built with HTML, CSS, and JavaScript.
```

Upload these files:

```text
index.html
style.css
script.js
images/
```

---

## GitHub Practical Option 2: If Students Do Not Have GitHub Accounts Yet

Show a teacher demo only.

Explain:

```text
1. Create GitHub account
2. Create new repository
3. Upload project files
4. Add README.md
5. Share repository link
6. Later connect with Vercel
```

Assign account creation as homework.

---

## Simple README.md Starter

```md
# My Portfolio Website

This is my first portfolio website created during the Web Development, AI Chatbots, Agentic AI Workflows & Automation Crash Course.

## What I Used

- HTML
- CSS
- JavaScript

## Website Sections

- Home
- About Me
- Skills
- Projects
- Contact

## What I Learned

I learned how to structure a website using HTML and style it using CSS.

## Future Improvements

- Add better design
- Make it responsive
- Add JavaScript interactivity
- Deploy it using Vercel
```

---

# 16. Recap Questions

Ask:

```text
1. What is CSS used for?
2. How do we connect CSS with HTML?
3. What is a selector?
4. What is padding?
5. What is margin?
6. What is border-radius?
7. What is box-shadow?
8. What does :hover mean?
9. What is GitHub?
10. What is a repository?
```

---

# 🏠 Day 03 Homework

Students should complete:

```text
1. Complete the CSS styling of your portfolio website.
2. Change colors according to your own theme.
3. Make sure all sections have proper spacing.
4. Style your button.
5. Style your contact form.
6. Write the meaning of these CSS properties:
   - color
   - background-color
   - margin
   - padding
   - border-radius
   - box-shadow
   - font-family
   - width
   - max-width
   - hover
7. Create a GitHub account if you do not already have one.
8. Create or prepare a repository named portfolio-website.
9. Write a simple README.md for your project.
10. Bring your GitHub username in the next class.
```

---

# ✅ Day 03 Success Criteria

Day 03 is successful if every student has:

```text
style.css connected
body styled
header styled
navigation styled
sections styled as cards
hero section styled
button styled
form styled
footer styled
website visually improved
personal color changes started
understands what GitHub is
knows what a repository is
has GitHub account created or planned
```

---

# 💡 Best Teaching Tip

Do not explain all CSS properties at once.

Use this pattern:

```text
Write 3–5 lines of CSS
Save
Refresh browser
Ask: What changed?
Explain the property
Let students customize
Move to next block
```

This keeps students interested because CSS gives instant visual results.

---

# 🎤 Best Day 03 Ending Line

> Today we turned our plain HTML structure into a styled website using CSS, and we also learned why developers use GitHub to save and showcase their projects. In the next class, we will improve the layout, make the design more professional, and prepare the website for responsive screens.
