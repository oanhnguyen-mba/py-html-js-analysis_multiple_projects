# GenAI Multi-Project Investment Decision Support Tool

This web-based tool supports decision-making for multiple Generative AI (GenAI) projects by enabling users to input data for up to three projects simultaneously and instantly receive comparative prioritization analysis. The interface features intuitive icons and interactive elements for real-time user engagement. 

Live demo:
👉[GenAI Investment Decision Support](https://oanhnguyen-mba.github.io/py-html-js-analysis_multiple_projects/)

## Abstract
With the rapid emergence of Generative AI technologies, organizations face challenges in allocating limited resources across competing projects. This tool facilitates evaluation and prioritization of multiple GenAI investment projects by calculating key financial metrics—ROI, Payback Period, NPV, IRR—and mapping projects on a value-feasibility matrix. It helps decision-makers identify which projects to start immediately, consider later, or deprioritize.

## Methodology
- **Data Input:** Users enter project-specific data including investment cost, annual savings, detailed cash flows over six years, and subjective business value and feasibility scores (on a 1-10 scale).
- **Real-time Updates:** Users can freely change input numbers in the form fields. Upon any change, the analysis results refresh instantly on the page without the need for manual reload or submit.
- **Financial Calculations:** 
  - ROI (Return on Investment)
  - PBP (Payback Period)
  - NPV (Net Present Value) using a 10% discount rate
  - IRR (Internal Rate of Return) calculated via iterative numeric method
- **Decision Matrix:** Projects are plotted on a two-dimensional scatter plot with axes for feasibility and value scores, divided into four quadrants to highlight investment priority:
  - Quadrant 1 (High Value, High Feasibility): Start Now
  - Quadrant 2 (Low Value, High Feasibility): Easy Wins
  - Quadrant 3 (Low Value, Low Feasibility): Low Priority
  - Quadrant 4 (High Value, Low Feasibility): Consider Later
- **Recommendations:** Based on combined financial thresholds (ROI > 10%, PBP ≤ 5 years, IRR > 10%) and quadrant positioning, tailored investment suggestions are generated.

## Requirements
- Modern web browser with JavaScript enabled.
- Internet connection to load external libraries (Chart.js, jsPDF, html2canvas).
- (Optional) Python environment only if you want to modify or generate the HTML file programmatically.

## Libraries Used
- [Chart.js](https://www.chartjs.org/) — for interactive scatter plot visualization of project scores.
- [jsPDF](https://github.com/parallax/jsPDF) — to generate downloadable PDF reports summarizing analysis results.
- [html2canvas](https://html2canvas.hertzen.com/) — to capture the matrix visualization as an image inside the PDF.

## Results
- Displays computed ROI, Payback Period, NPV, and IRR for each project.
- Provides clear investment recommendations based on financial thresholds and strategic scoring.
- Visual matrix plot categorizes projects into quadrants for intuitive prioritization.
- Users can download a comprehensive PDF report including all analysis details and visualizations.
- **Instant feedback:** Changing any input value refreshes all calculations and charts immediately on the frontend.

## Managerial Implications
- Enables data-driven multi-project investment prioritization for GenAI initiatives.
- Helps stakeholders balance financial returns with strategic feasibility and value considerations.
- Facilitates transparent communication of investment rationale through visual and downloadable reports.
- Supports continuous monitoring and iterative decision-making by allowing updates to project inputs and immediate re-analysis.

---

*This tool is ideal for IT leaders, portfolio managers, and business analysts involved in selecting and managing multiple GenAI projects within constrained budgets.*

