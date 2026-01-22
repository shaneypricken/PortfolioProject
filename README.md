# Guitar Chord Trainer 🎸

A lightweight, interactive application built with **Processing (Java)** designed to help beginners visualize and memorize common guitar chords. The app draws a virtual fretboard and indicates finger positions for a variety of open and barre chords.

## ✨ Features

*   **Fretboard Visualization:** Procedurally drawn guitar neck with varying string gauges (thicknesses) to distinguish low and high strings.
*   **Chord Library:** Includes 16 essential chords:
    *   **Major:** A, C, D, E, F, G
    *   **Minor:** Am, Dm, Em
    *   **7ths:** A7, B7, C7, D7, E7, G7, Fmaj7
*   **Practice Mode:**
    *   **Randomize:** Instantly switch to a random chord to test your recall speed.
    *   **Visual Indicators:** Clearly marks finger positions (black dots) and open strings (hollow circles).
*   **GUI System:** Custom-built button class with hover effects and active states.
*   **Navigation:** Functional Main Menu, Practice Screen, and Settings placeholders.

## 🚀 Getting Started

### Prerequisites

You need the **Processing IDE** to run this sketch.
1.  Download and install Processing from [processing.org](https://processing.org/download).

### Installation & Run

1.  Clone this repository or download the ZIP file.
2.  Open the folder.
3.  Double-click the `.pde` file to open it in the Processing IDE.
4.  Press the **Play** button (▶) in the top left corner to launch the application.

## 🕹️ Controls

*   **Mouse:** Use the mouse to interact with the UI buttons on the left panel.
*   **Randomize:** Click to cycle to a random chord shape from the library.
*   **Play Chord:** Currently prints the chord name to the console (audio integration planned).
*   **Navigation:** Use "Main Menu" or "Settings" to switch screens.

## 🧠 How It Works

The project uses a 3D integer array to store chord shapes. This allows for easy expansion of the chord library without modifying the drawing logic.

**Data Structure:**
```java
// Format: { {String_Index, Fret_Number}, ... }
// String Index: 0 (Low E) to 5 (High E)
int[][][] chordShapes = {
  { {2,2}, {3,2}, {4,2} },     // A Major
  { {1,3}, {2,2}, {4,1} },     // C Major
  // ...
};
