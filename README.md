# Real-time computation of bio-heat transfer in the fast explicit dynamics finite element algorithm (FED-FEM) framework (MIT License)

![fig1](https://user-images.githubusercontent.com/93865598/147665520-523adb97-a3cb-44da-a6d8-c215250d2167.PNG)

This is the source repository for the paper:

Zhang, J., & Chauhan, S. (2019). Real-time computation of bio-heat transfer in the fast explicit dynamics finite element algorithm (FED-FEM) framework. Numerical Heat Transfer, Part B: Fundamentals, 75(4), 217-238. [doi:10.1080/10407790.2019.1627812](https://www.tandfonline.com/doi/abs/10.1080/10407790.2019.1627812).

which is based on the work of [doi:10.1016/j.ijthermalsci.2019.01.030](https://www.sciencedirect.com/science/article/abs/pii/S1290072918317186) [[Code]](https://github.com/jinaojakezhang/FEDFEM).

Please cite the above paper if you use this code for your research.

# Environment:
•	Windows 10

•	Visual Studio 2017

•	OpenMP
# How to build:
1.	Download the source repository.
2.	Visual Studio 2017->Create New Project (Empty Project)->Project->Add Existing Item->Bioheat.cpp.
3.	Project->Properties->C/C++->Language->OpenMP Support->Yes (/openmp).
4.	Build Solution (Release/x64).
# How to use:
1.	(cmd)Command Prompt-> ![fig2](https://user-images.githubusercontent.com/93865598/147665523-e279c895-842d-4b30-a33b-5ecd613ce7f0.PNG)
2.	Output: T.vtk
# How to visualize:
1.	Open T.vtk. (such as using ParaView)

![fig3](https://user-images.githubusercontent.com/93865598/147665525-3ca085d7-f090-4124-8beb-6bb43494b321.PNG)
# Boundary condition (BC):
1.	Node index: HFlux, FixT.
2.	Element index: Perfu, BodyHFlux.
3.	All Elements: Metabo.
# Notes:
1.	Node and Element index can start at 0, 1, or any but must be consistent in a file.
2.	Liver_Iso.txt, node and element index start at 0; Liver_Iso_n1.txt, node and element index start at 1.
