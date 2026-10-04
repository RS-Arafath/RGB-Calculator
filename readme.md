# 🧮 Basic Calculator

A clean, modern, and interactive **Basic Calculator** built with **HTML, CSS, and Vanilla JavaScript**. It features a polished dark/light interface, keyboard support, smooth button animations, and essential arithmetic operations.

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  
</p>

<p align="center">
  <a href="">🌐 Live Demo</a>
  &nbsp; • &nbsp;
  <a href="https://github.com/RS-Arafath/RGB-Calculator.git">📂 GitHub Repository</a>
</p>

---

## 📸 Preview

<table width="100%">
  <tr>
    <td width="50%" align="center">
      <img src="/images/light-theme.png" alt="Light Theme" width="100%" />
    </td>
    <td width="50%" align="center">
      <img src="/images/dark-theme.png" alt="Dark Theme" width="100%" />
    </td>
  </tr>
</table>

> Replace `YOUR_SCREENSHOT_URL` with your calculator screenshot after uploading it to the repository.

---

## ✨ Features

* ➕ Addition
* ➖ Subtraction
* ✖️ Multiplication
* ➗ Division
* `%` Percentage calculation
* `+/−` Positive/negative toggle
* `AC` All Clear
* 🔢 Decimal number support
* ⌨️ Full keyboard support
* 🌙 Dark mode
* ☀️ Light mode
* 💫 Ripple button animation
* 🌈 RGB button press effect
* 📱 Compact responsive interface
* ⚠️ Division-by-zero error handling
* 📐 Automatic result text resizing for long numbers

---

## 🛠️ Tech Stack

| Technology       | Purpose                           |
| ---------------- | --------------------------------- |
| **HTML5**        | Application structure             |
| **CSS3**         | Styling and animations            |
| **JavaScript**   | Calculator logic and interactions |
| **Tailwind CSS** | Utility-based styling             |
| **DaisyUI**      | UI styling support                |

Tailwind CSS and DaisyUI are loaded through CDN, while the calculator functionality is implemented using Vanilla JavaScript.

---

## ⌨️ Keyboard Shortcuts

| Key           | Action            |
| ------------- | ----------------- |
| `0 – 9`       | Enter number      |
| `+`           | Addition          |
| `-`           | Subtraction       |
| `*`           | Multiplication    |
| `/`           | Division          |
| `Enter` / `=` | Calculate         |
| `.`           | Decimal point     |
| `Backspace`   | Delete last digit |
| `Escape`      | Clear calculator  |

---

## 🧠 How It Works

The calculator maintains its current state using JavaScript:

```js
const S = {
  current: '0',
  stored: null,
  op: null,
  evaled: false,
  expr: ''
};
```

Arithmetic operations are processed through a dedicated calculation function:

```js
function calculate(a, op, b) {
  a = parseFloat(a);
  b = parseFloat(b);

  if (op === '+') return a + b;
  if (op === '-') return a - b;
  if (op === '*') return a * b;
  if (op === '/') return b === 0 ? NaN : a / b;

  return b;
}
```

The application also handles invalid results and displays `Error` when necessary.

---

## 🎨 Theme System

The calculator supports two themes:

### 🌙 Dark Mode

A dark interface designed for comfortable use in low-light environments.

### ☀️ Light Mode

A brighter interface for users who prefer a traditional light UI.

The theme can be switched instantly using the built-in toggle.

---

## 💫 UI & Interaction

The interface includes several small interaction details to make the calculator feel more polished:

* Button press animation
* Ripple effect
* RGB flash effect
* Hover states
* Smooth theme transition
* Dynamic result font sizing
* Animated calculator entrance

These details are implemented with CSS animations and JavaScript event handling.

---

## 📁 Project Structure

```text
basic-calculator/
│
├── index.html
└── README.md
```

The project is intentionally lightweight and does not require a build tool or package installation.

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Navigate to the Project

```bash
cd basic-calculator
```

### Run the Project

Open `index.html` directly in your browser.

No additional dependencies or installation steps are required.

---

## 🔢 Supported Operations

```text
Addition        +
Subtraction     −
Multiplication  ×
Division        ÷
Percentage      %
Positive/Negative +/−
Decimal         .
```

---

## ⚠️ Error Handling

The calculator prevents invalid division results such as:

```text
10 ÷ 0
```

Instead of returning an invalid numeric result, the display shows:

```text
Error
```

The calculator can then be reset using the `AC` button.

---

## 🌱 Future Improvements

Possible improvements for future versions:

* [ ] Calculation history
* [ ] Scientific calculator mode
* [ ] Memory buttons (`M+`, `M−`, `MR`, `MC`)
* [ ] Improved mobile layout
* [ ] Sound feedback
* [ ] LocalStorage for calculation history
* [ ] Custom themes
* [ ] Copy result button

---

## 👨‍💻 Author

### RS Arafath

**Junior Web Developer | Front-End & MERN Stack Developer**

* 🌐 Portfolio: `YOUR_PORTFOLIO_URL`
* 💼 LinkedIn: `YOUR_LINKEDIN_URL`
* 🐙 GitHub: `YOUR_GITHUB_URL`

---

## ⭐ Support

If you found this project useful or interesting, consider giving it a ⭐ on GitHub.

---

<p align="center">
  Made with ❤️ by <strong>RS Arafath</strong>
</p>
