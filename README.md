# 🚁 Project Leah-SAR: Extreme Environment Preset
![Betaflight](https://img.shields.io/badge/Betaflight-4.4%2B-blue) ![Stars](https://img.shields.io/github/stars/Kloudz805/leah-sar?style=social) ![License](https://img.shields.io/badge/License-MIT-green)

> *A high-reliability Betaflight firmware preset optimized for maximum signal penetration, rapid deployment, and low-resource logging in heavy-interference zones.*

## 🌍 The Mission
This project was built to make FPV drone technology more accessible and reliable for operators on the ground. Whether for search and rescue operations, critical field deployments, or assisting forces in Ukraine, the goal is simple: **keep the bird in the air and the video feed clear when it matters most.**

## ✨ Key Features
* **🛡️ Signal Reliability:** Aggressive filtering and VTX optimizations designed to punch through concrete, urban environments, and heavy RF noise.
* **🚀 Field Operations Mode:** Stripped-down, rapid-deployment settings. Plug in, arm, and fly without needing to navigate complex OSD menus in the field.
* **📊 Low-Resource Logging:** Optimized Blackbox settings to capture only mission-critical flight data without filling up onboard storage mid-deployment.
* **🤖 AI-Vision Ready:** Serves as the base flight tuning for the broader **Project Leah-SAR** and **Project Exocoetus** computer vision integrations.

## ⚙️ Quickstart Installation
Copy and paste the following snippet directly into your Betaflight CLI. *(Note: Ensure you are on Betaflight 4.4 or higher before applying).*

```text
# Project Leah-SAR: Extreme Environment Base Preset
# Author: Kloudz805

# VTX & Link Quality (Adjust power levels to your local regulations/mission needs)
set vtx_low_power_disarm = ON
set rc_interp = AUTO

# Low-Resource Blackbox Logging
set blackbox_p_ratio = 64
set blackbox_mode = NORMAL

# Heavy Payload/Extreme Environment Filtering
set dterm_lowpass_hz = 75
set gyro_lowpass_hz = 90

save
 ```
## 🛠️ Recommended Hardware
While this preset works on most modern 5" to 7" rigs, it was developed with industrial-grade reliability in mind. Best results are achieved using high-tier components like T-Motor flight stacks, iFlight hardware, and high-output VTX systems paired with reliable receivers like Fat Shark goggles.

## 🗺️ Roadmap
- [x] Base "Extreme Environment" PID & Filter tuning
- [ ] Low-bandwidth telemetry optimizations
- [ ] Project Exocoetus integration testing
- [ ] Full Leah-SAR AI-FPV vision handoff protocols

### ⭐️ Support the Project!
If this preset helped you maintain a vital video link or made your rapid deployment seamless, please consider hitting the Star button at the top right of this repository. It helps push this tool up in the algorithm so it can reach the operators who need it most!

*Built to save lives. 🇺🇦*

​
