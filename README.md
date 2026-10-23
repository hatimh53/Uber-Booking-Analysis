# Uber Booking Analysis

## Objective
To explore the NCR Uber bookings dataset and find patterns in booking status, cancellations, vehicle types, and payment methods.

## Dataset
150,000 Uber ride bookings from the NCR region, covering all of 2024. Includes booking status, vehicle type, pickup and drop location, payment method, ride distance, booking value, cancellation reasons, and customer/driver ratings.

## Tech Stack
- **Python** (pandas,matplot,seaborn) — data cleaning and exploratory analysis
- **Power BI** — interactive dashboard with click-to-filter vehicle selection
- **Jupyter Notebook** — analysis workflow

## Project Structure
```
├── Uber_Booking_Analysis.ipynb
├── Uber report data.csv
├── Uber Dashboard image.png
└── README.md
```

## Key Findings
👉🏻 The completed ride status is good, almost 62%. But Uber should focus on rides where drivers are not available and where rides are incomplete. Combined, they're almost 13% share, which the company can improve with the right measures.

👉🏻 Completed rides average about 2.5x the distance of incomplete rides (26 km vs 10.55 km). This could reflect either that short rides are more likely to be abandoned, or that incomplete rides simply stop early.

👉🏻 Drivers cancel rides about 2x more often than customers (18% vs 7%). There's no standout reason for either side — the cancellation reasons are evenly spread.

👉🏻 UPI is the most popular payment method, accounting for ~₹23.34M in total booking value. Cash comes second at ~₹12.9M. Together they make up about 70% of total booking value.

👉🏻 Auto holds the largest vehicle share (~25%) and the highest total booking value (~₹12.9M), but only because it has the most rides — its average value per ride is close to every other vehicle type. Go Mini and Go Sedan together make up around 38% of the vehicle category.

## Dashboard Preview
<img src="Uber Dashboard image.png" width="300">


## Methodology
Null values were treated as structural, not missing — for example, a blank `Cancelled Rides by Customer` means the booking wasn't cancelled by a customer, not that data is missing. Several patterns in the dataset (round status counts, uniform cancellation reasons, flat failure rates across vehicle type/hour/location) suggest the data may be simulated rather than collected from real rides, so findings describe patterns within this dataset rather than claims about real-world Uber behavior.

---
If you found this project helpful, consider giving it a ⭐ — it helps others discover it too.
