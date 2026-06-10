# Day 02 — Developer Setup + HTML Foundation + First Portfolio Page

[Presntation Link](https://canva.link/is94oensrm315ja)

---

## 🎯 Day 02 Goal

Students will set up their coding environment and build the first real structure of their portfolio website using HTML.

Day 01 gave students the full course overview.  
Day 02 moves from inspiration to implementation.

---

## ✅ Day 02 Learning Outcomes

By the end of Day 02, students should be able to:

- Open VS Code and create a project folder
- Understand the purpose of `index.html`, `style.css`, and `script.js`
- Run a website using Live Server
- Write a proper HTML boilerplate
- Use basic HTML tags
- Understand semantic HTML structure
- Create the first structure of a portfolio website
- Understand that HTML is the foundation of every website

---


## What is a Website?

A website is a collection of pages that people open in a browser.

Examples:

- School website
- YouTube
- Portfolio website
- Online store
- Registration page

---

## What is Web Development?

Web development means creating websites and web applications.

It includes:

- Structure
- Design
- Interactivity
- Deployment

---

## Static vs Dynamic Website

| Static Website | Dynamic Website |
|---|---|
| Same content for everyone | Content can change for each user |
| Best for portfolios and landing pages | Used for dashboards, accounts, e-commerce |
| No database needed | Usually uses database |
| Easier for beginners | More advanced |


> In this course, we will first build a static portfolio website because it is the best foundation project.

---

## Frontend vs Backend

| Frontend | Backend |
|---|---|
| What users see | What happens behind the scenes |
| HTML, CSS, JavaScript | Database, login, APIs, server |
| Buttons, text, images, layout | User accounts, payments, stored data |

---

## Client and Server

Simple explanation:

```text
Client = your browser
Server = computer that sends website files
```

Flow:

```text
Browser asks for website
↓
Server sends website files
↓
Browser shows website
```

---

## 3. Old Way vs Modern Way of Coding

### Old Way

Developers can write HTML in Notepad.

```html
<h1>Hello Students</h1>
<p>This is my first web page.</p>
```


> This works, but professional developers use VS Code because it helps us write code faster, cleaner, and with fewer mistakes.

---

## 4. VS Code Setup

### Step 1: Create Project Folder

Create a folder on Desktop:

```text
portfolio-website
```

Inside it, create:

```text
index.html
style.css
script.js
images
```

Final structure:

```text
portfolio-website/
  index.html
  style.css
  script.js
  images/
```

---

## File Purpose

| File | Purpose |
|---|---|
| `index.html` | Main website structure |
| `style.css` | Website design |
| `script.js` | Website interactivity |
| `images/` | Store pictures and icons |

---

### Step 2: Open Folder in VS Code

Steps:

```text
1. Open VS Code.
2. Click File → Open Folder.
3. Select portfolio-website.
4. Create files if not already created.
```

---

### Step 3: Open Website With Live Server


> Live Server lets us open our website in the browser and see changes quickly.

Steps:

```text
1. Right-click index.html.
2. Select Open with Live Server.
3. Your website will open in the browser.
```

---

## 5. HTML Boilerplate


> Every proper HTML page has a basic structure. This is called the HTML boilerplate.

Write this code together:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio Website</title>
</head>
<body>

</body>
</html>
```

---

## HTML Boilerplate Explanation

| Code | Meaning |
|---|---|
| `<!DOCTYPE html>` | Tells the browser this is an HTML document |
| `<html lang="en">` | Starts the HTML page and sets language to English |
| `<head>` | Contains information about the website |
| `<meta charset="UTF-8">` | Helps browser understand text and symbols |
| `<meta name="viewport"...>` | Helps the website work on mobile screens |
| `<title>` | Text shown on the browser tab |
| `<body>` | Visible content of the website |


> If you understand this structure, you already understand the skeleton of every website.

---

## 6. Basic HTML Tags

Inside `<body>`, add:

```html
<h1>Welcome to My Portfolio</h1>
<p>Hello, my name is Ali. I am learning web development.</p>
```



---

## Common HTML Tags

| Tag | Purpose |
|---|---|
| `<h1>` | Main heading |
| `<h2>` | Section heading |
| `<h3>` | Smaller heading |
| `<p>` | Paragraph |
| `<ul>` | Unordered list |
| `<ol>` | Ordered list |
| `<li>` | List item |
| `<a>` | Link |
| `<img>` | Image |
| `<button>` | Button |
| `<section>` | Page section |
| `<form>` | Form container |
| `<input>` | Input field |
| `<textarea>` | Message box |
| `<label>` | Form label |

---

## Add About Section

```html
<h2>About Me</h2>
<p>I am a student who is interested in technology, websites, and AI.</p>
```

---

## Add Skills List

```html
<h2>My Skills</h2>
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
  <li>AI Tools</li>
</ul>
```

---

## Add Link

```html
<h2>My Favorite Website</h2>
<a href="https://www.google.com" target="_blank">Visit Google</a>
```


```text
href = link address
target="_blank" = opens link in a new tab
```

---

## Add Button

```html
<h2>Contact Me</h2>
<button>Send Message</button>
```

---

## Add Image Placeholder

```html
<img src="images/profile.png" alt="My profile picture" width="200">
```


```text
src = image location
alt = image description
width = image size
```

> Even if the image does not show today, you now understand how images are added.

---

## 7. Semantic HTML Structure

Semantic HTML means using tags that clearly describe the purpose of each part of the page.

| Tag | Purpose |
|---|---|
| `<header>` | Top part of website |
| `<nav>` | Navigation links |
| `<main>` | Main content |
| `<section>` | Content section |
| `<footer>` | Bottom part of website |


> Good developers do not only write code that works. They write code that is clean and understandable.

---

## 8. First Portfolio Website Structure

Now students build the first proper version of their portfolio.

> Do not paste everything at once. Teach it block by block.

---

## Complete Starter Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio Website</title>
</head>
<body>

  <header>
    <h1>My Portfolio</h1>

    <nav>
      <a href="#about">About</a>
      <a href="#skills">Skills</a>
      <a href="#projects">Projects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>

    <section id="hero">
      <h2>Hello, I am [Your Name]</h2>
      <p>I am learning Web Development, AI Chatbots, and Agentic AI Workflows.</p>
      <button>View My Work</button>
    </section>

    <section id="about">
      <h2>About Me</h2>
      <p>
        I am a student interested in technology, creativity, and future digital skills.
        This is my first portfolio website.
      </p>
    </section>

    <section id="skills">
      <h2>My Skills and Interests</h2>
      <ul>
        <li>Web Development</li>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>AI Tools</li>
      </ul>
    </section>

    <section id="projects">
      <h2>My Projects</h2>

      <h3>Portfolio Website</h3>
      <p>A personal website created using HTML, CSS, and JavaScript.</p>

      <h3>AI Chatbot / AI Assistant</h3>
      <p>An AI assistant idea that helps users with useful information.</p>
    </section>

    <section id="contact">
      <h2>Contact Me</h2>
      <p>You can contact me for learning, collaboration, or project ideas.</p>

      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" placeholder="Enter your name">

        <br><br>

        <label for="message">Message:</label>
        <textarea id="message" placeholder="Write your message"></textarea>

        <br><br>

        <button type="button">Submit</button>
      </form>
    </section>

  </main>

  <footer>
    <p>© 2026 My Portfolio Website. Built with HTML.</p>
  </footer>

</body>
</html>
```

---

## Teaching the Code Block by Block

### Block 1: Header

```html
<header>
  <h1>My Portfolio</h1>
</header>
```


> This is the top area of our website.

---

### Block 2: Navigation

```html
<nav>
  <a href="#about">About</a>
  <a href="#skills">Skills</a>
</nav>
```


> These links move us to sections of the same page.

---

### Block 3: Hero Section

```html
<section id="hero">
  <h2>Hello, I am [Your Name]</h2>
  <p>I am learning Web Development.</p>
</section>
```


> The hero section is the first main section visitors see.

---

### Block 4: About and Skills



> About tells who you are. Skills show what you are learning.

---

### Block 5: Projects



> Project section is important because developers show what they have built.

---

### Block 6: Contact Form


> Forms are how websites collect information.

---

## 9. Student Customization

Students should customize:

```text
1. Replace [Your Name] with their real name.
2. Change the about paragraph.
3. Add their own skills.
4. Add one project idea.
5. Change footer text.
```

This makes the class feel personal.

---

## 10. Recap Questions

Ask students:

```text
1. What is index.html?
2. What is HTML used for?
3. What does <h1> do?
4. What does <p> do?
5. What is a section?
6. Why do we use semantic tags?
7. What is Live Server?
```

---

## 🏠 Day 02 Homework

Students should complete:

```text
1. Complete your HTML portfolio structure.
2. Replace all sample text with your own content.
3. Add at least 5 skills/interests.
4. Add 2 project ideas.
5. Add your own About Me paragraph.
6. Write the meaning of these tags:
   - h1
   - p
   - a
   - img
   - ul
   - li
   - section
   - header
   - footer
   - form
7. Bring one image or avatar idea for your portfolio.
```

---

## ✅ Day 02 Success Criteria

Day 02 is successful if every student has:

```text
Project folder created
index.html created
style.css created
script.js created
Live Server working
HTML boilerplate written
Portfolio structure created
At least 5 HTML tags used
At least 4 sections created
Basic form added
Personal content started
```

---

## 💡 Best Teaching Tip

Do not say:

> Copy this code.

Say:

> Let’s build this website step by step like real developers.

After every 5–7 lines of code, ask:

> What changed on the website?

This keeps students interested because they immediately see the result of each line.

---

## 🎤 Best Day 02 Ending Line

> Today you did not just learn HTML tags. You created the structure of your first real portfolio website. In the next class, we will use CSS to make this website look modern and professional.
