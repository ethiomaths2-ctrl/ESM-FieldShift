# ESM – FieldShift Ethiopia

**Clear Planting & Residual Moisture Decisions for Rain-fed Smallholder Farmers**

NASA Space Apps Challenge 2026  
Challenge: **Field Shift – Adapting Farms with NASA Data**

---

### Overview

ESM (FieldShift Ethiopia) is a practical decision-support tool that turns multiple NASA Earth observation datasets into simple, actionable advice for Ethiopian smallholder farmers.

Instead of showing complex satellite maps, the system answers three real questions farmers face:

1. **Is the soil ready to plant this week?**
2. **Is a dangerous dry spell (flash drought) starting?**
3. **After the main rains, is there still enough residual moisture for a short second crop?**

The tool is designed for dual delivery:
- Simple web/mobile app
- Future SMS channel
- Partnership pathway with Development Agents and the Ministry of Agriculture

---

### Live Demo

Open the file **`index.html`** in any modern browser (Chrome, Edge, Firefox, Safari).

No installation required.

---

### Key Features

- Woreda-level location selection (Region → Woreda)
- Multiple crops relevant to Ethiopia (Teff, Maize, Wheat, Chickpea, Lentil, etc.)
- Full English / Amharic language support
- Three clear decision engines with color-coded recommendations
- Transparent explanation of the backend data fusion logic
- Lightweight and works offline once loaded

---

### How the System Works (Backend Logic)

We do **not** simply display raw NASA layers. The system uses a three-layer approach:

1. **Data Ingestion**  
   SMAP L4 (root-zone soil moisture), NASA-USDA Soil Moisture, GPM IMERG rainfall, ECOSTRESS, MODIS ESI/LST, FLDAS, GLDAS, and supporting NASA POWER data.

2. **Interpretation / Fusion**  
   - Planting Readiness Engine  
   - Flash Drought Watch Engine  
   - Residual Moisture Opportunity Engine  

3. **Translation Layer**  
   Technical results are converted into plain-language recommendations (Plant Now / Wait / Good Opportunity, etc.) in English and Amharic.

> Note: The current prototype uses intelligent regional simulation to demonstrate the user experience and decision logic. The architecture is ready for connection to live Google Earth Engine or NASA data services.

---

### NASA Datasets Used

| Dataset | Purpose |
|---------|---------|
| SMAP L4 Root-zone Soil Moisture | Core input for planting readiness and residual moisture |
| NASA-USDA Global Soil Moisture | Surface and subsurface moisture support |
| GPM IMERG | Recent rainfall and anomalies |
| ECOSTRESS | High-resolution evaporative stress (flash drought) |
| MODIS ESI / LST | Vegetation and thermal stress confirmation |
| FLDAS & GLDAS | Land surface model context and residual moisture |
| NASA POWER | Climate context and historical normals |

---

### Project Structure

```
ESM-FieldShift/
├── index.html                  # Main application (open this file)
├── README.md                   # This file
└── docs/
    └── FieldShift_Ethiopia_Project_Description_Detailed.pdf
```

---

### How to Run Locally

1. Download or clone this repository
2. Open `index.html` in any browser
3. Select Region → Woreda → Crop
4. Click **Get Clear Advice**

---

### Future Development Roadmap

- Connect live NASA data via Google Earth Engine
- Add SMS gateway for farmers without smartphones
- Partner with local Development Agents and agricultural offices
- Improve woreda-level accuracy with higher-resolution products
- Add harvest-time rainfall risk module

---

### Team & Challenge

**Project Name:** ESM – FieldShift Ethiopia  
**Challenge:** Field Shift: Adapting Farms with NASA Data  
**Event:** NASA Space Apps Challenge 2026

---

### License & Attribution

This project was developed for the NASA Space Apps Challenge 2026.  
NASA data products used are open and publicly available.

---

**ESM – Turning NASA Earth Data into Clear Farmer Decisions**
