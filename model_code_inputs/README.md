# Model Code & Inputs

## Notes:
The models were generated using a commercial 3D magnetotelluric inversion algorithm (CGG RLM-3D). While the inversion software itself cannot be distributed, all relevant model inputs required to reproduce or reinterpret the results are provided.

Key inversion settings include:
- Non-linear conjugate gradient optimisation with L-BFGS preconditioning
- Frequency range: 0.01–100 Hz (4 points per decade)
- Full impedance tensor inversion with per-site galvanic distortion estimation
- Resistivity bounds constrained between 0.5–5000 Ωm
- Smoothness-constrained inversion using a hybrid Laplacian regularisation

Full parameter files and input datasets are included, with:

- [Interpolated EDI data](https://github.com/user-attachments/files/26999946/Interpolated_EDI_Files.zip)
- [Model parameters](https://github.com/user-attachments/files/26999969/parameters.txt)
- [Site Locations](https://github.com/user-attachments/files/26999972/sites.csv)
- [Starting model mesh](https://github.com/user-attachments/files/27000002/Vulcan_Job_RLM3DMT_1_it050_start.out.zip)
- [Tear boundary](https://github.com/user-attachments/files/27000006/Vulcan.tear.zip)