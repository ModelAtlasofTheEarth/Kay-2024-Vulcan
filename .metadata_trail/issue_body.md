### -> submitter ORCID (or name)

0000-0002-9738-7277

### -> slug

Kay-2024-Vulcan

### -> license

CC-BY-4.0

### -> alternative license URL

_No response_

### -> model category

inverse model, model published in study

### -> model status

completed

### -> associated publication DOI

https://doi.org/10.1080/08123985.2024.2378132

### -> model creators

0000-0002-9738-7277
0000-0001-7106-0789
0000-0002-7743-7812

### -> title

3D magnetotelluric-derived electrical resistivity models of the Vulcan IOCG prospect under thick cover, South Australia

### -> description

Three-dimensional electrical resistivity models derived from magnetotelluric (MT) data across the Vulcan iron-oxide copper–gold (IOCG) prospect in South Australia. The models image conductive sedimentary cover, a low-resistivity haematite breccia zone, and a deeper vertical conductive structure interpreted as a fluid pathway. Two inversion variants are provided: a smooth model and a structurally constrained “tear” model incorporating a known basement interface. These models provide constraints on subsurface structure and fluid pathways relevant to mineral exploration beneath thick conductive cover.

### -> abstract

This dataset contains 3D electrical resistivity models derived from magnetotelluric (MT) data collected over the Vulcan iron-oxide copper–gold (IOCG) prospect, located ~30 km northeast of Olympic Dam, South Australia. The survey comprises 100 broadband MT sites on a 1 km grid across a 9 × 9 km area.

Inversion of MT responses resolves three primary domains: (1) conductive sedimentary cover (~850 m thick), (2) a low-resistivity zone associated with haematite breccia beneath the cover, and (3) a vertically extensive conductive structure extending to several kilometres depth, interpreted as a pathway for mineralising fluids.

Two model variants are included: a smooth inversion and a model incorporating a structural discontinuity (“tear”) at the base of the sedimentary cover, based on drillhole constraints. The models provide insight into lithospheric-scale fluid pathways and the geometry of IOCG mineral systems under conductive cover sequences.

### -> scientific keywords

magnetotellurics, electrical resistivity, IOCG

### -> funder

Geological Survey of South Australia, Accelerated Discovery Initiative (ADI) project RD02-260.
FMG Resources Pty Ltd, Accelerated Discovery Initiative (ADI) project RD02-260.

### -> model embargo?

_No response_

### -> include model code ?

- [x] yes

### -> model code/inputs DOI

_No response_

### -> model code/inputs notes

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

### -> include model output data?

- [x] yes

### -> data creators

https://orcid.org/0000-0002-9738-7277
https://orcid.org/0000-0001-7106-0789
https://orcid.org/0000-0002-7743-7812

### -> model output data DOI

_No response_

### -> model output data notes

The output dataset includes both model results and predicted data products for two inversion variants:

Smooth model (uniform regularisation):

- [Native CGG Geotools format](https://github.com/user-attachments/files/27003430/Vulcan_2022_Smooth_Resistivity_Model.out.zip)
- [ASCII XYZV format](https://github.com/user-attachments/files/27003433/Vulcan_2022_Smooth_Resistivity_Model.xyzv.zip)

Tear model (structurally constrained at the base of sedimentary cover):
- [Native CGG Geotools format](https://github.com/user-attachments/files/27003429/Vulcan_2022_Tear_Resistivity_Model.out.zip)
- [ASCII XYZV format](https://github.com/user-attachments/files/27003432/Vulcan_2022_Tear_Resistivity_Model.xyzv.zip)

Predicted magnetotelluric responses are also provided as [EDI files](https://github.com/user-attachments/files/27003625/Modelled_Data.zip), enabling direct comparison between observed and modelled impedance tensors.

### -> model output data size

23 Mb

### -> software framework DOI/URI

_No response_

### -> software framework source repository

_No response_

### -> name of primary software framework (e.g. Underworld, ASPECT, Badlands, OpenFOAM)

CGG RLM-3D

### -> software framework authors

_No response_

### -> software & algorithm keywords

CGG RLM-3D, Viridien, NLCG, L-BFGS

### -> computer URI/DOI

_No response_

### -> add landing page image and caption

<img width="2726" height="2192" alt="Image" src="https://github.com/user-attachments/assets/8fe4048f-788b-4f60-a24c-afac83aa5309" />
3D perspective views of the smooth (top) and tear (bottom) resistivity models, highlighting differences in basement structure. Clipped resistivity values (30–60 Ωm) emphasise the vertical conductive feature and haematite breccia zone; the tear model better resolves structure at the top of basement consistent with drillhole and gravity constraints.

### -> add an animation (if relevant)

_No response_

### -> add a graphic abstract figure (if relevant)

<img width="3457" height="2406" alt="Image" src="https://github.com/user-attachments/assets/d576735d-f06a-4077-9ae8-7daec32ea6fa" />
Comparison of smooth and tear-constrained 3D resistivity models showing improved resolution of basement structures and strong spatial agreement with gravity and drillhole constraints, highlighting a conductive pathway linked to the mineral system.

### -> add a model setup figure (if relevant)

<img width="1814" height="508" alt="Image" src="https://github.com/user-attachments/assets/b0a6d761-3e7b-40ef-bd1a-7b722ba4df75" />
Inversion mesh used for 3D MT modelling, including padding cells and a structural “tear” boundary at the base of the sedimentary cover. MT site locations are shown as black triangles; drillhole logs provide constraints on the tear depth. Mesh projection UTM Zone 54S.

### -> add a description of your model setup

The 3D resistivity models were generated using a non-linear conjugate gradient (NLCG) inversion scheme with L-BFGS preconditioning, designed to produce smooth, data-consistent models. A maximum of 50 inversion iterations was applied, with adjoint updates performed periodically during optimisation.

The inversion utilised magnetotelluric impedance tensor data over a frequency range of 0.01-100 Hz, sampled at approximately four points per decade. All four complex impedance components were inverted, with simultaneous estimation of frequency-independent 2×2 galvanic distortion matrices at each site. A strong regularisation weight (1000) was applied to keep distortion matrices close to the identity.

Forward modelling and sensitivity calculations were controlled with solver tolerances of 1×10⁻⁶ and 1×10⁻⁵, respectively, with a maximum of 1000 iterations per linear solve. A 1D adjoint approximation was used to improve computational efficiency.

Model resistivity was bounded between 0.5 and 5000 Ωm. Regularisation followed a smoothest-model approach using a hybrid Laplacian formulation, with anisotropic smoothing applied via vertical (τ = 0.006) and horizontal (τ = 2) weighting parameters. Additional near-surface smoothing was imposed to a depth of 500 m to suppress inversion artefacts and reflect the expected lateral continuity of sedimentary cover.

### Please provide any feedback on the model submission process?

Some file formats couldn't be uploaded, hence the zipped files.