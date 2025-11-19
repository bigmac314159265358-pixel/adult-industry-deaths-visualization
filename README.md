# 📊 Adult Industry Deaths Analysis Dashboard

This project is an interactive data visualization tool built primarily using an **AI Chatbot (Google Gemini; Pro Version as of November 19, 2025)**. The front-end utilizes Chart.js, Tailwind CSS, and vanilla JavaScript. It is designed to provide clear insights into the distribution and timeline of recorded deaths, with a unique filtering mechanism for redistributing ambiguous data points.

## ✨ Features

This single-page application (`index.html`) provides a powerful and customizable view of the dataset:

* **Interactive Filtering:** Filter records by a **multi-select Cause dropdown** and a **Year Range selector** (with an easy-to-use year picker).
* **Total Count Accuracy:** The total record count updates instantly and accurately based on all applied filters and chart interactions.
* **Dynamic Charting:** Switch between four visualization modes for the main panel:
    * **Doughnut Chart** (with center total count)
    * **Stacked Bar Chart** (Timeline)
    * **Horizontal Bar Chart** (Ranking)
    * **Polar Area Chart**
* **Timeline Scatter Plot:** A dedicated chart visually plotting individual deaths over time, categorized vertically by cause.

### 🔬 Unique Feature: Customize Unknowns

The dashboard includes a dedicated **"Customize Unknowns"** feature that allows the user to dynamically handle ambiguity in the data:

* Users can select two concrete categories (e.g., "Suicide" and "Medical").
* A slider lets the user split the counts from the **"Unknown"** and **"Unsure"** categories between the two selected categories (e.g., 70% to Suicide, 30% to Medical).
* When applied, the charts and filtered data are instantly re-rendered to reflect this hypothetical distribution, providing a powerful tool for sensitivity analysis.

***

## 🚀 Getting Started

Since this project is a single, self-contained HTML file, no server or complex setup is required.

### Viewing Online (Recommended)

This dashboard is deployed using GitHub Pages and can be accessed directly at:

**`[Insert GitHub Pages URL Here]`**

*(e.g., `https://yourusername.github.io/repository-name/`)*

### Running Locally

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yourusername/your-repository-name.git](https://github.com/yourusername/your-repository-name.git)
    ```
2.  **Open the File:** Navigate to the cloned folder and simply **double-click** the `index.html` file. It will open directly in your web browser.

***

## 🛠️ Technical Details

| Technology | Purpose |
| :--- | :--- |
| **HTML** | Structure and main container. |
| **Tailwind CSS** | Styling and rapid UI development. |
| **JavaScript (Vanilla)** | All core logic, filtering, and chart rendering. |
| **Chart.js v4** | Primary charting library for dynamic visualizations. |
| **Moment.js & Adapter** | Handling time series data in the timeline chart. |

The application's data is currently **embedded within the JavaScript** section of the `index.html` file. To update the dataset, simply replace the content of the `window.rawData = [...]` array within the script tags.
