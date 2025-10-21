# Measuring changes in Plasmodium falciparum census population size in response to sequential malaria control interventions

If you use data from this work, please cite:

Tiedje KE, Zhan Q, Ruybal-Pésantez S, Tonkin-Hill G, He Q, Tan MH, Argyropoulos DC, Deed SL, Ghansah A, Bangre O, Oduro AR, Koram KA, Pascual M, Day KP. (2025) Measuring changes in Plasmodium falciparum census population size in response to sequential malaria control interventions. eLife 12: RP91411 [https://elifesciences.org/reviewed-preprints/91411v3](https://doi.org/10.7554/eLife.91411.3)


## Genotyping Protocols used in this study

* _P. falciparum var_ DBLα PCR: [Pfalciparum_varDBLalpha_PCR](https://github.com/UniMelb-Day-Lab/Pfalciparum_varDBLalpha_PCR)
> Note: This study used version 1 (v1) of DBLαAF and DBLαBR primers. For Version 1 the universal degenerate primers (i.e., forward primer: DBLαAF and reverse primer: DBLαBR) were coupled with a GS FLX Titanium primer sequence (i.e., adaptor). In addition, both the forward and reverse primers were barcoded with a unique 10 bp multiplex identifier (MID) tag ([Roche, 2009](https://www.scribd.com/doc/316505708/The-GS-FLX-Titanium-Chemistry-Extended-MID-Set-Copia)) for multiplexed sequencing.



## Data files: Descriptions

### MRS_eLife_Metadata_201025.csv
Metadata for all participants surveyed in each MRS survey (2012, 2014, 2015, and 2017).  
* **survey_year**: Survey year during which the participants were surveyed  
* **study_id**: General participant identifier  
* **mrs_study_id**: Unique identifier of isolate sent for DBLa sequencing  
* **age_groups**: Age group of participant  
* **pf_positive**: Microscopic *P. falciparum* status (i.e., Para+ = Pf positive; Para− = Pf negative)  
* **ParasiteuL**: Microscopic *P. falciparum* density (parasites/μL of blood)  
* **DBLa_ParaPos**: DBLa sequencing success for all isolates positive for *P. falciparum* by microscopy  
* **DBLa_rep_size**: Total number of DBLα types detected for the isolate (i.e., repertoire size)  
* **DBLa_upsA_rep_size**: Total number of upsA DBLα types (i.e., upsA repertoire size)  
* **DBLa_upsBC_rep_size**: Total number of non-upsA DBLα types (i.e., non-upsA repertoire size)  
* **MOI**: Multiplicity of infection based on varcoding  
* **MOI_group**: MOI groupings, MOI = 1 or MOI > 1  

This dataset can be used to generate the source data for the following figures and tables:
* **Figures**
  * Figure 1 B (see Fig1_B_all_prev.csv)
  * Figure 1 C (see Fig1_C_age_prev.csv)
  * Figure 3 - figure supplement 1 (i.e.,DBLa_upsA_rep_size and DBLa_upsBC_rep_size vs. survey_year)
  * Figure 4 A (see Fig4_A_all_census.csv)
  * Figure 4 B (see Fig4_B_age_census.csv)
  * Figure 4 C (see Fig4_C_all_prev_census.csv)
  * Figure 4 D (Fig4_D_age_prev_census.csv)

* **Tables**
  * Appendix 1-table 1
  * Appendix 1-table 2


### MRS_eLife_PTS_201025.csv
Contains the estimated genetic similarity between all pairs of isolates in each MRS survey (2012, 2014, 2015, and 2017), based on parwise type sharing (PTS).
PTS, analogous to the Sørensen Index, is a similarity statistic to evaluate the proportion of DBLα types shared between two isolate repertoires (i.e., DBLα repertoire overlap) and ranges from 0 (i.e., no DBLα repertoire overlap) to 1 (i.e., identical DBLα isolate repertoires).
* **mrs_study_id1**: Unique identifier of isolate sent for DBLa sequencing  
* **mrs_study_id2**: Unique identifier of isolate sent for DBLa sequencing  
* **PAS_score**: PTS score between **mrs_study_id1** and **mrs_study_id2** (all DBLα types)  
* **upsA_PAS_score**: PTS score between **mrs_study_id1** and **mrs_study_id2** (upsA DBLα types)  
* **upsBC_PAS_score**: PTS score between **mrs_study_id1** and **mrs_study_id2** (non-upsA DBLα types)  
* **survey_year1**: Survey year for **mrs_study_id1**  
* **study_id1**: General participant identifier for **mrs_study_id1**  
* **MOI1**: Multiplicity of infection based on varcoding for **mrs_study_id1**  
* **survey_year2**: Survey year for **mrs_study_id2**  
* **study_id2**: General participant identifier for **mrs_study_id2**  
* **MOI2**: Multiplicity of infection based on varcoding for **mrs_study_id2** 

This dataset can be used to generate the source data for the following figures:
* **Figures**
  * Figure 2 A (i.e.,upsA_PAS_score, plotted by survey_year1)
  * Figure 2 B (i.e.,upsBC_PAS_score, plotted by survey_year1)
  * Figure 2 - figure supplement 1 (i.e.,upsA_PAS_score vs. survey_year1 and upsBC_PAS_score vs. survey_year1; selecting MOI1 =1 and MOI2 = 1)


### MRS_eLife_DBLatypes_201025.csv
Contains the frequency and proportion of all DBLA types in each MRS survey (2012, 2014, 2015, and 2017). 
* **DBLa_type**: DBLα type
* **Ups**: DBLα type ups group (i.e., A = upsA and BC = non-upsA)
* **2012_freq/2014_freq/2015_freq/2017_freq**: Frequency or the number of times (i.e., number of isolates) a DBLα type was observed in each MRS survey (2012, 2014, 2015, and 2017)
* **2012_freqbin/2014_freqbin/2015_freqbin/2017_freqbin**: Frequency category (i.e., 0, 1, 2-10, 11-20, > 20 isolates) for the DBLα types observed in each MRS survey (2012, 2014, 2015, and 2017)

This dataset can be used to generate the source data for the following figures and tables:
* **Figures**
  * Figure 6 A and B (i.e., 2012_freq, 2014_freq, 2015_freq, and 2017_freq vs. DBLa_type, by Ups)
  * Figure 6 C and D (i.e., 2012_freqbin, 2014_freqbin, 2015_freqbin, and 2017_freqbin vs. DBLa_type, by Ups)
  * Figure 6 E and F (i.e., survival curves include only those DBLα types that were seen at baseline in 2012 (2012_freq, 2012freq_bin)))
  * Figure 6 - figure supplement 1 (i.e., frequency of 2012_freq, 2014_freq, 2015_freq, and 2017_freq vs. proportion, by Ups)

* **Tables**
  * Appendix 1-table 3


