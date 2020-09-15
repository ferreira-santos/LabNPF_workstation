# LabNPF_workstation folder

The LabNPF_workstation folder is destined to automate and simplify the workflow when using the PC workstations at the [Laboratory of Neuropsychophysiology](https://www.fpce.up.pt/labpsi). As such, each PC workstation in the lab contains the folder "C:\LabNPF_workstation" to store files related to managing the workstation, matlab toolboxes, and other lab-related files. This allows users to quickly find the relevant information about the lab software that is installed and to easily perform updates - this is especially important when managing [EEGLAB](https://sccn.ucsd.edu/eeglab/index.php) (and [ERPLAB](https://erpinfo.org/erplab)) versions on the workstation.

## Instalation/update
To install/setup the LabNPF_workstation folder, simply download the folder from GitHub (https://github.com/ferreira-santos/LabNPF_workstation/archive/master.zip) and copy it to the root directory ("C:\"). Then add the folder "C:\LabNPF_workstation\matlab_toolboxes\" to the MATLAB path (e.g., by using the code `addpath('C:\LabNPF_workstation\matlab_toolboxes\')`).

Then, copy the toolboxes (like EEGLAB) to the "\matlab_toolboxes" folder.

When updating, it is safer to first delete the previous version of the LabNPF_workstation folder, and then download and copy the new version. You will have to reinstall the toolboxes as well.

## Details
The present structure of the LabNPF_workstation folder is the following:
- Subfolders:
	- "\\_manage_workstation"
		- Link to the LabNPF_workstation GitHub repository
		- Link to LabWiki section on the lab's workstations [planned]
		- Text file with the specifications of the PC (Speccy) [optional]
		- Scripts for activation of softare (e.g., Microsoft Office U.Porto KMS activation) [optional]
		- Other files relevant for managing the workstations
	- "\matlab_toolboxes"
		- This folder **must be added to the Matlab path** and saved.
		- Place toolbox folders here (e.g., EEGLAB).
		- For EEGLAB: **do not** add the EEGLAB folder to the Matlab path. This will be done automatically via the startup scripts in the LabNPF_workstation folder.
		- Place custom matlab functions here (files "labnpf_(...).m").
	- "\r_scripts" [optional]
		- Scripts for installing important R packages automatically when R is updated.
		- Maintain version control.
		- (Not implemented yet).

## Future versions
Possible updates to the folder include: 
- additional custom matlab functions/scripts
- custom electrode positioning files
- cheatsheets/reference documents (e.g., conversion between EGI and 10-20 electrode positions)

Lab members are welcome to suggest improvements to the folder. Please use the "issues" tool in GitHub (https://github.com/ferreira-santos/LabNPF_workstation/issues).
