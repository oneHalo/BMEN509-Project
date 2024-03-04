Dataset Name: task (language and motor)/rest fMRI datasets in tumor patients

Overview
This dataset contains retrospective task-based and resting-state functional magnetic resonance imaging (fMRI) data collected from patients diagnosed with brain tumors. Mapping motor and language functions with task-based vs. resting-state fMRI have been published in two papers:

https://doi.org/10.1371/journal.pone.0236423
https://doi.org/10.1016%2Fj.nic.2017.06.011

We encourage the use of this dataset for further research and analysis in the fields of cognitive neuroscience, neuro-oncology, and neuroimaging.

Dataset Description
Participants
The dataset includes data from 41 tumor patients diagnosed. Each participant underwent both task-based and resting-state fMRI scanning. Detailed demographic information (age, sex, handedness, tumor location, tumor pathology) is provided in the patient_demographics.csv file.

Imaging Data
Structural data: T1-weighted images for all subjects. Please note that some participants have additional T2-weighted and FLAIR images 

Task-based fMRI: Participants were engaged in language (word-stem completion) and motor (finger-tapping) tasks. 
The dataset reflects variability in the number of frames recorded across different subjects for their respective task runs.

The task paradigm used in this dataset is represented by the following sequence:
80 frames:
xx----------++++++++++----------++++++++++----------++++++++++----------++++++++

90 frames:
xx----------++++++++++----------++++++++++----------++++++++++----------++++++++++--------

100 frames: 
xx----------++++++++++----------++++++++++----------++++++++++----------++++++++++----------++++++++

    xx: Represents the initial baseline period before the task begins
    -: Indicates a rest period where participants are not engaged in any task-related activity
    +: Represents active task periods where participants are engaged in motor/language tasks

Resting-state fMRI: Participants were instructed to relax and remain still with their eyes open for the duration of the scan.
The dataset includes two rs-fMRI runs for each patient, 160 frames per run; exceptions of subjects sub-RS001, sub-RS006, and sub-RS018
sub-RS001: 1 run, 80 frames
sub-RS006: 2 runs, 60 frames each
sub-RS018: 1 run, 160 frames 

All fMRI data are provided in NIfTI format, with accompanying JSON files containing scan parameters. The dataset is organized according to the BIDS standard, with each participant's data stored in a separate subdirectory.