<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=260&color=0:642bd4,100:8ec127&text=Julian%20Martos%20Alvari%C3%B1o&fontSize=58&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=MSc%20Computer%20Science%20%7C%20Machine%20Learning%20%C2%B7%20Sensor%20Data%20%C2%B7%20Efficient%20AI&descAlignY=58&descSize=18" width="100%" />

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=8EC127&center=true&vCenter=true&width=640&lines=MSc+Student+in+Computer+Science+%F0%9F%8E%93;Human+Activity+Recognition+from+IMU+data+%F0%9F%8F%83;92.1%25+on+unseen+people+with+a+94k+CNN+%E2%9A%A1;Efficient+medical+vision-language+models+%F0%9F%A9%BA;First-author+IEEE+R10-HTC+2026+%F0%9F%93%84;Open+to+AI%2FML+engineering+roles+%F0%9F%9A%80" alt="Typing SVG" /></a>

<p>
  <a href="https://linkedin.com/in/julian-martos-alvarino"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:julianmaral@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://github.com/JasonBestBork"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" /></a>
</p>

<img src="https://komarev.com/ghpvc/?username=JasonBestBork&label=PROFILE%20VIEWS&color=8ec127&style=flat-square" alt="Profile views" />

</div>

---

## 👋 About Me

<img align="right" width="300" src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif" alt="coding" />

I'm an **MSc student in Computer Science** at National Dong Hwa University (Taiwan), in the **Intelligent Computing and Mobile Network Lab**. I build machine learning systems end to end, from **raw sensor data to compact, carefully tested models**, with a focus on **healthcare**.

- 🎓 **MSc** in Computer Science, NDHU (2025 – 2027), ranked **1st of 11** in my first semester
- 🔬 **Research:** Human Activity Recognition from cheap phone and smartwatch IMUs, and efficient medical vision-language models
- 📄 **First-author paper** at IEEE R10-HTC 2026 (Bangkok, oral presentation)
- 💼 **Open to** AI/ML engineering roles in Taiwan and abroad
- 🎮 **Hobbies:** game development, VR and content creation
- 🌎 **Languages:** Spanish (native), English (fluent), Chinese (conversational)

<br clear="right"/>

---

## 🧪 Research

### 🏃 Thesis: Human Activity Recognition from Low-Cost IMU Sensors

I'm building a preprocessing pipeline that turns **raw accelerometer data from phones and smartwatches** into **Continuous Wavelet Transform (CWT)** images for CNNs, aimed at **medical and hospital use**. The long-term goal is a multi-sensor model where cheap sensors complement each other.

```mermaid
flowchart LR
    A[⌚ Raw IMU<br/>x, y, z] --> B[🧹 Audit + 20 Hz<br/>10 s windows]
    B --> C[🌊 CWT<br/>RGB image]
    C --> D[🧠 94k-param CNN<br/>+ motion features]
    D --> E[🏃 Activity]
```

| Result (WISDM, tested on 10 people never used in training) | Accuracy | Macro F1 |
|:--|:--:|:--:|
| Always guess "Walking" | 45.4% | – |
| Best published subject-wise result (ConvFormer, *Sensors* 2026) | 88.9% | 78.8 |
| **My CNN (3 seeds)** | **92.1% ± 0.4** | **88.5 ± 0.3** |

**Key finding:** how the image is built moves the score by up to **5.5 points**, while a **16× change in network size does not**. Random train/test splits inflate results by about 10 points, so every number here is split by person.

> [!NOTE]
> **Next:** replication on MotionSense and HAPT, then accelerometer + gyroscope fusion across devices.

### 🩺 Quantization of Medical Vision-Language Models

Does a compressed medical AI model still **look at the image**, or does it answer from the question alone?

- Evaluated **Qwen2-VL-2B** and **Qwen2.5-VL-3B** on **VQA-RAD** and **SLAKE**, from 16-bit down to 2-bit weights, with no-image and shuffled-image controls
- Found and fixed a **bfloat16 tie bug** that shifted results by up to 8 points
- Measured real GPU latency and energy: **INT8 was 2.0× slower and used 1.5× more energy** than bf16

