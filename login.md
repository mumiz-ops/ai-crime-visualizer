---
layout: default
title: Login Simulation
---

# 🔐 Restricted Access
### AI Crime Visualizer - Secure Portal

<div id="login-container" style="background: #f9f9f9; padding: 20px; border-radius: 8px; border: 1px solid #ddd;">
  <p>Please enter your developer credentials to access the AI Dashboard.</p>
  
  <label for="username">Username:</label><br>
  <input type="text" id="username" placeholder="Enter username" style="width: 100%; padding: 8px; margin: 8px 0;"><br>
  
  <label for="password">Password:</label><br>
  <input type="password" id="password" placeholder="Enter password" style="width: 100%; padding: 8px; margin: 8px 0;"><br>
  
  <button id="login-btn" style="background: #0366d6; color: white; border: none; padding: 10px 20px; border-radius: 4px; cursor: pointer; width: 100%;">Login</button>
  
  <p id="error-msg" style="color: red; display: none; margin-top: 10px;">❌ Access Denied: Invalid Credentials.</p>
</div>

<script>
  document.getElementById('login-btn').addEventListener('click', function() {
    const user = document.getElementById('username').value;
    const pass = document.getElementById('password').value;
    const error = document.getElementById('error-msg');

    // Simulation Credentials
    if (user === "admin" && pass === "portfolio2026") {
      alert("Success! Redirecting to AI Visualizer...");
      // In a real app, this would link to your secure dashboard
      window.location.href = "https://github.com/mumiz-ops/ai-crime-visualizer"; 
    } else {
      error.style.display = "block";
    }
  });
  const hour = new Date().getHours();
let greeting = "Good Evening";
if (hour < 12) greeting = "Good Morning";
else if (hour < 18) greeting = "Good Afternoon";

alert(greeting + "! Welcome to Mumiz's AI Laboratory.");
</script>
