<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Typing Replace Animation</title>

  <style>
    body {
      background: #0f172a;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
    }

    .text {
      font-size: 32px;
      font-weight: 600;
      text-align: center;
      min-height: 50px;
    }

    .cursor {
      display: inline-block;
      width: 3px;
      background: white;
      margin-left: 5px;
      animation: blink 0.7s infinite;
    }

    @keyframes blink {
      0%, 50%, 100% { opacity: 1; }
      25%, 75% { opacity: 0; }
    }
  </style>
</head>

<body>

<div class="text" id="text"></div>

<script>
  const lines = [
    { text: "Hello. i'm Sandeep Kumar", color:"#38bdf8" },
    { text: "Data Analyst", color: "#22c55e" },
    { text: "Turning Raw Data Into Insights", color: "#facc15" },
    { text: "Power BI | Excel | SQL | Python", color: "#f472b6" }
  ];

  const textElement = document.getElementById("text");

  let lineIndex = 0;
  let charIndex = 0;

  function typeEffect() {
    if (lineIndex >= lines.length) return;

    const currentLine = lines[lineIndex];
    textElement.style.color = currentLine.color;

    if (charIndex < currentLine.text.length) {
      textElement.textContent += currentLine.text.charAt(charIndex);
      charIndex++;
      setTimeout(typeEffect, 50);
    } else {
      // Wait, then erase
      setTimeout(eraseEffect, 800);
    }
  }

  function eraseEffect() {
    if (charIndex > 0) {
      const currentLine = lines[lineIndex];
      textElement.textContent = currentLine.text.substring(0, charIndex - 1);
      charIndex--;
      setTimeout(eraseEffect, 30);
    } else {
      // Move to next line
      lineIndex++;
      charIndex = 0;
      setTimeout(typeEffect, 300);
    }
  }

  typeEffect();
</script>

</body>
</html>







<p align="center">
  <a href="#"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <a href="mailto:sandeeprawat0500@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="#"><img src="https://img.shields.io/badge/GitHub-000?style=for-the-badge&logo=github&logoColor=white"></a>
  <a href="#"><img src="https://img.shields.io/badge/Portfolio-FF5722?style=for-the-badge&logo=google-chrome&logoColor=white"></a>
</p>

---

### 🚀 About Me
**Data Analyst** skilled in **Python, SQL, Power BI, and Excel**, focused on solving real-world business problems using data.

- 🎓 B.Tech CSE (2023–2027)  
- 📊 Strong in **EDA, Data Cleaning & Visualization**  
- 📈 Experience with **real-world datasets**  
- 🎯 Goal: Deliver **data-driven insights for business growth**

---

### 📊 Featured Projects

#### 🛒 E-Commerce Data Analysis
- Cleaned and transformed messy datasets using **Python (Pandas)**
- Performed **SQL analysis** to extract revenue insights
- Built **Power BI dashboard** with KPIs and trends
- Generated business insights for decision-making

---

#### 🎬 Netflix Data Analysis
- Handled missing values and cleaned dataset
- Performed **EDA on genres and ratings**
- Visualized trends using **Matplotlib & Seaborn**
- Built dashboard for content insights

---

### 🧰 Technical Toolkit
<table align="center">
  <tr>
    <td align="center" width="33%"><strong>Languages</strong></td>
    <td align="center" width="33%"><strong>Libraries</strong></td>
    <td align="center" width="33%"><strong>Tools</strong></td>
  </tr>
  <tr>
    <td align="center">
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white"/><br>
      <img src="https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white"/>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white"/><br>
      <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white"/><br>
      <img src="https://img.shields.io/badge/Seaborn-4D8BBE?style=flat-square"/><br>
      <img src="https://img.shields.io/badge/Matplotlib-005C8E?style=flat-square"/>
    </td>
    <td align="center">
      <img src="https://img.shields.io/badge/PowerBI-F2C811?style=flat-square&logo=powerbi&logoColor=black"/><br>
      <img src="https://img.shields.io/badge/Excel-217346?style=flat-square&logo=microsoft-excel&logoColor=white"/><br>
      <img src="https://img.shields.io/badge/PowerQuery-E21017?style=flat-square"/><br>
      <img src="https://img.shields.io/badge/Data%20Analysis-6A1B9A?style=flat-square"/>
    </td>
  </tr>
</table>

---

### 📈 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YOUR_GITHUB_USERNAME&show_icons=true&theme=tokyonight" width="48%" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_GITHUB_USERNAME&layout=compact&theme=tokyonight" width="38%" />
</p>

---

### 📬 Connect with Me
- 🌐 Portfolio: (Add your portfolio link here)  
- 💼 LinkedIn: (Add your LinkedIn link here)  
- 📧 Email: sandeeprawat0500@gmail.com  

---

🚀 **Actively seeking Data Analyst Internship and Job opportunities**
