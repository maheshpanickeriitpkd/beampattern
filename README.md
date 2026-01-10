# 🔊 beampattern: k-Wave Based Ultrasound Pressure Field Estimation

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/)
[![Toolbox: k-Wave](https://img.shields.io/badge/Toolbox-k--Wave-blue.svg)](http://www.k-wave.org/)
[![Language: MATLAB](https://img.shields.io/badge/Language-MATLAB-red.svg)](https://www.mathworks.com/products/matlab.html)

**beampattern** is a MATLAB-based simulation toolbox designed to estimate and visualize acoustic pressure patterns for various ultrasound array configurations. By leveraging the **k-Wave** acoustic simulation framework, this tool allows researchers and engineers to model beamforming characteristics and energy distribution for custom transducer geometries.

---

## 🚀 Key Features

* **Diverse Array Support:** Easily estimate beampatterns for Linear, Phased, and Convex ultrasound arrays.
* **k-Wave Integration:** Utilizes the robust k-Wave toolbox for full-wave acoustic simulations in complex media.
* **Pressure Field Visualization:** Generate 2D and 3D maps of acoustic pressure to analyze side lobes, main lobe width, and focal zones.
* **Customizable Parameters:** Fine-tune transducer frequency, element spacing, focal depth, and medium properties.
* **Research-Ready:** Ideal for validating new beamforming algorithms or optimizing transducer design before hardware implementation.

---

## 🛠️ Installation & Prerequisites

### Prerequisites
- **MATLAB** (R2019b or later recommended)
- **k-Wave Toolbox:** Must be installed and added to your MATLAB path. Download it from [k-wave.org](http://www.k-wave.org/download.php).

### Setup
1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/drSigPro/beampattern.git](https://github.com/drSigPro/beampattern.git)
    cd beampattern
    ```
2.  **Add to Path:** In MATLAB, right-click the `beampattern` folder and select "Add to Path > Selected Folders and Subfolders".

---

## 💻 Usage

1.  **Configure Transducer:** Open the main script (e.g., `main_beampattern.m` or similar) to define your array type and focal points.
2.  **Run Simulation:**
    ```matlab
    % Execute the script to start the k-Wave simulation
    run('your_simulation_script.m')
    ```
3.  **Analyze Results:** The script will output the steady-state pressure field and plot the normalized beampattern across the lateral and axial dimensions.

---

## 📊 Technical Overview
The toolbox follows a structured simulation pipeline:
1.  **Grid Definition:** Creating a computational grid optimized for the chosen ultrasound frequency.
2.  **Source Modeling:** Defining the geometry and excitation pulse of the ultrasound transducer elements.
3.  **Sensor Masking:** Positioning sensors to capture the pressure distribution across the field of view.
4.  **Simulation:** Solving the acoustic wave equations.
5.  **Post-Processing:** Extracting peak pressure and beamwidth metrics.

---

## 📜 Academic Reference
If you use this toolbox in your research, please cite it as:

**Panicker, M. R.**, *beampattern: K-Wave based approach to estimate pressure pattern for various ultrasound array shapes*, (2022), GitHub repository, https://github.com/drSigPro/beampattern.

---

## ⚖️ License & Usage Terms

**Code Available under Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International (CC BY-NC-ND 4.0)**

See the [official license text](https://creativecommons.org/licenses/by-nc-nd/4.0/) for full details. 

*Commercial use of this code is strictly prohibited without prior written consent from the author.*

---
**Maintained by:** [Mahesh Raveendranatha Panicker](https://github.com/drSigPro)  
*For collaborations or inquiries, visit [PulseEcho](https://www.pulseecho.in/).*
