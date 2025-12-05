# TypePunk - Cyberpunk Speed Racer ⌨️⚡

# 

**Vibe Coding Assignment - Category 4: Interaction Heavy**

TypePunk is a retro-futuristic typing speed test that transforms mundane typing practice into a high-stakes cyberpunk hacking simulation. It features real-time WPM tracking, visual feedback for accuracy, and persistent local high scores.

## 🚀 Live Demo

# 

https://gemini.google.com/share/747f22717fcf

## ✨ Features

# 

*   **Real-time WPM & Accuracy Engine**: Calculates speed and precision instantly as you type.
    
*   **Visual Feedback System**:
    
    *   Green/Cyan highlighting for correct characters.
        
    *   Red background & Screen Shake effects for errors.
        
    *   Dynamic WPM progress bar.
        
*   **Persistence**: High scores are saved to the browser's LocalStorage.
    
*   **Intentional Design**: Cyberpunk aesthetic with neon gradients, monospace typography, and glassmorphism UI.
    
*   **Mobile Responsive**: Fully functional on touch devices with virtual keyboards.
    

## 🛠 Tools Used

# 

*   **Bolt.new**: Used for the initial scaffolding and Tailwind configuration.
    
*   **Claude 3.5 Sonnet**: Used to refine the WPM calculation logic and generate cyberpunk-themed quotes.
    
*   **React + Tailwind CSS**: The core stack for component-based UI and rapid styling.
    
*   **Lucide React**: For lightweight, consistent iconography.
    

## 🤖 Prompts That Worked

# 

> "Act as a Senior Frontend Dev. Build a typing speed test app with a cyberpunk aesthetic. Use Tailwind CSS for styling. The app needs to track WPM and accuracy in real-time. Store high scores in localStorage. Make the screen shake slightly when the user makes a typo."

**Why it worked:** Giving a specific "vibe" (cyberpunk) and specific "interaction details" (screen shake on error) prevented the AI from generating a generic white-background typing test.

## 🐛 Challenges & Learnings

# 

*   **Challenge:** The initial WPM calculation was jumpy because it calculated based on every keystroke interval.
    
*   **Fix:** Switched to a formula based on `(total_chars / 5) / time_elapsed_minutes` which smoothed out the number.
    
*   **Surprise:** How easy it was to implement the "screen shake" effect using a simple Tailwind conditional class (`translate-x-1`) triggered by React state.
    

## 📦 Setup Instructions

# 

1.  Clone the repo
    
2.  Run `npm install`
    
3.  Run `npm run dev`
    
4.  Open `http://localhost:5173`
    

## ⚠️ Known Limitations

# 

*   The cursor is currently a static blinking line at the end of the text string; moving the cursor back to edit previous mistakes is not fully supported in this version (Arcade mode style).
    

*Built for the Vibe Coding Assignment 2025*