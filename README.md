# Processing-dependent structural evolution and glass transition in Ni–Mn alloys

This repository contains the input files, selected simulation outputs, and processed data used in the manuscript:

"Processing-dependent structural evolution and glass transition in Ni–Mn alloys: A molecular dynamics study"

## 1. Simulation details

All molecular dynamics (MD) simulations were performed using **LAMMPS** with the MEAM potential for Ni–Mn alloys.

- Ensemble: NVT (Nosé–Hoover thermostat)
- Time step: 1 fs
- Temperature range: 4500 K → 300 K
- Cooling rates: 5×10¹², 1×10¹³, 1×10¹⁴ K/s

Atomic configurations were analyzed using **OVITO** and **Origin**.

---

## 2. Repository structure

### input/
LAMMPS input scripts for different system sizes:

- NiMn_4000.in  
- NiMn_6912.in  
- NiMn_10976.in  
- NiMn_16384.in  

---

### dump/
Selected atomic configurations (LAMMPS dump format):

- dump_16384_300K.dump  
- dump_16384_500K.dump  
- dump_16384_700K.dump  
- dump_16384_900K.dump  

Additional files for system-size comparison are also included.

---

### data/
Processed data used to generate all figures in the manuscript:

- rdf_vs_cooling_rate.dat  
- rdf_vs_system_size.dat  
- rdf_vs_annealing_time.dat  
- CNA_vs_temperature.csv  
- CNA_vs_system_size.csv  
- coordination_number.csv  
- Warren_Cowley.csv  
- S_q.csv  
- energy_vs_temperature.dat  
- Q4_Q6_vs_temperature.dat  

---

## 3. Reproducibility

To reproduce the simulations:

1. Run LAMMPS using input files in the `input/` directory.
2. Analyze atomic structures using OVITO (CNA, coordination number).
3. Use the provided data files to reproduce figures (RDF, S(q), Q4, Q6, etc.).

---

## 4. Notes

- Only representative dump files are provided due to file size limitations.
- ICO structures were identified but not included in detailed analysis due to their negligible fraction.

---

## 5. Contact

Corresponding author:  
Mai Van Dung  
Email: dungmv@ut.edu.vn