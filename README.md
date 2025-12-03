# Mekhava Siri (మేఖవా సిరి) 🌾
### Smart Farming Simulator & Profit Calculator for Mekhava Village

**Mekhava Siri** is an offline-first, single-page web application designed to help farmers in Mekhava village make data-driven decisions. By simulating crop conditions (Soil, Water, Season), farmers can estimate their yield and potential profit before they sow seeds.

## 🚀 Features

* **Bilingual Support:** Fully translated into **Telugu (తెలుగు)** and English for local accessibility.
* **Smart Simulation Engine:** Calculates yield percentage based on real-world logic (e.g., Rice needs clay soil, Mango hates flooding).
* **Visual Feedback:**
    * **Dynamic Plant Growth:** Plant animation grows taller based on yield success.
    * **Cracking Soil Effect:** Visual warning when water levels are too low.
    * **Neon UI:** High-contrast, dark-mode interface for easy reading in sunlight or low light.
* **Profit Calculator:**
    * `Profit = (Base Profit/Acre × Acres Owned) × Yield Efficiency`
    * Visualized using a "Speedometer" gauge.
* **Actionable Advice:** Provides specific tips (Intercropping, Disease Management) based on the selected crop.
* **100% Offline:** No internet connection or database required. Works entirely in the browser.

## 🛠️ How to Use

### On Computer (Windows/Mac/Linux)
1.  Download the `mekhava_final.html` file.
2.  **Double-click** the file.
3.  It will open in your default web browser (Chrome, Edge, Firefox).

### On Mobile (Android/iOS)
1.  Send the `.html` file to your phone (via WhatsApp, Bluetooth, or USB).
2.  Open the file using a browser app (Chrome is recommended).
3.  **Tip:** You can "Add to Home Screen" to make it look like a real app.

## ⚙️ How it Works (The Logic)

The simulator uses a weighted scoring system to calculate results:

1.  **Inputs:** User selects Land Size, Crop, Soil Type, Water Level, and Season.
2.  **Processing:**
    * Each crop has a "Base Profit" per acre.
    * The code checks compatibility. *Example: If `Crop = Rice` AND `Water = Low`, the Yield Score drops by 40%.*
3.  **Output:**
    * **Yield Bar:** Shows percentage (0% to 100%).
    * **Profit:** Calculates total estimated rupee value.
    * **Tips:** Fetches an array of specific advice for that crop.

## 📂 Project Structure

This is a **Single Page Application (SPA)**. All logic, styling, and content are contained in one file for portability.

```text
mekhava-siri/
│
├── mekhava_final.html      # Contains HTML, CSS (Neon Styles), and JS (Logic)
├── README.md               # Project Documentation
└── (Optional) screenshots/ # Images of the app
