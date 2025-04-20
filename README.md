# Photography & Videography Price Analysis

## Overview

This is a web-based tool designed for internal use by photography and videography businesses to quickly and accurately analyze prices for various events and services. It operates from a single HTML file, leveraging modern web technologies for a user-friendly interface.

*(Note: This version uses external libraries loaded via CDN, so an internet connection is required for full functionality.)*

## Features

* **Dynamic Rate Customization:** Adjust cost ranges (Minimum and Maximum) for different personnel and services using intuitive dual-thumb sliders or by direct numerical input. Default rates are provided for common roles.
* **Service Type Management:** Add new types of field workers/services (e.g., Makeup Artist) with their default rate ranges or remove existing ones (excluding core post-production like Editor/Album by default).
* **Multi-Day Event Handling:** Calculate costs accurately for events spanning multiple days. Assign specific quantities of personnel required for each individual day.
* **Post-Production Options:** Include costs for Editor and Album services, with adjustable rates.
* **Miscellaneous Costs:** Add a single overall value for miscellaneous project expenses (travel, rentals, etc.).
* **Flexible Profit Calculation:** Apply a profit margin either as a percentage of the subtotal or as a fixed amount.
* **Real-Time Calculation:** All costs, subtotals, profit amounts, and grand totals update instantly as inputs are changed.
* **Detailed Summary:** View an itemized cost breakdown of all included components.
* **Cost Visualization:**
    * **Doughnut Chart:** Shows the proportion of the Grand Total allocated to major cost categories (individual field workers, post-production, miscellaneous, profit).
    * **Bar Chart:** Compares the Grand Total at different standard profit margins (10%, 15%, 20%, etc.) alongside the total based on the currently selected profit setting.
* **Print Functionality:** Generate a clean, print-friendly summary of the quote using the browser's native print function (`window.print()`). This allows easy saving as a PDF or printing directly. Print styles are included to optimize the layout.
* **Responsive Design:** The layout adapts to various screen sizes, from desktops to mobile devices.
* **Theming:** Uses CSS variables for easy theme adjustments (currently set to a red primary color) and employs the Montserrat font.

## Dependencies

* **Modern Web Browser:** Requires a browser supporting HTML5, CSS3 (Flexbox/Grid), and modern JavaScript.
* **Internet Connection:** Relies on Content Delivery Networks (CDNs) to load the following external libraries:
    * [noUiSlider](https://refreshless.com/nouislider/) (for rate sliders)
    * [Chart.js](https://www.chartjs.org/) (for generating charts)
* **JavaScript:** Core logic is built with Vanilla JavaScript.

## How to Use

1.  **Download:** Obtain the `index.html` file.
2.  **Open:** Open the `index.html` file in a modern web browser. Ensure you have an active internet connection so the external libraries (noUiSlider, Chart.js) can load.
3.  **Configure Rates:**
    * Use the sliders in the "Configuration" column to set the desired Minimum and Maximum rates for each service/worker type.
    * Alternatively, type numerical values directly into the Min/Max input fields next to the sliders.
4.  **Manage Services (Optional):**
    * Click the "+" button to add a new worker/service type, providing a label and default Min/Max rates.
    * Click the "x" button next to a *removable* service type to delete it globally.
5.  **Overall Costs:**
    * Check the boxes for "Editor Needed?" or "Album Needed?" if required. Adjust their rates using their respective sliders/inputs.
    * Enter any overall "Miscellaneous Costs".
6.  **Set Profit:**
    * Select either "Percentage" or "Fixed Amount" for the profit type.
    * Enter the corresponding profit value.
7.  **Daily Breakdown:**
    * Click the "Add Day" button for each day of the event.
    * For each Day card, enter the quantity of each *Field Worker* type needed for that specific day.
    * Click the "x" on a Day card (if more than one exists) to remove it.
8.  **Review Summary:** Observe the real-time updates in the "Quote Summary" column, including the itemized breakdown, totals, and charts.
9.  **Print/Save:** Click the "Print Quote" button. Your browser's print dialog will appear. You can then choose to print directly or use the "Save as PDF" (or similar) option provided by your browser/OS.
