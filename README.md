# 🚖 Uber Trip Analysis Dashboard (Power BI)

An interactive and comprehensive Power BI business intelligence dashboard developed to analyze Uber ride bookings, revenue trends, passenger behavior, fleet demand, and granular trip metrics[cite: 1, 5, 6].

---

## 📌 Project Overview
This project processes raw transactional trip records to identify peak demand windows, route efficiencies, vehicle category preferences, and location-based trip density[cite: 1, 5, 6]. The dashboard provides key operational KPIs alongside drill-down capabilities for granular ride auditing[cite: 5, 6].

---

## 📊 Dashboard Views & Pages

### 1. Overview Analysis
* **High-Level KPIs:** Displays core performance metrics including Total Bookings (103.7K), Total Booking Value ($1.6M), Avg Booking Value ($15.0), Total Distance Traveled (349K Miles), Avg Distance (3 Miles), and Avg Trip Time (16 Min)[cite: 5].
* **Filter Capabilities:** Date range picker and City drop-down slicer for tailored analysis[cite: 5].
* **Visual Cards & Distribution:** Booking breakdowns by pickup trends and vehicle categories[cite: 3, 5].

### 2. Time Analysis
* **Total Booking By Pickup Time:** Hourly line chart illustrating continuous rider demand fluctuations throughout the 24-hour cycle[cite: 5].
* **Total Booking By Day Name:** Day-wise trend showing weekly volume distributions (e.g., commute patterns vs. weekend surges)[cite: 5].
* **Total Booking By Day & Hour (Heatmap Matrix):** Granular matrix covering Monday through Sunday across all 24 hours to pinpoint peak fleet operational hours[cite: 5].

### 3. Details View (Granular Data Table)
* Tabular view allowing full row-level audit of completed bookings[cite: 6].
* **Captured Fields:** `Trip ID`, `Pickup Date`, `Pickup Hour`, `Vehicle`, `Payment_type`, `No of Passengers`, `Trip Distance`, `Total Booking`, and `Location`[cite: 6].

---

## 🗃️ Data Dictionary

### Trip Details
| Field Name | Description |
| :--- | :--- |
| **Trip ID** | Unique identifier assigned to each Uber trip[cite: 1, 6]. |
| **Pickup Date / Time** | Exact date and timestamp when the trip commenced[cite: 1, 6]. |
| **Drop Off Time** | Exact timestamp when the passenger was dropped off[cite: 1]. |
| **Passenger Count / No of Passengers** | Headcount of riders accommodated in the vehicle[cite: 1, 6]. |
| **Trip Distance** | Total road distance traveled in miles[cite: 1, 6]. |
| **Vehicle** | Uber service category booked (UberX, UberXL, Uber Comfort, Uber Green, Uber Black)[cite: 1, 6]. |
| **Payment Type** | Transaction method used (Cash, Uber Pay, Credit Card)[cite: 1, 6]. |
| **Fare Amount / Total Booking** | Base fare and gross revenue charged per completed ride[cite: 1, 6]. |
| **Surge Fee** | Additional premium charged during high-demand windows[cite: 1]. |
| **PULocationID / DOLocationID** | Numeric identifiers linked to pickup and drop-off reference tables[cite: 1]. |

### Location Table
| Field Name | Description |
| :--- | :--- |
| **LocationID** | Primary key mapping numerical codes to physical locations[cite: 1, 2]. |
| **Location** | Name of the neighborhood or landmark (e.g., Central Park, Midtown North, Flatiron)[cite: 2, 6]. |
| **City** | City name used for geographic segmentation[cite: 2]. |

---

## 🛠️ Built With
* **Tool:** Microsoft Power BI Desktop[cite: 4]
* **Techniques Used:** Data Modeling, DAX Measures, Bookmarks & Selection Panels for dynamic popups/navigation, Heatmap Visualizations, Interactive Slicers[cite: 4, 5, 6]

---

## 🚀 How to Use & View
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/uber-trip-analysis.git](https://github.com/your-username/uber-trip-analysis.git)
