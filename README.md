# Airbnb Open Data – Exploratory Data Analysis

A simple data analysis mini-project on the **Airbnb Open Data** (NYC listings).
This was made as part of my data analysis coursework using Python, Pandas,
Matplotlib and Seaborn.

---

## 📌 Project Goal

To clean the Airbnb dataset and explore it visually to answer questions like:

- Which neighbourhood group has the most listings?
- What is the average price in each area?
- Which room types are most common?
- How are reviews and prices related?

---

## 📁 Project Structure

```
Event_Data_Analysis_Project/
│
├── Airbnb_Open_Data.xlsx      # Original dataset
├── airbnb_eda.py              # Main analysis script
├── airbnb_cleaned.csv         # Cleaned dataset (created after running)
├── requirements.txt           # Python libraries needed
├── index.html                 # Project website
├── style.css                  # Website styling
├── images/                    # Charts created by the script
└── README.md
```

---

## ⚙️ How to Run

1. Clone this repository
   ```bash
   git clone https://github.com/ParvathyM155/Event_Data_Analysis_Project.git
   cd Event_Data_Analysis_Project
   ```

2. Install the required libraries
   ```bash
   pip install -r requirements.txt
   ```

3. Run the analysis script
   ```bash
   python airbnb_eda.py
   ```

4. Open `images/` to see the generated charts, or open `index.html`
   in a browser to view the project website.

---

## 🧹 Data Cleaning Steps

- Renamed columns to lowercase with underscores
- Fixed typos in `neighbourhood_group` (`brookln` → `Brooklyn`,
  `manhatan` → `Manhattan`)
- Dropped the almost-empty `license` column
- Removed duplicate rows
- Removed rows missing important fields (`price`, `room_type`, etc.)
- Filtered out unrealistic values (price ≤ 0, minimum nights > 365, etc.)

---

## 📊 Charts Generated

| File | What it shows |
|------|---------------|
| `listings_by_group.png` | Number of listings per neighbourhood group |
| `room_type_distribution.png` | How common each room type is |
| `avg_price_by_group.png` | Average price in each neighbourhood group |
| `price_distribution.png` | Overall distribution of prices |
| `price_by_room_type.png` | Price comparison across room types |
| `top10_neighbourhoods.png` | Top 10 neighbourhoods by number of listings |
| `reviews_vs_price.png` | Relationship between reviews and price |
| `heatmap.png` | Correlation heatmap of numeric columns |

---

## 🌐 Website

A simple HTML/CSS page (`index.html`) is included to present the project.
You can host it for free using **GitHub Pages**:

1. Push the project to GitHub
2. Go to **Settings → Pages**
3. Under *Source*, choose `main` branch and `/root`
4. Save — your site will be live at
   `https://<your-username>.github.io/Event_Data_Analysis_Project/`

---

## 🛠️ Tools Used

- Python 3
- Pandas
- Matplotlib
- Seaborn
- Jupyter / Google Colab (for early exploration)

---

## 👩‍🎓 Author

**Parvathy M**

Data Analysis Mini Project
