# Performance Appraisal Modeler

A beautifully designed, client-side single-page application built to streamline and calculate employee performance evaluations, budget projections, and compensation hikes. 

<a href="https://16th-psyche.github.io/Appraisal-Calculator/">Appraisal Calculator</a>

## 🚀 Features

- **Role-Based Presets:** Automatically pre-fills standard weightage distributions for different corporate hierarchies (L1 Junior Execs through L4 Senior Managers) while fully supporting custom overrides.
- **Dynamic Evaluation Matrix:** Add, remove, and customize unlimited "Area of Focus" metrics to perfectly tailor the appraisal criteria to individual associates.
- **Real-Time Financial Projections:** Instantly calculates monthly/annual appraisal budgets, percentage achievements, and final forecasted salaries as you type.
- **Automated Data Persistence:** Automatically saves all configurations, inputs, and edits to the browser's native `localStorage` on every keystroke. Your data effortlessly survives accidental tab closures and browser restarts.
- **1-Click PDF Export:** Uses an optimized `@media print` CSS engine to seamlessly convert the interactive dashboard into a clean, minimalist paper report—stripping out buttons, boundaries, and UI clutter natively via your browser's Print pipeline.
- **Zero Dependencies:** Built from the ground up with vanilla HTML/CSS/JS, meaning no heavy frameworks, building tools, or backend servers are required to run it immediately.

## 💻 Installation & Usage

Because the entire application operates completely local to the browser window, getting started takes literally two seconds:

1. Clone or download the repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/appraisal-calculator.git
   ```
2. Double-click the `index.html` file to launch the application directly in your default web browser. *(Google Chrome, Safari, or Microsoft Edge are recommended for perfect PDF translation).*
3. Start entering your associate's profile budget lines and achieved scores. The system will handle all complex math, cache storing, and formatting (enforcing the Indian Numbering System where required).

## 🖨️ Exporting to PDF

To generate and save a finalized record of an appraisal:
1. Ensure all calculations are settled.
2. Click the highly-visible **Export Appraisal Report** button at the top of the dashboard.
3. In your system's native print menu, select **Save as PDF** as the destination. 
   *(Note: For the highest fidelity output, verify that "Background graphics" is enabled in your print settings so the highlight colors translate into the PDF).*
4. Click Save.

## 🧹 Resetting the Dashboard

If you need to wipe out the stored local memory cache and begin a fresh evaluation for a different associate, execute the **Clear & Start Over** command located in the top right corner of the dashboard. This instantly clears the database and safely resets the matrix back to the L1 baseline.

## 🛠️ Architecture
- **HTML5:** Semantic structure.
- **CSS3:** Heavy utilization of Flexbox systems, responsive queries, and `@media print` layout fallbacks.
- **ES6 JavaScript:** Modular, client-side mathematics handler managing DOM state integration and localized serialization.
