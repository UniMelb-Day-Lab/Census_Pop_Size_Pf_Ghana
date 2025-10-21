# Measuring changes in Plasmodium falciparum census population size in response to sequential malaria control interventions

If you use data or code from this work, please cite:

Tiedje KE, Zhan Q, Ruybal-Pésantez S, Tonkin-Hill G, He Q, Tan MH, Argyropoulos DC, Deed SL, Ghansah A, Bangre O, Oduro AR, Koram KA, Pascual M, Day KP. (2025) Measuring changes in Plasmodium falciparum census population size in response to sequential malaria control interventions. eLife 12: RP91411 [https://elifesciences.org/reviewed-preprints/91411v3](https://doi.org/10.7554/eLife.91411.3)


## Genotyping Protocols used in this study

* _P. falciparum var_ DBLα PCR: [Pfalciparum_varDBLalpha_PCR](https://github.com/UniMelb-Day-Lab/Pfalciparum_varDBLalpha_PCR)
> Note: This study used version 1 (v1) of DBLαAF and DBLαBR primers. For Version 1 the universal degenerate primers (i.e., forward primer: DBLαAF and reverse primer: DBLαBR) were coupled with a GS FLX Titanium primer sequence (i.e., adaptor). In addition, both the forward and reverse primers were barcoded with a unique 10 bp multiplex identifier (MID) tag ([Roche, 2009](https://www.scribd.com/doc/316505708/The-GS-FLX-Titanium-Chemistry-Extended-MID-Set-Copia)) for multiplexed sequencing.



## Data files: Descriptions

### MRS_eLife_Metadata_201025.csv
Metadata for all participants surveyed during the 2012, 2014, 2015, and 2017 MRS surveys.  
> ```
> survey_year: Survey year during which the participants were surveyed
> study_id: General participant identifier
> mrs_study_id: Unique identifier of isolate sent for DBLa sequencing
> age_groups: Age group of participant 
> pf_positive: Microscopic P. falciparum status (i.e., Para+ = Pf positive; Para- = Pf negative)
> ParasiteuL: Microscopic P. falciparum density (parasite/uL of blood)
> DBLa_ParaPos: DBLa sequencing success for all isolates positive for P. falciparum by microscopy
> DBLa_rep_size: Total number of DBLα types detected for the isolate (i.e. repertoire size)
> DBLa_upsA_rep_size: Total number of upsA DBLα types (i.e. upsA repertoire size)
> DBLa_upsBC_rep_size: Total number of non-upsA DBLα types (i.e. non-upsA repertoire size)
> MOI: multiplicity of infection based on varcoding
> MOI_group: MOI groupings, MOI = 1 or MOI > 1
> ```

### MRS_eLife_PTS_201025.csv
Contains the estiamted genetic similarity calculated between all pairs of isolates in each survey (2012, 2014, 2015, and 2017), based on parwise type sharing (PTS) 

> mrs_study_id1: Unique identifier of isolate sent for DBLa sequencing
> mrs_study_id2: Unique identifier of isolate sent for DBLa sequencing
> PAS_score: PTS score between mrs_study_id1 and mrs_study_id2 (all DBLα types)
> upsA_PAS_score: PTS score between mrs_study_id1 and mrs_study_id2 (upsA DBLα types)
> upsBC_PAS_score: PTS score between mrs_study_id1 and mrs_study_id2 (non-upsA DBLα types)
> survey_year1: Survey year for mrs_study_id1
> study_id1: General participant identifier for mrs_study_id1
> MOI1: multiplicity of infection based on varcoding for mrs_study_id1
> survey_year2: Survey year for mrs_study_id2
> study_id2: General participant identifier for mrs_study_id2
> MOI2: multiplicity of infection based on varcoding for mrs_study_id2

