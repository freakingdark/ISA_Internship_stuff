# 🌌 ISA Internship Projects – Astronomy & Cosmology

This repository contains projects completed during the **Indian Space Academy (ISA) Internship – Summer School of Astronomy and Astrophysics**.

The work focuses on observational astrophysics and cosmology using real astronomical datasets, statistical analysis, and physical modeling.

Author: **Deepali Pandey**  
Institute: Ramniranjan Jhunjhunwala College  
ISA Admission No: 396517  

---

## 📚 Project Overview

This repository includes two major projects:

1. **Estimating the Dynamical Mass of a Galaxy Cluster**
2. **Measuring Cosmological Parameters Using Type Ia Supernovae**

Both projects combine astrophysical theory, observational data analysis, numerical methods, and scientific visualization.

---

# 🛰️ Project 1: Dynamical Mass of a Galaxy Cluster

### Objective
To estimate the physical properties of a galaxy cluster — including redshift, velocity dispersion, size, dynamical mass, luminous mass, and mass-to-light ratio — using spectroscopic and photometric data.

### Dataset
- Redshift (`specz`)
- Right Ascension (RA)
- Declination (DEC)
- Projected angular separation
- r-band magnitudes

---

## 🔬 Methodology

### 1️⃣ Cluster Member Identification
- Applied **3σ clipping** on redshift distribution.
- Identified cluster members within:
- 0.0551 ≤ z ≤ 0.1066
- Likely cluster identified: **Abell 2255**

---

### 2️⃣ Cluster Redshift
- z_cluster ≈ 0.08007

  
---

### 3️⃣ Velocity Dispersion

Using the relativistic Doppler formula:

σ_v ≈ 1218 km/s


This confirms a gravitationally bound massive system.

---

### 4️⃣ Physical Size

Using cosmological relations:

- Diameter ≈ **0.923 Mpc**
- Radius ≈ **0.462 Mpc**

---

### 5️⃣ Dynamical Mass (Virial Theorem)
M_dyn ≈ 4.62 × 10^14 M☉

---

### 6️⃣ Luminous Mass
M_lum ≈ 4.97 × 10^12 M☉

---

### 7️⃣ Mass-to-Light Ratio
M/L ≈ 169


This large value strongly indicates the presence of **dark matter**, as expected for galaxy clusters.

---

## 📊 Visualizations Included

- Redshift histogram & boxplot
- Velocity dispersion histogram
- Angular separation distribution
- RA vs DEC sky map

These plots validate cluster membership and spatial coherence.

---

# 🌠 Project 2: Supernova Cosmology

### Objective
To estimate cosmological parameters using the **Pantheon+SH0ES Type Ia Supernova dataset** and test the ΛCDM cosmological model.

---

## 🔭 Methodology

- Constructed the **Hubble Diagram** (μ vs z)
- Used numerical integration for luminosity distance
- Fitted parameters using `scipy.optimize.curve_fit`
- Estimated:
  - Hubble constant (H₀)
  - Matter density parameter (Ωm)
  - Age of the Universe
- Analyzed residuals
- Split dataset into low-z and high-z samples

---

## 📈 Key Results

### Best-fit Parameters (Flat ΛCDM)
H₀ = 72.97 ± 0.26 km/s/Mpc
Ωm ≈ 0.35


This aligns with local SH0ES measurements and reflects the ongoing **Hubble tension** compared to Planck CMB results (~67.4 km/s/Mpc).

---

### Age of the Universe

Assuming Ωm = 0.3:
Age ≈ 12.92 Gyr


---

### Redshift Split Analysis

- Low-z (z < 0.1): H₀ ≈ 73.01
- High-z (z ≥ 0.1): H₀ ≈ 73.85

Indicates mild redshift-dependent variation.

---

## 📊 Visualizations Included

- Redshift vs Distance Modulus
- Hubble Diagram with Model Fit
- Residual plot (μ_obs − μ_model)
- Low-z vs High-z comparison

Residuals show no major systematic trend, confirming model consistency.

---

# 🧠 Scientific Insights

- Galaxy clusters are dark matter dominated.
- Supernova data alone yields a high H₀ consistent with local probes.
- Results reinforce the observational basis of the **Hubble tension**.
- Flat ΛCDM provides a strong fit but may require refinement.

---

# 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Astropy
- SciPy
- Astroquery

---

# 🚀 How to Run

1. Clone the repository:

```bash
git clone https://github.com/freakingdark/ISA_Internship_stuff.git
cd ISA_Internship_stuff

Create virtual environment:

python -m venv venv
source venv/bin/activate

Install dependencies:

pip install numpy pandas matplotlib astropy scipy astroquery

Run notebooks in Jupyter:

jupyter notebook
📌 Key Skills Demonstrated

Observational data analysis

Statistical filtering (3σ clipping)

Cosmological modeling

Numerical integration

Curve fitting

Scientific visualization

Interpretation of astrophysical results

📄 License

This repository is intended for academic and portfolio purposes.


