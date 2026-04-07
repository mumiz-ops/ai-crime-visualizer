<div align="center">

# 🚨 AI Crime Visualizer
**Final Year Project | Computer Science Portfolio**
[**🚀 Launch AI Visualizer Portal**](https://mumiz-ops.github.io/ai-crime-visualizer/login)

<div style="background: #1a1a1a; color: #00ff00; padding: 15px; border-radius: 10px; font-family: 'Courier New', Courier, monospace; border: 2px solid #333;">
  <p style="margin: 0;">📡 <b>AI CRIME SYSTEM STATUS:</b> <span id="status-text">SCANNING...</span></p>
  <div style="background: #333; width: 100%; height: 10px; border-radius: 5px; margin-top: 10px;">
    <div id="progress-bar" style="background: #00ff00; width: 0%; height: 10px; border-radius: 5px; transition: width 0.5s;"></div>
  </div>
  <p style="font-size: 12px; margin-top: 10px; color: #888;">LATENCY: 14ms | MODELS: ACTIVE | SECURITY: ENFORCED</p>
</div>

<script>
  let width = 0;
  const bar = document.getElementById('progress-bar');
  const status = document.getElementById('status-text');
  
  setInterval(() => {
    width = (width + Math.random() * 20) % 100;
    bar.style.width = width + "%";
    if(width > 80) status.innerText = "THREAT DETECTED";
    else if(width > 40) status.innerText = "ANALYZING DATA";
    else status.innerText = "SYSTEM SECURE";
  }, 2000);
</script>

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
