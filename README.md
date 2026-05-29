# CyberBot — Part 2

An optimized, professional-grade interactive WPF security chatbot application designed to demonstrate robust Object-Oriented Programming (OOP) practices, efficient data structure utilization, and strict Separation of Concerns.

## 🛠️ Architectural Highlights

- **Separation of Concerns (Decoupling):** The presentation layer (`MainWindow.xaml`) is entirely separated from the underlying conversational business logic. 
- **Type-Safe Delegate Pipeline:** Communication between the UI and the backend engine is managed through a secure `ChatProcessor` delegate pipeline, avoiding hard dependencies.
- **State Preservation:** The core execution instance is persistent across form states, ensuring conversational context values stay intact.

---

## 📋 Implemented Features 

### 1. Memory and Recall
The chatbot actively tracks user interests throughout the session using a state tracker (`favoriteTopic`). Keywords like *“interested in privacy”* flag state properties in the background, allowing the system to personalize subsequent security recommendations dynamically.

### 2. Sentiment Detection
The engine evaluates the user's emotional state by parsing high-impact triggers (`worried`, `frustrated`, `curious`). Upon detection, it prepends an empathetic, context-aware prefix string immediately followed by the relevant technical tip—delivering seamless, uninterrupted UX without demanding re-input.

### 3. Error Handling & Edge Cases
- **Null Guards:** Strings are validated instantly via white-space fallback checks to suppress structural failure exceptions.
- **Fail-Safe Fallback:** The default branch acts as an all-inclusive boundary that handles unrecognized keywords gracefully without breaking application execution state.

### 4. Code Optimisation & Data Structures
- **Generic Collections:** Utilizes high-performance `Dictionary<string, string>` and `List<string>` maps for optimized lookup times instead of messy hardcoded chains.
- **Pattern-Matching Switch:** Implements localized conditional pattern evaluations (`case string s when...`) to execute highly granular context evaluation cleanly.

---

## 🚀 How to Run the Project

1. Clone or download the repository solution.
2. Open the solution file (`.sln`) inside **Visual Studio**.
3. Rebuild the solution (`Ctrl + Shift + B`) to verify references clear perfectly.
4. Press **F5** or hit **Start** to initialize the interactive terminal console.

---

## 🎥 YouTube Explanation Video Outline
*A walk-through video explaining the implementation architecture is structured into the following sections:*
- **Part 1:** Visual Demonstration of XAML Text Wrapping and Font Scaling.
- **Part 2:** Code-Behind Deconstruction (The Delegate and Form Isolation).
- **Part 3:** Backend Architecture (The Switch Matrix, Dictionary Loops, State Persistence).
