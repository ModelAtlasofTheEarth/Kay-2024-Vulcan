# New [M@TE](https://mate.science/)! model: 
 _we have provided a summary of your model as a starting point for the README, feel free to edit_
## Section 1: Summary of your model   

**Model Submitter:**  

Ben Kay ([0000-0002-9738-7277](https://orcid.org/0000-0002-9738-7277))

**Model Creator(s):**  

- Ben Kay ([0000-0002-9738-7277](https://orcid.org/0000-0002-9738-7277))  
  
**Model slug:**  


`Kay-2024-Vulcan-1` 

(this will be the name of the model repository when created) 

**Model name:**  

_3D magnetotelluric-derived electrical resistivity models of the Vulcan IOCG prospect under thick cover, South Australia_  

**License:**  

[Creative Commons Attribution 4.0 International]( https://creativecommons.org/licenses/by/4.0/legalcode.txt)

**Model Category:**  

- inverse model   
- model published in study   
  
**Model Status:**  

- completed   
  
**Associated Publication title:**  

_[Magnetotelluric imaging of an iron-oxide copper gold (IOCG) deposit under thick cover](https://doi.org/10.1080/08123985.2024.2378132)_ 

**Short description:**  

Three-dimensional electrical resistivity models derived from magnetotelluric (MT) data across the Vulcan iron-oxide copper–gold (IOCG) prospect in South Australia. The models image conductive sedimentary cover, a low-resistivity haematite breccia zone, and a deeper vertical conductive structure interpreted as a fluid pathway. Two inversion variants are provided: a smooth model and a structurally constrained “tear” model incorporating a known basement interface. These models provide constraints on subsurface structure and fluid pathways relevant to mineral exploration beneath thick conductive cover.

**Abstract:**  

This dataset contains 3D electrical resistivity models derived from magnetotelluric (MT) data collected over the Vulcan iron-oxide copper–gold (IOCG) prospect, located ~30 km northeast of Olympic Dam, South Australia. The survey comprises 100 broadband MT sites on a 1 km grid across a 9 × 9 km area.

Inversion of MT responses resolves three primary domains: (1) conductive sedimentary cover (~850 m thick), (2) a low-resistivity zone associated with haematite breccia beneath the cover, and (3) a vertically extensive conductive structure extending to several kilometres depth, interpreted as a pathway for mineralising fluids.

Two model variants are included: a smooth inversion and a model incorporating a structural discontinuity (“tear”) at the base of the sedimentary cover, based on drillhole constraints. The models provide insight into lithospheric-scale fluid pathways and the geometry of IOCG mineral systems under conductive cover sequences.

**Scientific Keywords:**  

- magnetotellurics   
- electrical resistivity   
- IOCG   
  
**Funder(s):**  
- Geological Survey of South Australia   
- FMG Resources Pty Ltd   
  
## Section 2: your model code, output data  

**No embargo on model contents requested** 

**Include model code:**   

True 

**Model code notes:**   

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

**Include model output data:**   

True 

**Model output data notes:**   

The output dataset includes both model results and predicted data products for two inversion variants:

Smooth model (uniform regularisation):

- [Native CGG Geotools format](https://github.com/user-attachments/files/27003430/Vulcan_2022_Smooth_Resistivity_Model.out.zip)
- [ASCII XYZV format](https://github.com/user-attachments/files/27003433/Vulcan_2022_Smooth_Resistivity_Model.xyzv.zip)

Tear model (structurally constrained at the base of sedimentary cover):
- [Native CGG Geotools format](https://github.com/user-attachments/files/27003429/Vulcan_2022_Tear_Resistivity_Model.out.zip)
- [ASCII XYZV format](https://github.com/user-attachments/files/27003432/Vulcan_2022_Tear_Resistivity_Model.xyzv.zip)

Predicted magnetotelluric responses are also provided as [EDI files](https://github.com/user-attachments/files/27003625/Modelled_Data.zip), enabling direct comparison between observed and modelled impedance tensors. 

## Section 3: software framework and compute details   
**Name of primary software framework:**  

CGG RLM-3D 

**Software & algorithm keywords:**  

- CGG RLM-3D   
- Viridien   
- NLCG   
- L-BFGS   
  
## Section 4: web material (for mate.science)   
**Landing page image:**  

Filename: [Vulcan_Graphical_Abstract_MATE.png](<https://github.com/user-attachments/assets/1d873775-f924-4c1c-872f-2f92d4ecdb92>)  
Caption: 3D perspective views of the smooth (top) and tear (bottom) resistivity models, highlighting differences in basement structure. Clipped resistivity values (30–60 Ωm) emphasise the vertical conductive feature and haematite breccia zone; the tear model better resolves structure at the top of basement consistent with drillhole and gravity constraints.  
  
**Animation:**  

Filename: [None]()  
  
**Graphic abstract:**  

Filename: [Vulcan_CrossSections_MATE.png](<https://github.com/user-attachments/assets/5dafaae7-e0c0-4489-bf79-1ba7aefc15d1>)

Caption: Comparison of smooth and tear-constrained 3D resistivity models showing improved resolution of basement structures and strong spatial agreement with gravity and drillhole constraints, highlighting a conductive pathway linked to the mineral system.  
  
**Model setup figure:**  

Filename: [Model_Setup.png](<https://github.com/user-attachments/assets/5d5f9d43-f624-4f76-bb0b-c6c7e72f1ddb>)  
Caption: Inversion mesh used for 3D MT modelling, including padding cells and a structural “tear” boundary at the base of the sedimentary cover. MT site locations are shown as black triangles; drillhole logs provide constraints on the tear depth. Mesh projection UTM Zone 54S.  

Description: The 3D resistivity models were generated using a non-linear conjugate gradient (NLCG) inversion scheme with L-BFGS preconditioning, designed to produce smooth, data-consistent models. A maximum of 50 inversion iterations was applied, with adjoint updates performed periodically during optimisation.

The inversion utilised magnetotelluric impedance tensor data over a frequency range of 0.01-100 Hz, sampled at approximately four points per decade. All four complex impedance components were inverted, with simultaneous estimation of frequency-independent 2×2 galvanic distortion matrices at each site. A strong regularisation weight (1000) was applied to keep distortion matrices close to the identity.

Forward modelling and sensitivity calculations were controlled with solver tolerances of 1×10⁻⁶ and 1×10⁻⁵, respectively, with a maximum of 1000 iterations per linear solve. A 1D adjoint approximation was used to improve computational efficiency.

Model resistivity was bounded between 0.5 and 5000 Ωm. Regularisation followed a smoothest-model approach using a hybrid Laplacian formulation, with anisotropic smoothing applied via vertical (τ = 0.006) and horizontal (τ = 2) weighting parameters. Additional near-surface smoothing was imposed to a depth of 500 m to suppress inversion artefacts and reflect the expected lateral continuity of sedimentary cover.
