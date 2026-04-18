<div align="center">

# 🚨 AI Crime Visualizer
**Final Year Project | Computer Science Portfolio**

[**🚀 Launch AI Visualizer Portal**](https://mumiz-ops.github.io/ai-crime-visualizer/login)

<br>

<div style="background: #0d1117; color: #58a6ff; padding: 20px; border-radius: 12px; font-family: 'Consolas', monospace; border: 1px solid #30363d; text-align: left; max-width: 550px; margin: 20px auto;">
  <div style="display: flex; justify-content: space-between; align-items: center;">
    <b style="color: #f0883e;">📡 AI NETWORK SCANNER: ACTIVE</b>
    <span id="timer" style="font-size: 11px; color: #8b949e;">SYSTEM SECURE</span>
  </div>
  <div style="background: #21262d; width: 100%; height: 8px; border-radius: 4px; margin: 15px 0; overflow: hidden;">
    <div id="ai-progress" style="background: #238636; width: 0%; height: 100%; border-radius: 4px; transition: width 0.3s;"></div>
  </div>
  <div style="background: #010409; padding: 12px; border-radius: 6px; height: 100px; overflow: hidden; font-size: 12px; border: 1px solid #21262d; line-height: 1.6;">
    <div id="data-log" style="color: #3fb950;">
      > Initializing CrimeVision 2.0...<br>
      > Connecting to Lahore Dataset...
    </div>
  </div>
</div>

<script>
  const log = document.getElementById('data-log');
  const bar = document.getElementById('ai-progress');
  const crimeData = [
    "LOC: Gulberg III | TYPE: Theft | RISK: Med",
    "LOC: DHA Phase 5 | TYPE: Vandalism | RISK: Low",
    "LOC: Model Town | TYPE: Burglary | RISK: High",
    "LOC: Johar Town | TYPE: Vehicle Theft | RISK: Med",
    "LOC: Anarkali | TYPE: Crowd Control | RISK: High",
    "LOC: Bahria Town | TYPE: Suspicious | RISK: Low"
  ];
  let progress = 0;
  setInterval(() => {
    progress = (progress + 15) % 100;
    if (bar) bar.style.width = progress + "%";
    const randomRecord = crimeData[Math.floor(Math.random() * crimeData.length)];
    const time = new Date().toLocaleTimeString();
    if (log) {
      log.innerHTML = `<div style="border-bottom: 1px solid #161b22;">[${time}] > ${randomRecord}</div>` + log.innerHTML;
      if (log.children.length > 4) log.removeChild(log.lastChild);
    }
  }, 2000);
</script>
<br>

[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)](https://www.tensorflow.org/)

</div>
