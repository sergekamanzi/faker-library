# faker-library

# 🏠 Household Energy Usage Dataset (Synthetic)

This project generates a **synthetic dataset** of household energy usage in Rwanda using the [Faker](https://pypi.org/project/Faker/) library and Python.  
The dataset is designed for **machine learning, data analysis, and energy consumption insights**.

---

## 📑 Features

- **11,000 household records** with structured data.  
- Appliances commonly found in Rwandan homes (e.g., *Iron, Laptop, Blender, LED Lamp, TV*).  
- Realistic **power consumption (Watts)** per appliance type.  
- **Monthly energy usage (kWh)** computed from power, usage hours, and quantity.  
- **Estimated bills (Frw)** calculated using Rwanda’s 2025 tariff brackets:
  - `0–20 kWh → 89 Frw per kWh`
  - `21–50 kWh → 310 Frw per kWh`
  - `50+ kWh → 369 Frw per kWh`
- Income level distribution: *Low (35%), Medium (50%), High (15%)*.  
- Regional diversity: *Kigali, Huye, Musanze, Rubavu, Nyagatare, Rusizi, Muhanga*.  

---

## 📂 Dataset Columns

| Column                | Description |
|------------------------|-------------|
| Household_ID           | Unique ID (H-0001 … H-11000) |
| Appliance              | Type of appliance |
| Power_Watts            | Power rating of appliance |
| Usage_Hours_Daily      | Average daily usage (hours) |
| Quantity               | Number of such appliances in the household |
| Region                 | Household location (district/city) |
| Income_Level           | Low, Medium, or High |
| Appliances_Count       | Total appliances in the household |
| Usage_Days_Monthly     | Days used per month |
| Household_Size         | Number of people in the household |
| Total_kWh_Monthly      | Monthly consumption in kWh |
| Tariff_Bracket         | Consumption block (0–20, 21–50, 50+ kWh) |
| Estimated_Bill_Fr      | Calculated bill (in Rwandan Francs) |

---

## 🚀 How to Generate

Clone the repo and run:

```bash
pip install faker pandas
python generate_dataset.py
