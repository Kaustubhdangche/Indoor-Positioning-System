# Indoor Positioning System with Kalman Filter

This project implements a basic **indoor positioning system** using **trilateration** and **Kalman Filter** smoothing in Python. It was created as part of preparation for contributing to the **Movement** project under **Google Summer of Code (GSoC) 2025**.

## 📌 Project Overview

The goal is to estimate the position of a moving object indoors by using distance measurements from three fixed beacons (A, B, C). We apply:
- **Trilateration**: Calculates raw position estimates from distances.
- **Kalman Filtering**: Smooths the noisy position estimates over time.

## 📁 Dataset

A CSV file contains the measured distances to three beacons (`Distance A`, `Distance B`, `Distance C`) at each timestamp. Example:

```
Distance A,Distance B,Distance C
2.1, 3.9, 2.8
...
```

Beacon coordinates:
- A: (0, 0)
- B: (5, 0)
- C: (2.5, 5)

## 🛠️ Installation

Create a virtual environment and install dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ How to Run

Open the notebook:

```bash
jupyter notebook Indoor_Positioning_System.ipynb
```

Run all cells to perform:
- Distance-based trilateration
- Kalman Filter smoothing
- Visualization

## 📊 Output Insight

The final plot shows:
- Raw estimated positions from trilateration (blue dots)
- Smoothed trajectory using Kalman Filter (orange line)

This shows how filtering reduces noise in indoor location tracking.

## 📄 GSoC Use

This project demonstrates:
- Experience with **Kalman Filters** and **state estimation**
- Working with **noisy sensor data**
- Real-world use cases of **motion smoothing**

It aligns well with the Movement GSoC project on Kalman filters for animal tracking or indoor positioning.

## 👨‍💻 Author

**[Your Name]**  
Master’s in Data Science, USA  
GitHub: [yourusername]

---