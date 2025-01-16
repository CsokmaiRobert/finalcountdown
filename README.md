# ⏱ React Timer Challenge App

This React app challenges players to stop a timer as close as possible to predefined target times. It offers multiple difficulty levels and includes features to track player names, display scores, and provide feedback via a modal.

---

## **Features:**
- **Player Name Input:** Allows users to input and display their name for a personalized experience.
- **Multiple Challenges:** Includes timers with different target times (e.g., 1, 5, 10, and 15 seconds) for increasing difficulty.
- **Dynamic Timer Control:** Users can start and stop the timer, aiming to match the target time as closely as possible.
- **Score Calculation:** Provides feedback on how accurately the user stopped the timer compared to the target time.
- **Result Modal:** Displays the player's score or indicates if they lost, along with the target and remaining time.
- **Portal-Based Modal:** The result modal is implemented using React portals for clean separation from the main DOM tree.

---

## **How It Works:**
1. **Player Component:** Users can input their name, which is displayed on the app.
2. **Timer Challenge Component:** Displays the target time for the challenge. Users start the timer, and when they stop it:
   - If the timer runs out, they lose.
   - If stopped early, a score is calculated based on the remaining time.
3. **Result Modal Component:** Shows detailed results, including the target time, remaining time, and score, and provides a reset option.
4. **Reusable Modal:** Implements `useImperativeHandle` and React portals for a flexible, forward-ref modal design.

---

## **Tech Stack:**
- **React:** For the app's component-based structure.
- **Hooks:** Uses `useState`, `useRef`, and `useImperativeHandle` for state management and custom modal behavior.
- **React Portals:** To create a reusable modal component that renders outside the root DOM hierarchy.

---

## **How to Run:**
1. Clone or download the repository containing the project files.
2. Ensure the following files are structured correctly:
   - `App.jsx`: The main entry point for the app.
   - `Player.jsx`: Handles player name input and display.
   - `TimerChallenge.jsx`: Displays each timer challenge with start/stop functionality.
   - `ResultModal.jsx`: Displays results after each challenge attempt.
3. Run the app locally:
   - Install required dependencies: `npm install`.
   - Start the development server: `npm start`.
4. Interact with the app:
   - Enter your name and try to match the target times across multiple challenges.
   - View results in the modal after stopping the timer.

---

## **Live Demo:**
Experience the Timer Challenge App live: [Final Countdown React App](https://finalcountdown-rc.netlify.app)

---

## **Dependencies:**
- React and React DOM: Core libraries for building the app.
- Node.js and npm: To manage dependencies and run the development server.

---

This Timer Challenge App combines fun gameplay with technical features like React hooks and portals, offering an engaging and responsive user experience. 🚀🎮

