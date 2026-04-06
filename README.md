<div align="center">

# 🚨 AI Crime Visualizer
**Final Year Project | Computer Science Portfolio**

[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)](https://www.tensorflow.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

</div>

---

## 📖 Project Overview
The **AI Crime Visualizer** is a data-driven platform designed to analyze and forecast crime patterns. By leveraging Machine Learning, this tool identifies "hotspots" to assist law enforcement in proactive resource allocation.

### 🛠️ Technical Stack & CS Core
| Domain | Technology | Implementation |
| :--- | :--- | :--- |
| **Language** | Python 3.x | Core Logic & Data Processing |
| **AI Models** | Scikit-Learn / TF | Random Forest & Clustering |
| **Visualization** | Folium / Matplotlib | Geospatial Mapping & Trend Charts |
| **Security** | SHA-256 / HTTPS | Secure Data Hashing & Encryption |

---

## 🚀 Key Features
* **Trend Prediction:** Uses historical data to forecast future crime peaks using Regression models.
* **Interactive Geospatial Map:** A visual dashboard showing incident density across specific regions.
* **Information Security:** Implemented input sanitization and secure database architecture to prevent SQL injection.

---

---
---

## 📊 System Architecture

```mermaid
graph LR
    Data[Raw Crime Data] --> Pre[Pre-processing]
    Pre --> Model{AI Model Engine}
    Model --> Visual[Visualizer Dashboard]
    Visual --> User[End User/Police]
