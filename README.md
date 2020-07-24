
Description
===
Supplementary information for publication Ruan et al. in AAAS 2020.

Simulation of artificial cell with E number of ERMES spots, simulate distribution of minimum distances from 1 artificially spawned DUMP spot into the cell. E spots are not allowed to overlap, while DUMP spot is allowed to overlap.


Reports
===
### 20200518_LinhaoERMESDUMPSim[.ipynb, .html]
	Simulation driver and dataset compiler. Responsible for generation of datasets:
		Datasets with 10k simulation runs per dimension, with columns corresponding to :
		    [SimulationNumber, NumberOfERMESSpots, Minimum Distance]
		* stackedHistograms/2D_targetSpace.csv
		* stackedHistograms/3D_targetSpace.csv

		Filename is indicative of # of ERMES targets, and dimension space:
			ntargets_[ERMES NUMBER]_dim[DIMENSION SIZE].csv
		Columns correspond to:
			[Simulation Number, number of ERMES targets, minimum distance between ERMES and DUMP spot]
			Each data file has a corresponding "*.eps" file mapping the distribution.

		* singleDS_Plots/ntargets_1_dim2.csv
		* singleDS_Plots/ntargets_1_dim3.csv
		* singleDS_Plots/ntargets_2_dim2.csv
		* singleDS_Plots/ntargets_2_dim3.csv
		* singleDS_Plots/ntargets_3_dim2.csv
		* singleDS_Plots/ntargets_3_dim3.csv
		* singleDS_Plots/ntargets_4_dim2.csv
		* singleDS_Plots/ntargets_4_dim3.csv
		* singleDS_Plots/ntargets_5_dim2.csv
		* singleDS_Plots/ntargets_5_dim3.csv
		* singleDS_Plots/ntargets_6_dim2.csv
		* singleDS_Plots/ntargets_6_dim3.csv
		* singleDS_Plots/ntargets_7_dim2.csv
		* singleDS_Plots/ntargets_7_dim3.csv
		* singleDS_Plots/ntargets_8_dim2.csv
		* singleDS_Plots/ntargets_8_dim3.csv
		* singleDS_Plots/ntargets_9_dim2.csv
		* singleDS_Plots/ntargets_9_dim3.csv

### QQ_plots[.ipynb, .html]
	Generates QQ plots of real dataset against simulated dataset
	Actual measurements recorded by Linhao
		* qq_realData/experimentalMeasurements.csv

	Datasets with 203 simulations runs per dimension
		* qq_realData/QQ_output_dim3.csv
		* qq_realData/QQ_output_dim2.csv


Folders and Datasets
===
### qq_exptData
	Figures and datasets for comparison of simulated dataset against real dataset provided by Linhao.

### singleDS_Plots
	Single histogram datasets and plots for each individual tested # of ERMES spots and number of dimensions

### stackedHistograms
	Dataset and plots for distribution of simulated minimum distance separation dataset in 2D and 3D, testing for a range ERMES spots.

Plots
===
### 2dModelExanpleDiagram.png
	Sample rendering of 2D space with targets and "darts"
### 3dModelExanpleDiagram.png
	Sample rendering of 3D space with targets and "darts"
### deterministicSolution.eps
	deterministic probability distribution function calculated and plotted.