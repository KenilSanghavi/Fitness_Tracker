# 💪 Fitness Tracker

A Python-based command-line application to log, analyze, and visualize your daily fitness activities. Built using object-oriented programming with data stored in a CSV file.

---

## 📋 Features

- **Log activities** — Record any activity with duration and calories burned (with validation for negative values)
- **Load data** — Load previously saved activity records from CSV
- **Calculate fitness metrics** — View total calories burned, average session duration, and activity frequency
- **Filter activities** — Filter records by activity type or date range
- **Analyze data** — Get average duration and calories, and total time spent per activity type
- **Visualize data** — Generate 4 types of charts:
  - Bar chart — Time spent per activity
  - Bar chart — Calories burned per day
  - Pie chart — Activity distribution
  - Heatmap — Correlation between duration and calories

---

## 🛠️ Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data storage, filtering, and manipulation |
| `numpy` | Statistical calculations (mean, averages) |
| `matplotlib` | Bar charts, pie charts, line graphs |
| `seaborn` | Heatmap visualization |
| `datetime` | Auto-stamping activity logs with current date |

---

## 📁 Project Structure

```
Fitness_Tracker/
├── fitness_tracker.py     ← Main application (FitnessTracker class)
└── fitness_tracker.csv    ← Activity data storage
```

---

## ⚙️ Installation

**Step 1 — Clone the repository**
```bash
git clone https://github.com/KenilSanghavi/Fitness_Tracker.git
cd Fitness_Tracker
```

**Step 2 — Install required libraries**
```bash
pip install pandas numpy matplotlib seaborn
```

**Step 3 — Run the program**
```bash
python fitness_tracker.py
```

---

## 🚀 Usage

The `FitnessTracker` class provides the following methods:

```python
tracker = FitnessTracker()

# Log a new activity
tracker.log_activity("Running", 30, 300)   # activity, duration (mins), calories

# Load existing data from CSV
tracker.load_data()

# View fitness metrics
tracker.calculate_metrics()

# Filter by activity type
tracker.filter_activities("Running")

# Analyze averages and totals
tracker.analyze()

# Generate all charts
tracker.visualize()

# Print full report
tracker.generate_report()
```

---

## 📊 Sample CSV Format

The data is stored in `fitness_tracker.csv` with the following structure:

```
date,activity type,duration,calories burned
2025-01-15,Running,30,300
2025-01-15,Swimming,45,310
2025-01-16,Cycling,60,450
```

---

## 📈 Visualizations

The `visualize()` method generates 4 charts automatically:

- **Time per activity** — Which activities you spend the most time on
- **Calories burned over time** — Your daily calorie burn trend
- **Activity distribution** — Percentage breakdown of activity types
- **Correlation heatmap** — Relationship between duration and calories burned

---

## 🔮 Future Improvements

- [ ] Add a GUI using Tkinter or a web interface
- [ ] Set personal fitness goals and track progress
- [ ] Export reports to PDF
- [ ] Add BMI and heart rate tracking
- [ ] Weekly and monthly summary reports

---

## 👨‍💻 Author

**Kenil Sanghavi**  
GitHub: [@KenilSanghavi](https://github.com/KenilSanghavi)
