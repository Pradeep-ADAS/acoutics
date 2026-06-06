# Automotive-NVH-Prediction-ML

⭐ **1. Introduction**

Lightweight porous foams are widely used in automotive interiors for noise reduction, passenger comfort, and vibration damping. Components such as headliners, door panels, dashboard insulation, wheel arch liners, and cabin acoustic treatments rely on carefully engineered foam structures to achieve targeted sound absorption performance across a broad frequency range.

This project investigates the relationship between the physical characteristics of polyurethane-based composite foams and their acoustic behavior. Using experimentally measured material properties such as thickness, density, porosity, and pore size, multiple machine learning models were developed to predict frequency-dependent Sound Absorption Coefficients (SAC). The objective is to evaluate the feasibility of using data-driven methods to estimate acoustic performance and reduce the need for extensive experimental testing during material development.

<p align="center">
  <img src="Acoustics1.jfif" width="35%"><br>
  <b>Acoustic Insulation – Door Panels</b>
</p>

---

🧩 **2. Challenge**

Predicting the acoustic performance of porous materials such as polyurethane foams is a complex task due to the strong coupling between microstructural properties and frequency-dependent sound absorption behavior.

Experimental characterization using impedance tube testing is accurate but time-consuming, resource-intensive, and requires specialized equipment. Additionally, each material configuration must be physically fabricated and tested across multiple frequencies to obtain its full acoustic response.

Key challenges include:

* Capturing the nonlinear relationship between foam structural properties (porosity, pore size, density, thickness) and Sound Absorption Coefficient (SAC).
* Modeling frequency-dependent acoustic behavior rather than a single scalar output.
* Handling limited experimental datasets typical in materials research.
* Reducing reliance on repeated physical testing through data-driven prediction methods.

---

🎯 **3. Objectives**

This project focuses on developing a machine learning-based framework to predict the sound absorption performance of polyurethane-based composite foams for automotive acoustic applications.

Key objectives include:

* Develop regression models to predict frequency-dependent Sound Absorption Coefficients (SAC) from foam structural properties.
* Analyze the influence of material characteristics such as porosity, pore size, density, and thickness on acoustic performance.
* Assess model robustness under limited dataset conditions typical of experimental material science studies.
* Enable data-driven estimation of acoustic performance to reduce reliance on repeated impedance tube experiments.

---

🛠 4. **Tech Stack**

Key techniques used in the prediction of acoustic performance of polyurethene based composite foams include:

* Python – core implementation for data processing and machine learning models
* NumPy – numerical computations for dataset handling and feature processing
* Pandas – structured data manipulation and analysis of experimental results
* Scikit-learn – machine learning models including Random Forest, Decision Tree, SVR, and regression baselines
* Matplotlib / Seaborn – visualization of SAC trends, model performance, and feature relationships
* Jupyter Notebook – exploratory analysis and model development environment

---

🧱 5. **Test Sample Structure: 4-Layer Sandwich Configuration**

Each experimental specimen is constructed as a four-layer sandwich structure, where each layer corresponds to a specific foam type defined by its material composition (e.g., PU foam with varying natural fiber content).

The overall sample configuration is represented using a four-character code (e.g., aaaa, aaab, aaba), where:

- Each character represents one foam layer in the stack <br>
- Each layer has a defined material composition (PU or PU + fiber content) <br>
- A full 4-character code represents the complete test specimen

<table>
  <tr>
    <td align="center">
      <b>Simplified Animation of Sandwich Structure </b><br>
      <img src="Acoustic_GIF.gif" width="700"/>
    </td>
  </tr>
</table>

---

📊 **6. Data Collection for ML Model Training – Lab Tests**

The dataset used for machine learning model development is obtained from controlled laboratory experiments on polyurethane-based composite foams reinforced with natural fillers such as sawdust and rice husk.

The experimental data captures both material structural properties and acoustic response characteristics across multiple frequency ranges.

🔬 **Experimental Data Acquisition Methods:**

* Foam samples were fabricated using a single-shot free-rise polyurethane foaming process.
* Frequency-dependent Sound Absorption Coefficient (SAC) values were measured using an impedance tube setup in accordance with ASTM E1050 standards.
* Microstructural analysis was performed using FESEM imaging to capture pore morphology.
* Pore size distribution was estimated using ImageJ-based image processing techniques.
* Porosity was evaluated using a gas-based non-acoustic measurement method based on the ideal gas law.

<p align="center">
  <img src="Impendance_Tube_Setup.PNG" width="50%"><br>
  <b> Impedance Tube Setup for SAC measurement</b>
</p>

---

📊 **7. Final Dataset for ML**
