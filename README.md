# Kujenga-Final-project-analyzing-Addis-Ababa-public-transport-distribution-using-GTFS-data.

This project develops a **Digital Twin** of Addis Ababa’s public transit network to evaluate its structural health and operational efficiency. By combining network science (PageRank) with biological flow models (SEIR), we identify why the city experiences intense congestion and where the system is failing to meet demand.

## 🚀 Project Overview

Is Addis Ababa's transit distributed optimally? To answer this, we analyzed the **2026 AddisMapTransit GTFS** dataset through two distinct lenses:

1.  **The Skeleton (Structure):** Using Weighted PageRank to find the "Critical Anchors" of the city.
2.  **The Pulse (Flow):** Using an SEIR Stress Test to simulate 100,000 commuters during the morning rush.

## 📊 Key Findings

*   **Extreme Centralization:** The top 1% of stops control nearly 4% of the entire network's importance, creating a "Single-Point-of-Failure" model.
*   **The 6:00 AM Crisis:** Systemic strain begins just 12 minutes into the morning rush. By 6:22 AM, over 52% of commuters are stuck in congestion.
*   **Red Zone Paradox:** We identified critical areas like **Merkato** that are operationally overloaded but structurally isolated—the definition of sub-optimality.

## ⚙️ Installation & Setup

To run this analysis, ensure you have Python installed, then install the dependencies using:

```bash
pip install -r requirements.txt
```

## 📂 Data Provenance & License

The data for this project is provided by the **AddisMap Team**, supported by the **DT4A Innovation Challenge Grant**. 

*   **License:** The data is under the **OSM License (ODbL OpenStreetMap contributors / AddisMapTransit.com)**.
*   **Source:** Data is extracted via the OSM OverPass API and updated weekly. You can find the live repository at the [AddisMap GitHub](https://github.com).
*   **Reproducibility:** Because the dataset is live and evolves with OpenStreetMap history, real-time versions may differ from this report. To reproduce these exact findings, use the static snapshot provided in the `/data` folder.

## 📝 Acknowledgments
Special thanks to **AddisMap** and **Digital Transport for Africa (DT4A)** for their ground-level data collection efforts. For official inquiries, contact `info@addismap.com`.

---
**Developed for the Addis Ababa Transit Optimization Study.**
