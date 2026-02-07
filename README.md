# 5 Clues 🕵️‍♂️

**Five Clues** is a fast-paced, "Reverse Taboo" style browser game. Players must guess a hidden entity (Person, Place, Thing, or Concept) based on exactly five keyword clues.

Built with a "Mobile-First" approach, it features a sleek Neon/Dark Mode aesthetic, 60fps animations, and distinct game modes for solo or party play.

## 🎮 Game Modes

### 1. Solo Rush 👤

* **Objective:** Score as high as possible before you are eliminated.
* **Rules:** You start with **3 Lives** ❤️.
* **Scoring:** Base points + Time bonus.
* **Lose Condition:** Running out of time or clicking "Missed It" costs 1 Life.

### 2. Party War (Teams) 👥

* **Objective:** "Pass and Play" mode for groups.
* **Teams:** Team Blue 🔵 vs. Team Red 🔴.
* **Flow:** The game prompts players to pass the device between turns.
* **Winning:** The team with the highest score after 5 rounds wins.

---

## ✨ Key Features

* **📱 Native App Feel:** Uses `dvh` (Dynamic Viewport Height) and `touch-action` manipulation to feel like a native mobile app on iOS and Android.
* **🎨 Neon Dark UI:** High-contrast dark mode design to reduce eye strain and make gameplay pop.
* **⚡ Zero Dependencies:** Built entirely in Vanilla JavaScript, HTML5, and CSS3. No frameworks, no build steps.
* **⚙️ Configurable Difficulty:** Filter cards by "Easy", "Medium", or "Hard".
* **🧱 Modular Architecture:** Strict separation of Data (`data.js`), Logic (`script.js`), and Styling (`styles.css`).

---

## 🚀 Getting Started

Since this is a static web application, no installation (`npm install`) is required.

### Prerequisites

* A modern web browser (Chrome, Safari, Firefox, Edge).

### Installation

1. **Clone the repository** (or download the files):
```bash
git clone https://github.com/yourusername/five-clues.git

```


2. **Navigate to the folder:**
```bash
cd five-clues

```


3. **Run the game:**
* Simply double-click `index.html` to open it in your browser.
* *Tip:* For the best mobile experience, serve it over a local network (e.g., using VS Code "Live Server") and open the IP on your phone.



---

## 📂 Project Structure

```text
/five-clues
│
├── index.html      # Main entry point (HTML Structure)
├── styles.css      # Neon Theme & Responsive Layout
├── script.js       # Game Engine & UI Controller
├── data.js         # JSON Data Source (The Questions)
└── README.md       # Documentation

```

---

## 🛠️ Customization

You can easily add your own cards by editing the `data.js` file. The game automatically loads whatever is in this array.

**Data Schema:**

```javascript
{
  "name": "Target Answer",      // The answer the player must guess
  "hint": "A short hint",       // Displayed on the answer card
  "category": "General",        // Category label
  "country": "Global",          // Origin (Optional)
  "words": [                    // MUST contain exactly 5 strings
    "Clue 1", 
    "Clue 2", 
    "Clue 3", 
    "Clue 4", 
    "Clue 5"
  ],
  "difficulty": "Easy"          // "Easy", "Medium", or "Hard"
}

```

---

## 💻 Tech Stack details

* **HTML5:** Semantic structure with strict viewport meta tags for mobile scaling prevention.
* **CSS3:** Uses CSS Variables (`:root`) for theming, Flexbox for layout, and hardware-accelerated transitions.
* **JavaScript (ES6):**
* **Game Loop:** `requestAnimationFrame` friendly logic.
* **State Management:** Object-oriented `app` controller.
* **Event Handling:** Passive event listeners for performance.



---

## 🤝 Contributing

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---

*Made with ❤️ for Game Night.*
