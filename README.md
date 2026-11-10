# SARS-CoV-2 Spike–ACE2: a bioinformatics overview

A sequence-, structure- and epitope-level computational study of how the SARS-CoV-2 Spike glycoprotein interacts with human ACE2, written as a report at the GenoBiotek Internship.

**Full report:** [`report/Spike_ACE2_Overview_Soumik_Roy.pdf`](report/Spike_ACE2_Overview_Soumik_Roy.pdf) (55 pages)

## What this covers
- **Background:** Spike structure and function, ACE2 biology, viral entry, and Spike/ACE2 as vaccine and therapeutic targets.
- **Data:** Spike (UniProt P0DTC2.1) and human ACE2 (NP_001358344.1) sequences retrieved from NCBI.
- **Sequence analysis:** pairwise alignment (Needleman–Wunsch/BLAST concepts, PAM and BLOSUM scoring), dot-matrix plots, and EMBOSS tools (Dotmatcher, Pepstats, Antigenic).
- **Structure:** homology models (SWISS-MODEL) visualised in UCSF Chimera.
- **Phylogeny:** maximum-likelihood trees (MUSCLE alignment, 100 bootstrap replicates) of ACE2 and Spike homologs in MEGA.
- **Immunoinformatics:** MHC-II binding prediction (IEDB) and antibody-inducing epitope scans (IgPred).
- **Docking:** protein–protein docking of ACE2 with Spike using the HDOCK server.

## Selected figures
| | |
|---|---|
| ACE2 phylogeny across species | [figure](figures/ace2_phylogenetic_tree_report_p27.png) |
| Spike phylogeny and alignment tools | [figure](figures/spike_phylogeny_report_p28.png) |
| HDOCK result (ACE2–Spike) | [figure](figures/hdock_docking_report_p49.png) |
| Model quality report | [figure](figures/hdock_model_quality_report_p50.png) |

## Limitations (stated honestly)
- This is a **learning-oriented computational overview**, not new experimental research. Nothing here was validated in the lab.
- The HDOCK run reports a docking score of -251.95 and a confidence score of 0.8848, but also a **ligand RMSD of 178.46 Å**, which indicates a large uncertainty in the predicted pose.
- The Spike model was built on a template with a TM-score of about 0.60, which is only moderate confidence.
- Docking scores from a single web-server run should not be read as binding affinities.

## Tools
NCBI, UniProt, EMBOSS, SWISS-MODEL, UCSF Chimera, MEGA, MUSCLE, IEDB, IgPred, HDOCK.

## Author
Soumik Roy, M.Tech Computational Biology, IIIT Delhi (B.Tech Biotechnology, Adamas University).
