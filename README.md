# Measuring changes in _Plasmodium falciparum_ census population size in response to sequential malaria control interventions

## Data Availability & Citation Statement

All data associated with this study, including de-identified individual participant data, are available in the manuscript, appendicies, or the accompanying GitHub repository [Census_Pop_Size_Pf_Ghana](https://github.com/UniMelb-Day-Lab/Census_Pop_Size_Pf_Ghana/tree/main/data).

Redistribution or reuse of these data requires proper attribution and prior approval. Researchers interested in further use of these data should contact the Malaria Reservoir Study Team, represented by the corresponding author, Prof. Karen Day (karen.day@unimelb.edu.au), to discuss how these data will be utilized for academic or research purposes and, if appropriate, to identify opportunities for collaboration.

If you use data from this work, please cite:
_Tiedje KE, Zhan Q, Ruybal-Pésantez S, Tonkin-Hill G, He Q, Tan MH, Argyropoulos DC, Deed SL, Ghansah A, Bangre O, Oduro AR, Koram KA, Pascual M, Day KP. (2025) Measuring changes in _Plasmodium falciparum_ census population size in response to sequential malaria control interventions. eLife 12: RP91411 [https://elifesciences.org/reviewed-preprints/91411v3](https://doi.org/10.7554/eLife.91411.3)_


## Human subject ethical approval

The study was reviewed/approved by the ethics committees at the Navrongo Health Research Centre Ghana (NHRC IRB-131), Noguchi Memorial Institute for Medical Research, Ghana (NMIMR-IRB CPN 089/11-12; NMIMR-IRB CPN 066/20-21), The University of Chicago, United States (IRB14-1495; IRB19-0760;  IRB21-0417), and New York University, United States (IRB-FY2024-8572), and The University of Melbourne, Australia (Project IDs 13433, 31586, 21649). Individual informed consent was obtained in the local language (i.e., Gurene) from each participant enrolled by signature or thumbprint, accompanied by the signature of an independent witness. For children < 18 years of age, a parent or guardian provided consent. In addition, all children between the ages of 12 and 17 provided assent. Details on the study area, study population, inclusion/exclusion criteria, and data collection procedures have been previously described ([Tiedje et al., 2017](https://pubmed.ncbi.nlm.nih.gov/28719306/), [Tiedje et al., 2022](https://journals.plos.org/globalpublichealth/article?id=10.1371/journal.pgph.0000285)).


## Genotyping protocols

* _P. falciparum var_ DBLα PCR: [Pfalciparum_varDBLalpha_PCR](https://github.com/UniMelb-Day-Lab/Pfalciparum_varDBLalpha_PCR)
> Note: This study used version 1 (v1) of DBLαAF and DBLαBR primers. For Version 1 the universal degenerate primers (i.e., forward primer: DBLαAF and reverse primer: DBLαBR) were coupled with a GS FLX Titanium primer sequence (i.e., adaptor). In addition, both the forward and reverse primers were barcoded with a unique 10 bp multiplex identifier (MID) tag ([Roche, 2009](https://www.scribd.com/doc/316505708/The-GS-FLX-Titanium-Chemistry-Extended-MID-Set-Copia)) for multiplexed sequencing.



## Sequence analysis pipelines

* Raw DBLα sequence tags were cleaned, clustered, and classified (upsA and non-upsA) using the following bioinformatic pipelines:
  * [DBLaCleaner](https://github.com/UniMelb-Day-Lab/DBLaCleaner)
  * [clusterDBLalpha](https://github.com/UniMelb-Day-Lab/clusterDBLalpha)
  * [classifyDBLalpha](https://github.com/UniMelb-Day-Lab/classifyDBLalpha)
> For additional information on the use of these bioinformatic pipelines a detailed tutorial is available: [tutorialDBLalpha](https://github.com/UniMelb-Day-Lab/tutorialDBLalpha).

*  For additional information on the use of the Bayesian approach to estimate MOIvar please see [Bayesian-formulation-varcoding-MOI-estimation](https://github.com/qzhan321/Bayesian-formulation-varcoding-MOI-estimation).



## Data files: Descriptions

## MRS_eLife_Metadata_201025.csv
Metadata for all participants surveyed in each MRS survey (2012, 2014, 2015, and 2017). This dataset includes de-identified information from individual survey participants in each MRS survey.
* **survey_year**: Survey year during which the participants were surveyed  
* **study_id**: General study participant ID  
* **mrs_study_id**: Unique study participant ID of isolate sent for DBLa sequencing  
* **age_groups**: Age group of participant  
* **pf_positive**: Microscopic *P. falciparum* status (i.e., Para+ = Pf positive; Para− = Pf negative)  
* **ParasiteuL**: Microscopic *P. falciparum* density (i.e., parasites per μL of blood)  
* **DBLa_ParaPos**: DBLa sequencing success for all isolates positive for *P. falciparum* by microscopy  
* **DBLa_rep_size**: Total number of DBLα types detected for the isolate (i.e., repertoire size)  
* **DBLa_upsA_rep_size**: Total number of upsA DBLα types (i.e., upsA repertoire size)  
* **DBLa_upsBC_rep_size**: Total number of non-upsA DBLα types (i.e., non-upsA repertoire size)  

This dataset represents the underlying source data used to generate the figures and tables listed below. In addition, we have provided supplementary source data files derived from this dataset for specific figures and tables where relevant.
* **Figures**
  * Figure 1 B (see Source Data: Fig1_B_all_prev.csv)
  * Figure 1 C (see Source Data: Fig1_C_age_prev.csv)
  * Figure 3 A & B (see Source Data: Fig3_MOI_estimation_pool.csv)
  * Figure 3 - figure supplement 1 (i.e., DBLa_upsA_rep_size and DBLa_upsBC_rep_size vs. survey_year)
  * Figure 3 - figure supplement 2 (see Source Data: Fig3_S2_MOI_estimation_mixtureDist.csv)
  * Figure 4 A (see Source Data: Fig4_A_all_census.csv)
  * Figure 4 B (see Source Data: Fig4_B_age_census.csv)
  * Figure 4 C (see Source Data: Fig4_C_all_prev_census.csv)
  * Figure 4 D (see Source Data: Fig4_D_age_prev_census.csv)
  * Appendix 1-Figure 1 (see Source Data: Appendix1_Fig1_meanMOI_subsampling.csv)
  * Appendix 1-Figure 4 (see Source Data: Appendix1_Fig4_measurementError.csv) 

* **Tables**
  * Appendix 1-table 1
  * Appendix 1-table 2


## MRS_eLife_PTS_201025.csv
This dataset contains the estimated genetic similarity between all pairs of _P. falciaparum_ isolates derived from participants in each MRS survey (2012, 2014, 2015, and 2017), based on parwise type sharing (PTS). This dataset includes relevant de-identified information from individual survey participants.

PTS, analogous to the Sørensen Index, is a similarity statistic to evaluate the proportion of DBLα types shared between two isolate repertoires (i.e., DBLα repertoire overlap) and ranges from 0 (i.e., no DBLα repertoire overlap) to 1 (i.e., identical DBLα isolate repertoires).
* **mrs_study_id1**: Unique study participant ID of isolate sent for DBLa sequencing  
* **mrs_study_id2**: Unique study participant ID of isolate sent for DBLa sequencing  
* **PAS_score**: PTS score between **mrs_study_id1** and **mrs_study_id2** (all DBLα types)  
* **upsA_PAS_score**: PTS score between **mrs_study_id1** and **mrs_study_id2** (upsA DBLα types)  
* **upsBC_PAS_score**: PTS score between **mrs_study_id1** and **mrs_study_id2** (non-upsA DBLα types)  
* **survey_year1**: Survey year for **mrs_study_id1**  
* **study_id1**: General study participant ID for **mrs_study_id1**  
* **MOI1**: Multiplicity of infection based on varcoding for **mrs_study_id1**  
* **survey_year2**: Survey year for **mrs_study_id2**  
* **study_id2**: General study participant ID for **mrs_study_id2**  
* **MOI2**: Multiplicity of infection based on varcoding for **mrs_study_id2** 

This dataset represents the underlying source data used to generate the figures listed below.
* **Figures**
  * Figure 2 A (i.e., upsA_PAS_score, plotted by survey_year1)
  * Figure 2 B (i.e., upsBC_PAS_score, plotted by survey_year1)
  * Figure 2 - figure supplement 1 (i.e., upsA_PAS_score vs. survey_year1 and upsBC_PAS_score vs. survey_year1; selecting MOI1 =1 and MOI2 = 1)


## MRS_eLife_DBLatypes_201025.csv
Contains the frequency and proportion of all DBLA types in each MRS survey (2012, 2014, 2015, and 2017). 
* **DBLa_type**: DBLα type
* **Ups**: DBLα type ups group (i.e., A = upsA and BC = non-upsA)
* **2012_freq/2014_freq/2015_freq/2017_freq**: Frequency or the number of times (i.e., number of isolates) a DBLα type was observed in each MRS survey (2012, 2014, 2015, and 2017)
* **2012_freqbin/2014_freqbin/2015_freqbin/2017_freqbin**: Frequency category (i.e., 0, 1, 2-10, 11-20, > 20 isolates) for the DBLα types observed in each MRS survey (2012, 2014, 2015, and 2017)
  
This dataset represents the underlying source data used to generate the figures and tables listed below. In addition, we have provided supplementary source data files derived from this dataset for specific figures and tables where relevant.
* **Figures**
  * Figure 5 A and B (see Source Data: Fig5_A_B_richness_prev.csv)
  * Figure 6 A and B (i.e., 2012_freq, 2014_freq, 2015_freq, and 2017_freq vs. DBLa_type, by Ups)
  * Figure 6 C and D (i.e., 2012_freqbin, 2014_freqbin, 2015_freqbin, and 2017_freqbin vs. DBLa_type, by Ups)
  * Figure 6 E and F (i.e., survival curves include only those DBLα types that were seen at baseline in 2012 (2012_freq; 2012freq_bin category))
  * Figure 6 - figure supplement 1 (i.e., frequency of 2012_freq, 2014_freq, 2015_freq, and 2017_freq vs. proportion, by Ups)

* **Tables**
  * Appendix 1-table 3 (in addition see Source Data: Fig5_A_B_richness_prev.csv)



