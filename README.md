# Visualizing Housing Market Trends: An Analysis of Sale Prices and Features using Tableau

![Project Banner](https://via.placeholder.com/1200x400?text=Tableau+Housing+Market+Dashboard)

*(Replace the above image link with an actual screenshot of your Tableau dashboard or the hero section of your web app.)*

---

## Project Overview

This project analyzes key factors influencing house sale prices and market trends using real estate data. The analysis focuses on:

- Impact of **renovations** on sale prices  
- **House age distribution** and renovation status  
- Relationship between **bedrooms, bathrooms, floors**, and house age  
- **Overall dataset summary** including total records, average price, and basement area  

The insights are presented through an **interactive Tableau dashboard embedded inside a Flask web application**, allowing users to explore visualizations directly in a web browser.

**Goal:**  
Provide actionable insights for **real estate analysts, marketing teams, and executives** to optimize pricing strategies and better understand market competitiveness.

---

## Features

- Interactive **Tableau Story** with **4 main visualization scenarios**
- **Responsive Bootstrap-based web interface**
- Embedded **live Tableau dashboard**
- Clean project structure suitable for **GitHub portfolio projects**
- Easy to deploy and share online

---

## Technology Stack

| Technology | Purpose |
|-----------|---------|
| Tableau | Data visualization & dashboard creation |
| Tableau Public | Hosting & embedding dashboards |
| Python + Flask | Lightweight backend server |
| HTML5 + Bootstrap 5 | Responsive frontend UI |
| CSS | Custom styling |

---

## Dataset

The project uses a housing dataset containing important real estate attributes:

**Main Fields**

- `price` – Sale price of the house  
- `bedrooms` – Number of bedrooms  
- `bathrooms` – Number of bathrooms  
- `floors` – Number of floors  
- `yr_built` – Year the house was built  
- `yr_renovated` – Year the house was renovated  
- `sqft_basement` – Basement size in square feet  

**Derived Fields (Calculated in Tableau)**

- `house_age`
- `years_since_renovation`
- `renovation_status`
- `age_group`
- `price_bin`

**Common Dataset Source**

King County House Sales dataset (Kaggle or similar housing market datasets).

---

## Tableau Dashboard Scenarios

### 1. Overall Data Overview
Displays key performance indicators such as:

- Total housing records  
- Average sale price  
- Total basement square footage  

Provides a quick snapshot of the dataset.

---

### 2. Total Sales by Years Since Renovation

A **histogram visualization** showing how sale prices are distributed based on how recently houses were renovated.

Insight:
Recently renovated homes may sell at **higher price ranges**.

---

### 3. Distribution of House Age by Renovation Status

A **pie chart** representing:

- Different **house age groups**
- Proportion of **renovated vs non-renovated homes**

Insight:
Helps understand **renovation trends across housing age categories**.

---

### 4. House Age Distribution by Bathrooms, Bedrooms, and Floors

A **grouped bar chart** showing relationships between:

- House age
- Number of bathrooms
- Number of bedrooms
- Number of floors

Insight:
Newer houses often include **modern layouts and additional floors**.

---

## Project Structure

```
housing-market-trends-tableau/
│
├── app.py                 # Flask application
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
│
└── templates/
    └── index.html         # Main webpage containing Tableau embed
```

### Optional Folders

```
static/    # CSS, images
data/      # CSV datasets (not required for running the project)
```

---

## Installation & Setup

### Prerequisites

- Python **3.8+**
- Git (optional)
- Tableau Public account

---

## Step 1: Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/housing-market-trends-tableau.git
cd housing-market-trends-tableau
```

---

## Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

Main dependency:

```
Flask
```

---

## Step 3: Update Tableau Embed URL

Open the following file:

```
templates/index.html
```

Replace the iframe source with your Tableau Public dashboard link.

Example:

```html
<iframe 
  src="https://public.tableau.com/views/YourVizName/Dashboard1?:embed=y&:display_count=no&:showVizHome=no"
  width="100%"
  height="900px"
  frameborder="0"
  allowfullscreen>
</iframe>
```

---

## Step 4: Run the Flask Application

```bash
python app.py
```

---

## Step 5: Open in Browser

Visit the following URL:

```
http://127.0.0.1:5000
```

The webpage will display your **embedded Tableau dashboard**.

---

# How to Get Your Tableau Embed Link

1. Publish your **Tableau workbook or story** to Tableau Public  
2. Open the published dashboard  
3. Click **Share → Embed Code**  
4. Copy the **iframe `src` URL**  
5. Paste it inside **index.html**

---

# Screenshots

(Add screenshots after running the project)

- Dashboard Overview  
- Renovation Histogram  
- House Age & Renovation Pie Chart  
- Features by Age Bar Chart  

---

# Team / Credits

## Project Lead / Developer
Krashika Raikwar

## Team Members

- Lokesh Choudhary  
- Krati Thakur  
- Manish Barman  

## Project Context

Academic / Real Estate Data Analysis Project

---

# License

MIT License

You are free to **use, modify, and distribute** this project.

---

# Acknowledgments

- Tableau Public for free dashboard hosting  
- BootstrapMade (Dewi Template) for UI inspiration  
- Flask for lightweight backend development  
- Kaggle Community for providing housing datasets  

---

# Tableau Public Dashboard

```
https://public.tableau.com/views/VisualizingHousingMarketTrends_AnAnalysisofSalePricesandFeaturesusingTableau/
```

---

# Happy Exploring Housing Trends 🏠📊

