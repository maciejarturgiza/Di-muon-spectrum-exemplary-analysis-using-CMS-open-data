# Di-muon-spectrum-exemplary-analysis-using-CMS-open-data
Analysis of the di-muon spectrum using data from the CMS detector

The topic of the exercise was to obtain a spectrum of di-muon invariant mass that would be similar to the official result of the CMS collaboration, using the open-source CSV files.

# Samples description

Samples taken from Zenodo website: "CMS Open Data 2012 datasets for dimuon exercises" by Alejandro Gomez Espinosa

All samples can be found under the link: https://zenodo.org/record/5345875#.YdgZdWjMJPY

These datasets are a subset of the CMS Open data with 2021 data-taking conditions for education purposes. The files are in CSV and PKL formats (only use one of those) and contain two datasets:

- Data files, starting with output_data_CMS_Run2012B, correspond to 4429.37 /pb of data collected by the CMS Experiment. They are a subset of the dataset on reference [1].

- Simulation files, starting with output_sim_CMS_MonteCarlo2012, are a subset of the dataset referenced on [2]. The number of generated events in this case is 30458871, and the cross section is 3503.71.

All the files were processed with a modified version of the AOD2NanoAODOutreachTool [3]. The small modifications are related to the number of triggers stored, and some objects like taus were removed.



[1] CMS collaboration (2017). DoubleMuParked primary dataset in AOD format from Run of 2012 (/DoubleMuParked/Run2012B-22Jan2013-v1/AOD). CERN Open Data Portal. DOI:10.7483/OPENDATA.CMS.YLIC.86ZZ

[2] Wunsch, Stefan; (2019). DYJetsToLL dataset in reduced NanoAOD format for education and outreach. CERN Open Data Portal. DOI:10.7483/OPENDATA.CMS.SRRA.2GON

[3] https://github.com/cms-opendata-analyses/AOD2NanoAODOutreachTool



# Used samples

For the case of this exemplary analysis (to limit the time spend by outside user on the processing), only a subset of the data files was used. These samples were:

- output_data_CMS_Run2012B_DoubleMuParked_AOD_22Jan2013-v1_20000_07.csv
- output_data_CMS_Run2012B_DoubleMuParked_AOD_22Jan2013-v1_20000_17.csv
- output_data_CMS_Run2012B_DoubleMuParked_AOD_22Jan2013-v1_20001_18.csv
- output_data_CMS_Run2012B_DoubleMuParked_AOD_22Jan2013-v1_20001_11.csv

They are also appended to the project in the folder "data".
The files are restricted under Creative Commons Attribution 4.0 International Licence.


# How to run the analysis on your own

In order to download the dataset to your workspace - use the command from the notebook cell:
!wget https://zenodo.org/record/5345875/files/DataFiles_csv.tar.gz


Then (to unpack the files):
!tar xvzf DataFiles_csv.tar.gz
Stop the execution after a few files - the statistics is large enough to be used in further calculations.
The files will be unpacked in folder "csv".
