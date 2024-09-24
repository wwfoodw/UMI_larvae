# UMI tagged bulk metabarcoding of Western Australian phyllosomas

This study uses unique molecular identifiers (UMIs) to individually label DNA before it undergoes PCR and sequencing. The basic rationale is that PCR and sequencing are known to introduce stochastic errors into the DNA sequence files obtained at the end of the process - but the UMIs inable us to track the fate of individual molecules through PCR and identify where errors occur. The lab protocol is described below. We have two biuoinformatic pipelines, which both an R package called UMIc (https://www.frontiersin.org/journals/genetics/articles/10.3389/fgene.2021.660366/full), but then diverge depending on whether they are investigating the intraspecific or interspecific dynamics of East Indian Ocean phyllosomas. 

Phyllosomas are the larvae of slipper and rock (spiny) lobsters. These larvae are characterised by travelling unusually long distances (10s to 100s of kilometers) for unusually long periods of time (months rather than days, even years). We look at intraspecific population dynamics of the Western Rock Lobster here (https://github.com/wwfoodw/UMI_larvae/blob/main/Population_UMI_metabarcoding_larvae.md), and interspecific details here (https://github.com/wwfoodw/UMI_larvae/blob/main/Species_Identification.md). 

# Lab protocol for UMI tagging

# Primers

i5_R13CN_12S_F_Achel :  5' - TCGTCGGCAGCGTC AGATGTGTATAAGAGACAG NNNNCNNNNCNNNNN GAAAGCGACGGGCAATATGTACA - 3'

i7_12S_R_Achel :        5' - GTCTCGTGGGCTCGG AGATGTGTATAAGAGACAG GTGCCAGCAKCCGCGGTTA - 3'

i5_min :                5' - TCGTCGGCAGCGTC AGATG - 3'

# Reaction conditions

The first stage of the process is to prepare the DNA for tagging with the UMIs, which in this case is 13 Ns interupted by a couple of Cs (NNNNCNNNNCNNNNN)
     
![image](https://github.com/user-attachments/assets/14258eb9-da21-48d1-98ca-beb7b434b74d)

95°C for 1 minute to melt DNA and then hold at 20°C
     
![image](https://github.com/user-attachments/assets/b814dcb2-1133-4a28-9727-0a5a0543240f)

hold at 60°C for 10 minutes, then 80°C for 45s, then hold at 37°C

then add exoI enzyme, hold for 3min at 37°C and then 30sec at 95°C

add labelled DNA to PCR:

![image](https://github.com/user-attachments/assets/4cf3e6bd-5544-4b78-a97a-0cd269b12415)

Thermocycler cinditions:

![image](https://github.com/user-attachments/assets/3ffb8a70-91e6-4a70-a913-1e9156c2e3b5)

Than add the i5 and i7 indices using the NEXTERA protocol
     
![image](https://github.com/user-attachments/assets/273181ad-e8fb-422d-9b28-aa369ba9cbfc)


![image](https://github.com/user-attachments/assets/0d76ce4c-8370-4960-8b74-1be8d26d4c17)
