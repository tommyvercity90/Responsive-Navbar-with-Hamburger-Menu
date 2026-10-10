# Responsive Navbar with Hamburger Menu

A simple and modern **Responsive Navigation Bar** built using HTML5, CSS3, and JavaScript. 
The navbar displays horizontal links on desktop screens and transforms into a hamburger menu 
with a smooth slide-in animation on mobile devices.


## 📌 Table of Contents

- Overview
- Features
- Technologies Used
- Project Structure
- Preview
- Installation
- How It Works
- Customization
- Learning Objectives
- Future Improvements
- Resources
- Author
- License

## 📖 Overview

The Responsive Navbar project demonstrates how to build a navigation bar that adapts to different screen sizes.

On desktop screens, navigation links are displayed horizontally. On smaller screens, the links are replaced by a hamburger button that opens and closes a slide-in navigation menu.

This project is ideal for beginners who want to practice responsive web design, CSS transitions, media queries, DOM manipulation, and JavaScript event handling.

## ✨ Features

- 📱 **Responsive Design:** Adapts to desktop, tablet, and mobile screens.
- 🍔 **Hamburger Menu:** Displays a menu toggle button on smaller screens.
- 🎬 **Smooth Animation:** Uses CSS transitions for the slide-in menu.
- ❌ **Animated Close Icon:** Transforms the hamburger icon into an X.
- 🔗 **Navigation Links:** Includes Home, About, Services, and Contact.
- 🖱️ **Click to Close:** The menu closes when a navigation link is selected.
- ♿ **Accessibility Support:** Uses ARIA attributes to communicate the menu's state.
- 🔄 **Resize Handling:** Resets the mobile menu when returning to desktop view.
- 🎨 **Customizable Styling:** Easy to modify colors, spacing, fonts, and animations.

## 🛠️ Technologies Used

| Technology | Purpose                                     |
| ---------- | ------------------------------------------- |
| HTML5      | Structure and navigation elements           |
| CSS3       | Styling, responsive layouts, and animations |
| JavaScript | Menu toggling and event handling            |

## 📂 Project Structure

```
responsive-navbar/
│
├── index.html
├── style.css
├── script.js
└── README.md
```

- **index.html** — Defines the navbar, hamburger button, navigation links, and hero section.
- **style.css** — Contains the navbar styling, mobile media query, and transition animations.
- **script.js** — Controls menu opening, closing, and responsive behavior.
- **README.md** — Documents the project and installation instructions.

## 🖥️ Preview

### Desktop View

The navigation links appear horizontally in the navbar.

```
┌─────────────────────────────────────────────────────┐
│  MyWebsite       Home  About  Services  Contact      │
└─────────────────────────────────────────────────────┘

             Welcome to MyWebsite
       A simple and responsive navigation bar.
```

### Mobile View

The navigation links are hidden until the hamburger button is clicked.

```
┌──────────────────────────────┐
│  MyWebsite               ☰   │
├──────────────────────────────┤
│                              │
│     Welcome to MyWebsite     │
│                              │
└──────────────────────────────┘
```

> Note: These are illustrative text previews, not actual screenshots.

## 🚀 Installation

Follow these steps to run the project locally.

### 1. Clone the Repository

```
git clone https://github.com/your-username/responsive-navbar.git
```

Replace `your-username` with your GitHub username and use your actual repository URL.

### 2. Navigate to the Project Folder

```
cd responsive-navbar
```

### 3. Open the Project

Open `index.html` in your web browser.

Alternatively, use the **Live Server** extension in Visual Studio Code for a convenient development experience.

No additional packages or dependencies are required.

## ⚙️ How It Works

### 1. Responsive Media Query

CSS uses a media query to change the navigation layout on smaller screens.

```
@media (max-width: 768px) {
  .hamburger {
    display: flex;
  }
}
```

When the viewport width is 768px or less, the hamburger button becomes visible.

### 2. Toggle the Menu

JavaScript toggles the `active` class when the hamburger button is clicked.

```
const isOpen = navMenu.classList.toggle("active");
```

- If the menu is closed, the `active` class is added.
- If the menu is open, the `active` class is removed.

### 3. Slide-In Animation

CSS transitions animate the menu's horizontal position.

```
.nav-menu {
  transform: translateX(100%);
  transition: transform 0.3s ease;
}

.nav-menu.active {
  transform: translateX(0);
}
```

The menu slides in from the right when the `active` class is applied.

### 4. Close on Navigation

JavaScript attaches click listeners to the navigation links. Selecting a link removes the `active` class and closes the mobile menu.

### 5. Accessibility

The hamburger button uses `aria-expanded` to indicate whether the menu is open and `aria-controls` to identify the navigation element it controls.

## 🎨 Customization

You can easily personalize the navbar.

### Change the Background Color

Edit `style.css`:

```
.navbar {
  background: #111827;
}
```

### Change the Navbar Logo

Edit `index.html`:

```
<a href="#" class="logo">MyWebsite</a>
```

Replace `MyWebsite` with your preferred website name.

### Change the Mobile Breakpoint

Edit the media query in `style.css`:

```
@media (max-width: 768px) {
  /* Mobile navigation styles */
}
```

For example, changing `768px` to `600px` makes the mobile layout activate at a narrower viewport.

### Adjust the Animation Speed

```
transition: transform 0.3s ease;
```

Change `0.3s` to `0.5s` for a slower transition.

## 🎯 Learning Objectives

By completing this project, you can practice:

- Creating semantic HTML navigation elements.
- Building flexible layouts with CSS Flexbox.
- Writing responsive media queries.
- Applying CSS transforms and transitions.
- Manipulating classes using JavaScript.
- Handling click and resize events.
- Improving accessibility with ARIA attributes.
- Organizing a project into separate HTML, CSS, and JavaScript files.

## 🔮 Future Improvements

Some ideas to extend the project:

- Add a dropdown menu.
- Add an overlay behind the mobile menu.
- Close the menu when the Escape key is pressed.
- Add active link highlighting based on the current section.
- Add a dark/light theme toggle.
- Improve keyboard navigation and focus management.
- Add a dedicated mobile menu animation style.

## 📚 Resources

- [MDN — CSS Media Queries](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries)
- [MDN — CSS Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_transitions/Using_CSS_transitions)
- [MDN — JavaScript classList](https://developer.mozilla.org/en-US/docs/Web/API/Element/classList)
- [MDN — addEventListener()](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener)
- [MDN — ARIA](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA)