`PyTorch` `Hugging Face` `bitsandbytes` `VLMs` `Energy measurement`

---

## 🚀 Current Status

| | |
|:--|:--|
| 🔭 **Working on** | Replicating my HAR pipeline on a second dataset |
| 🌱 **Learning** | Real-time optimization of deep learning models on edge devices |
| 👁️ **Exploring** | Computer vision applications in my free time |
| ⚡ **Fun fact** | I like content creation |

---

## 🏆 Highlights

| | Achievement |
|:--:|:--|
| 📄 | **IEEE R10-HTC 2026**, first author and oral presenter: *AIoT Wearable System for Safety-Critical Sound Detection in Sensory-Impaired Users* (Bangkok, Thailand) |
| 🥇 | **1st of 11 in class ranking**, MSc Computer Science, NDHU (Fall 2025, GPA 4.31) |
| 🎖️ | **Oral Presentation Honorable Mention**, 2026 Taiwan–Korea VIP International Exchange Workshop, for part of my HAR thesis work |
| 🥈 | **2nd Place, Project Presentation Award**, 2025 Taiwan–Korea VIP International Exchange Workshop, for Safe & Sound |
| 🏅 | **Excellence Award**, NDHU CSIE Undergraduate Project Exhibition (2025) |

---

## 📌 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### 🔊 Safe & Sound
AIoT wearable that detects alarms, sirens and horns and shows their direction, for sensory-impaired users. YAMNet + GCC-PHAT on a Realtek AMB82-Mini.

`Edge AI` `Arduino` `Android` `Firebase`

</td>
<td width="50%" valign="top">

### 🚁 VR Drone Simulator
Drone flight simulator for Meta Quest, built in Unity with ML-Agents.

`Unity` `C#` `ML-Agents` `VR`

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎯 VR Dodgeball
Dodgeball game for Meta Quest.

`Unity` `C#` `Meta Quest`

</td>
<td width="50%" valign="top">

### 🐦 CS50 Final Project
Flappy Bird-inspired game in Python (pygame). Harvard CS50P certificate.

`Python` `pygame`

</td>
</tr>
</table>

---

## 🛠 Tech Stack

<div align="center">

**🧠 AI / ML & Data**
<br/>
<img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow,sklearn" />
<br/>
<img src="https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat&logo=huggingface&logoColor=black" /> <img src="https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white" /> <img src="https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white" /> <img src="https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white" />

**💻 Languages**
<br/>
<img src="https://skillicons.dev/icons?i=cpp,c,cs,swift,kotlin" />

**📡 IoT & Mobile**
<br/>
<img src="https://skillicons.dev/icons?i=arduino,raspberrypi,androidstudio,firebase" />
<br/>
<img src="https://img.shields.io/badge/ESP32-E7352C?style=flat&logo=espressif&logoColor=white" /> <img src="https://img.shields.io/badge/ESP8266-E7352C?style=flat&logo=espressif&logoColor=white" /> <img src="https://img.shields.io/badge/IMU_sensors-555555?style=flat" />

**🎮 Game Dev & Design**
<br/>
<img src="https://skillicons.dev/icons?i=godot,unity,unreal,blender" />

**🧰 Tools**
<br/>
<img src="https://skillicons.dev/icons?i=linux,git,github,vscode" />

</div>

---

## 📊 GitHub Stats

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=JasonBestBork&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=8ec127&icon_color=642bd4" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JasonBestBork&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d1117&title_color=8ec127" />
  <br/>
  <img src="https://streak-stats.demolab.com?user=JasonBestBork&theme=tokyonight&hide_border=true&background=0d1117&ring=8ec127&fire=642bd4&currStreakLabel=8ec127" />
  <br/>
  <img width="100%" src="https://github-readme-activity-graph.vercel.app/graph?username=JasonBestBork&bg_color=0d1117&color=8ec127&line=642bd4&point=ffffff&area=true&hide_border=true" />
</div>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&height=120&section=footer&color=0:8ec127,100:642bd4" width="100%" />
</div>
