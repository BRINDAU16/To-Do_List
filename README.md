# To-Do_List
# ✅ To-Do List App

A clean, minimal To-Do List web app built with pure HTML, CSS, and JavaScript — no frameworks, no dependencies, no setup required.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## 🖥️ Demo

Just download `todo-list.html` and open it in any browser. That's it!

---

## ✨ Features

- **Add tasks** — type and press Enter or click the `+` button
- **Complete tasks** — click the circle checkbox to mark as done
- **Delete tasks** — click the ✕ button to remove a task
- **Filter tasks** — view All, Active, or Done tasks
- **Clear completed** — remove all finished tasks at once
- **Progress ring** — shows percentage of tasks completed
- **Persistent storage** — tasks are saved in `localStorage` and survive page refreshes

---

## 🚀 Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/todo-list.git
   ```

2. **Open the file**
   ```bash
   cd todo-list
   open todo-list.html
   ```
   Or just double-click `todo-list.html` in your file explorer.

No installs. No build steps. No internet required.

---

## 📁 Project Structure

```
todo-list/
└── todo-list.html   # The entire app — HTML, CSS, and JS in one file
└── README.md        # You're reading this!
```

---

## 🧠 How It Works

The app is built around three core ideas:

### 1. A tasks array
All tasks live in a JavaScript array of objects:
```javascript
let tasks = [
  { id: 1, text: "Learn HTML", done: false },
  { id: 2, text: "Build this app", done: true  }
];
```

### 2. A `render()` function
Every time something changes (add, delete, check), the list is re-drawn from scratch:
```javascript
function render() {
  listEl.innerHTML = '';
  tasks.forEach(task => {
    // create and append each task element
  });
}
```

### 3. localStorage
Tasks are saved to the browser so they persist across page refreshes:
```javascript
localStorage.setItem('tasks', JSON.stringify(tasks));
```

---

## 🎨 Customisation

All colours are stored as CSS variables at the top of the `<style>` block — easy to change:

```css
:root {
  --bg:      #f5f0e8;   /* page background   */
  --accent:  #c1440e;   /* primary colour    */
  --text:    #1a1610;   /* main text colour  */
}
```

---

## 💡 Ideas to Extend

- [ ] Add task priority levels (High / Medium / Low)
- [ ] Add due dates to tasks
- [ ] Allow editing a task by double-clicking it
- [ ] Add drag-and-drop to reorder tasks
- [ ] Add categories or tags
- [ ] Sync tasks to a backend using `fetch()`

---

## 📚 What I Learned

This project covers core beginner web development concepts:

- Structuring a page with **HTML**
- Styling with **CSS** (variables, flexbox, animations, custom checkboxes)
- DOM manipulation with **JavaScript**
- Handling user events (click, keydown, change)
- Persisting data with **localStorage**
- Writing clean, readable code

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

*Built as a beginner project to learn HTML, CSS, and JavaScript.*
