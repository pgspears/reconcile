# Reconciler Pro

**Version:** 3.0  
**Author:** Accelerate Solutions, LLC  
**License:** MIT  

A professional, browser‑based tool for converting QuickBooks exports, aggregating payroll tables, and reconciling cross‑platform payment data — all in one elegant interface.

---

## 🚀 Features

- **Shared Contractor Mapping**  
  Upload a CSV of “Contractor Name” → “Business Name” once, and reuse across all modules.

- **QuickBooks Converter**  
  - Automatically detect and normalize QuickBooks export columns  
  - Fuzzy‑match business names to contractors  
  - Format dates and currency consistently  
  - Generate pivot summaries with detailed drill‑downs  
  - Professional Excel styling (banded rows, custom headers, freeze panes)

- **Payroll Data Aggregator**  
  - Select a named table from one workbook, then add multiple files with the same table  
  - Merge all rows, preserve source‑file provenance  
  - Map provider names to business names via shared mapping  
  - Toggle between raw aggregation and grouped summary views

- **Data Reconciliation**  
  - Compare QuickBooks vs. Payroll totals by business  
  - Highlight missing entries and amount discrepancies beyond a user‑defined threshold  
  - Drill into individual payment details for each source

- **Combined Export**  
  - Bundle all processed sheets (Formatted, Pivot, Aggregate, Summary, Reconciliation) into one Excel workbook  
  - Choose which modules to include  

- **In‑App Preview & Search**  
  - Interactive table viewer with sticky headers, scrollable containers, and discrepancy highlights  
  - Live search/filter on pivot and summary views

- **Help & Troubleshooting**  
  - Built‑in guidance covering common errors, tips, and examples  
  - “Help” tab walks through every step  

---

## 🛠️ Prerequisites

- Modern web browser (Chrome, Firefox, Edge, Safari)  
- No server or build tools required: purely client‑side HTML/JS  

---

## 📥 Installation

1. Clone or download this repository.  
2. Open `index.html` in your browser.  
3. (Optional) Host on a static‑file web server (e.g., GitHub Pages, Nginx).

---

## ⚙️ Usage Guide

### 1. Shared Contractor Mapping  
1. Click **“Upload Contractor Banking Info CSV”** at the top.  
2. Ensure your CSV has columns **Contractor Name** and **Business Name** (case‑insensitive).  
3. Once loaded, you’ll see a “Loaded X mappings” confirmation.

### 2. QuickBooks Converter  
1. Switch to the **QuickBooks Converter** tab.  
2. Upload your QuickBooks export (`.xlsx`/`.xlsm`).  
3. Enter an output file name (e.g., `QB_Report.xlsx`).  
4. (Advanced) Adjust sheet name, fuzzy‑match threshold, and select which columns to include.  
5. Click **Convert QuickBooks Data** — the styled workbook downloads automatically.  
6. Preview formatted data or pivot summary in the in‑app viewer.

### 3. Payroll Data Aggregator  
1. Go to the **Payroll Data** tab.  
2. Upload the primary file and select the named table.  
3. Add one or more files containing the same table.  
4. Click **Export Payroll Data** — an aggregated Excel file downloads.  
5. Preview raw aggregation or summary groups in the app.

### 4. Data Reconciliation  
1. Open the **Reconciliation** tab.  
2. Ensure both QuickBooks and Payroll data have been processed (checkboxes will enable).  
3. Set your match threshold (e.g., `$0.50`).  
4. Click **Analyze Discrepancies**.  
5. View missing entries, amount differences, and detailed drill‑downs.  
6. Export a reconciliation report if desired.

### 5. Combined Export  
1. Head to the **Combined Export** tab.  
2. Check which modules to include in the final workbook.  
3. Provide an output name (e.g., `Combined_Report.xlsx`).  
4. Click **Export Combined File** to download everything in one file.

### 6. Help & Troubleshooting  
- Visit the **Help** tab for step‑by‑step instructions  
- Common issues and fixes (missing columns, table‑not‑found, mapping mismatches)

---

## 🔧 Under the Hood

- **SheetJS with Styling** (`xlsx-js-style`) for client‑side Excel read/write and styling  
- **FuzzySet.js** for in‑browser fuzzy matching of business names  
- Pure vanilla JavaScript, CSS custom properties, and semantic HTML  
- Responsive, accessible UI with sticky table headers and animated tabs  

---

## 🤝 Contributing

1. Fork the repository.  
2. Create a feature branch (`git checkout -b feature/my-feature`).  
3. Commit your changes (`git commit -m 'Add awesome feature'`).  
4. Push to the branch (`git push origin feature/my-feature`).  
5. Open a Pull Request detailing your improvements.

---

## 📄 License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

## 📞 Contact

**Accelerate Solutions, LLC**  
Website: https://acceleratesolutions.io  
Email: support@acceleratesolutions.io  
