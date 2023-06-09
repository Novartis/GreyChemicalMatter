# GreyChemicalMatter
A pipeline to identify bioactive small molecules with likely novel modes of actions and dynamic SAR from historic cell-HTS profiles, with an example application and hitlist from PubChem data



Grey Chemical Matter (GCM) is a small focused set of bioactive compounds with likely novel mode of actions (MoAs) for screening in phenotypic assays. The compounds are identified from their profiles over historic cellular High Throughput Screening (HTS) assays. Here we provide the code and results for the generation and analysis of GCM based on cell-HTS data from [PubChem BioAssays](https://pubchem.ncbi.nlm.nih.gov/docs/bioassays). Additionally we provide a shortlist of best GCM compounds from the PubChem data, that can be readily tested for novel disease associations, even in complex assays with low throughput. 

<br />
<br />

For questions and feedback reach out to [Steffen Renner](mailto:steffen.renner@novartis.com) or [Jason Thomas](mailto:jason.thomas@novartis.com).


<br />
<br />
   
The repository is organized into two folders: 
* create_gcm: Jupyter notebooks to calculate GCM from cell HTS data and store it in an SQLite database 
* gcm_tables: folder with the GCM data and Jupyter notebooks to extract data from the SQLite database 
	* **gcm.gcm_cpd_profile_scores.best.csv  - best scoring GCM compound for each GCM cluster from PubChem**
	* gcm.gcm_cpd_profile_scores.csv  - all compounds from PubChem GCM clusters with profile scores
	* gcm.gcm_cpds_assay_activity.csv - all compounds from PubChem GCM clusters with all cell HTS assay data
	* gcm.gcm_cluster_assay_stat.csv - assay enrichment data for all PubChem GCM clusters
	* gmc.gcm_cluster_summaries.csv - assay profile summaries for all PubChem GCM clusters
	* gcm.assay_meta.csv - PubChem assay metadata for all assays used for PubChem GCM



