# Performance Appraisal Calc

A beautifully designed, client-side single-page application built to streamline and calculate employee performance evaluations, budget projections, compensation hikes, and HR communication.

<a href="https://16th-psyche.github.io/Appraisal-Calculator/">Appraisal Calculator</a>

## 🚀 Features

- **Role-Based Presets:** Automatically pre-fills standard weightage distributions for different corporate hierarchies (L1 Junior Execs through L4 Senior Managers) while fully supporting custom overrides.
- **Dynamic Evaluation Matrix:** Add, remove, and customize unlimited "Area of Focus" metrics to perfectly tailor the appraisal criteria to individual associates.
- **Real-Time Financial Projections:** Instantly calculates monthly/annual appraisal budgets, percentage achievements, and final forecasted salaries as you type.
- **Automated HR Email Draft:** As you input data, the app dynamically generates a completely formatted HR email draft containing all necessary details (including updated CTC and effective dates).
- **1-Click Clipboard Copy:** Strip HTML formatting and copy the generated plain-text HR email straight to your clipboard for instant pasting into your email client.
- **Browser Print to PDF:** Uses the browser's native print dialog for clean, reliable PDF export with print-optimized spacing, visibility, and layout.
- **Automated Data Persistence:** Automatically saves all configurations, inputs, and edits to the browser's native `localStorage` on every keystroke. Your data survives accidental tab closures and browser restarts.

## 💻 Installation & Usage

Because the primary logic operates completely local to the browser window, getting started takes literally two seconds:

1. Clone or download the repository to your local machine:
   ```bash
   git clone https://github.com/16th-psyche/appraisal-calculator.git
   ```
2. Double-click the `index.html` file (or use a local server like Live Server) to launch the application.
3. Start entering your associate's profile, dates, and achieved scores. The system will handle all complex math, caching, and formatting (enforcing the Indian Numbering System where required).

## 🖨️ Exporting to PDF & Emailing HR

To execute a finalized appraisal and send records:
1. Ensure all calculations are settled and dates are filled in.
2. Click **Print / Save as PDF** at the top of the dashboard, or press `Command + P`, to open the browser's native print dialog.
3. Scroll down to the **HR Email Draft** section and click **Copy to Clipboard**. 
4. Save the print output as a PDF from the browser dialog, then paste the email text into your email client, attach the PDF, and send it to HR.

## 🧹 Resetting the Dashboard

If you need to wipe out the stored local memory cache and begin a fresh evaluation for a different associate, execute the **Clear & Start Over** command located in the top right corner of the dashboard. This instantly clears the database, resets dates, and restores the matrix back to the L1 baseline.

## 🛠️ Architecture & Dependencies
- **HTML5 & CSS3:** Semantic structure, heavy utilization of Flexbox systems, and responsive layouts.
- **ES6 JavaScript:** Modular, client-side mathematics handler managing DOM state integration and localized `localStorage` serialization.
- **Browser Print CSS:** Uses `@media print` rules to produce a clean print/PDF layout directly from the browser.
