# Real-time computation of bio-heat transfer in the fast explicit dynamics finite element algorithm (FED-FEM) framework (MIT License)
![GitHub](https://img.shields.io/github/license/jinaojakezhang/FEDFEMBioheat)
![GitHub top language](https://img.shields.io/github/languages/top/jinaojakezhang/FEDFEMBioheat)
<p align="center"><img src="https://user-images.githubusercontent.com/93865598/147665520-523adb97-a3cb-44da-a6d8-c215250d2167.PNG"></p>
This is the source repository for the paper:

| Zhang, J., & Chauhan, S. (2019). Real-time computation of bio-heat transfer in the fast explicit dynamics finite element algorithm (FED-FEM) framework. *Numerical Heat Transfer, Part B: Fundamentals*, 75(4), 217-238. [doi:10.1080/10407790.2019.1627812](https://www.tandfonline.com/doi/abs/10.1080/10407790.2019.1627812). |
| --- |

which is based on the work of
| <p align="left">Zhang, J., & Chauhan, S. (2019). Fast explicit dynamics finite element algorithm for transient heat transfer. *International Journal of Thermal Sciences*, 139, 160-175. [doi:10.1016/j.ijthermalsci.2019.01.030](https://www.sciencedirect.com/science/article/abs/pii/S1290072918317186) [[Code]](https://github.com/jinaojakezhang/FEDFEM).</p> |
| --- |

Please cite the above paper if you use this code for your research.

If this code is helpful in your projects, please help to :star: this repo or recommend it to your friends. Thanks:blush:
## Environment:
- Windows 10
- Visual Studio 2017
-	OpenMP
## How to build:
1.	Download the source repository.
2.	Visual Studio 2017->Create New Project (Empty Project)->Project->Add Existing Item->Bioheat.cpp.
3.	Project->Properties->C/C++->Language->OpenMP Support->**Yes (/openmp)**.
4.	Build Solution (Release/x64).
## How to use:
1.	(cmd)Command Prompt->build path>project_name.exe input.txt. Example: <p align="center"><img src="https://user-images.githubusercontent.com/93865598/149734301-a6b5adcd-3a77-4853-bf2c-c0ff085c5b94.PNG"></p>
2.	Output: T.vtk
## How to visualize:
1.	Open T.vtk. (such as using ParaView)
<p align="center"><img src="https://user-images.githubusercontent.com/93865598/147665525-3ca085d7-f090-4124-8beb-6bb43494b321.PNG"></p>

## How to make input.txt:
1.	Liver_Iso.inp (Abaqus input) is provided in the “models”, which was used to create Liver_Iso_n1.txt.
## Material types:
1.	Isotropic, orthotropic, and anisotropic thermal conductivities.
## Boundary conditions (BCs):
1.	Node index: HFlux, FixT.
2.	Element index: Perfu, BodyHFlux.
3.	All Elements: Metabo.
## Notes:
1.	Node and Element index can start at 0, 1, or any but must be consistent in a file.
2.	Index starts at 0: *.txt.
3.	Index starts at 1: *_n1.txt.
## Feedback:
Please send an email to jinao.zhang@hotmail.com. Thanks for your valuable feedback and suggestions.
