<div align="center">

# 🚨 AI Crime Visualizer
**Final Year Project | Computer Science Portfolio**

[**🚀 Launch AI Visualizer Portal**](https://mumiz-ops.github.io/ai-crime-visualizer/login)

<div style="background: #0d1117; color: #58a6ff; padding: 20px; border-radius: 12px; font-family: 'Consolas', monospace; border: 1px solid #30363d; box-shadow: 0px 4px 15px rgba(0,0,0,0.5); text-align: left; max-width: 600px;">
  <div style="display: flex; justify-content: space-between; align-items: center;">
    <b style="color: #f0883e;">📡 AI NETWORK SCANNER: ACTIVE</b>
    <span id="timer" style="font-size: 12px; color: #8b949e;">LOGGING...</span>
  </div>

  <div style="background: #21262d; width: 100%; height: 8px; border-radius: 4px; margin: 15px 0;">
    <div id="ai-progress" style="background: linear-gradient(90deg, #238636, #2ea043); width: 0%; height: 100%; border-radius: 4px; transition: width 0.3s; box-shadow: 0 0 10px #238636;"></div>
  </div>

  <div style="background: #010409; padding: 10px; border-radius: 6px; height: 110px; overflow: hidden; font-size: 13px; border: 1px solid #21262d;">
    <div id="data-log" style="color: #3fb950;">
      > Initializing dataset...<br>
      > Loading AI Model: CrimeVision 2.0...
    </div>
  </div>
</div>

<script>
  const log = document.getElementById('data-log');
  const bar = document.getElementById('ai-progress');
  
  const crimeData = [
    "LOCATION: Gulberg III | TYPE: Theft | RISK: Medium",
    "LOCATION: DHA Phase 5 | TYPE: Vandalism | RISK: Low",
    "LOCATION: Model Town | TYPE: Burglary | RISK: High",
    "LOCATION: Johar Town | TYPE: Vehicle Theft | RISK: Medium",
    "LOCATION: Anarkali | TYPE: Crowd Disturbance | RISK: High",
    "LOCATION: Bahria Town | TYPE: Suspicious Activity | RISK: Low",
    "LOCATION: Mall Road | TYPE: Traffic Violation | RISK: Low"
  ];

  let progress = 0;
  setInterval(() => {
    progress = (progress + Math.random() * 15) % 100;
    bar.style.width = progress + "%";

    const randomRecord = crimeData[Math.floor(Math.random() * crimeData.length)];
    const time = new Date().toLocaleTimeString();
    
    log.innerHTML = `<div style="margin-bottom: 4px; border-bottom: 1px solid #161b22;">[${time}] > ${randomRecord}</div>` + log.innerHTML;
    
    if (log.children.length > 4) {
      log.removeChild(log.lastChild);
    }
  }, 1800);
</script>

<br>

[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)](https://www.tensorflow.org/)

</div>
