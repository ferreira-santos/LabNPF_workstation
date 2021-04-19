# LabNPF_workstation folder

The LabNPF_workstation folder is destined to automate and simplify the workflow when using the PC workstations at the [Laboratory of Neuropsychophysiology](https://www.fpce.up.pt/labpsi). As such, each PC workstation in the lab contains the folder "C:\LabNPF_workstation" to store files related to managing the workstation, matlab toolboxes, and other lab-related files. This allows users to quickly find the relevant information about the lab software that is installed and to easily perform updates - this is especially important when managing [EEGLAB](https://sccn.ucsd.edu/eeglab/index.php) (and [ERPLAB](https://erpinfo.org/erplab)) versions on the workstation.

Please note this package was designed specifically to address issues in our lab (namely managing multiple versions of MATLAB toolboxes in the same computer), so it may not be appropriate for other settings. However, anyone is welcome to use it and modify it as needed.

## Instalation/update
To install/setup the LabNPF_workstation folder:

1. Download the folder's source code from GitHub (https://github.com/ferreira-santos/LabNPF_workstation/releases) and extract the folder "LabNPF_workstation" it to the root directory ("C:\").
2. Then add the folder "C:\LabNPF_workstation\matlab_toolboxes\" to the MATLAB path (make sure you save this change).
3. Then, copy the toolboxes (like EEGLAB) to the "\matlab_toolboxes" folder.

When updating, it is necessary to first delete the previous version of the LabNPF_workstation folder, and then download and copy the new version. You will have to reinstall the toolboxes as well.

## Details
The present structure of the LabNPF_workstation folder is the following:
- Subfolders:
	- "\\_manage_workstation"
		- 1) Link to the LabNPF_workstation GitHub repository
		- 2) Link to LabWiki section on the lab's workstations
		- 3) Link to Download "Patch My PC" (https://patchmypc.com/home-updater)
		- Other files relevant for managing the workstations (e.g., eeglab toolbox installation instructions)
	- "\matlab_toolboxes"
		- This folder **must be added to the Matlab path** and saved.
		- Place toolbox folders here (e.g., EEGLAB).
		- For EEGLAB: **do not** add the EEGLAB folder to the Matlab path. This will be done automatically via the startup scripts in the LabNPF_workstation folder.
		- Place custom matlab functions here (files "labnpf_(...).m").
	- "\utils"
		- "\\eeg_channel_locations" - EEGLAB channel location files
		- [Link] EGI Knowledge Center (with videos).txt
		- EGI HydroCel-GSN 128 layout PDF

## Changelog
- v0.2 - Updated "\\_manage_workstation", added "\\utils".
- v0.1 - Initial release.

## Future versions
Possible updates to the folder include: 
- additional custom matlab functions/scripts
- custom electrode positioning files
- cheatsheets/reference documents (e.g., conversion between EGI and 10-20 electrode positions)
- add subfolder "r_scripts" for installing important R packages automatically when R is updated?

Lab members are welcome to suggest improvements to the folder. Please use the "issues" tool in GitHub (https://github.com/ferreira-santos/LabNPF_workstation/issues).
